---
title: 将 Azure AD Graph .NET 应用迁移到 Microsoft Graph
description: 介绍如何将 Azure Active Directory （Azure AD） API 应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 884802fafcccf4408b84da96f6c4f94818e31b16
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234038"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>将 .NET 客户端库使用迁移到 Microsoft Graph

本文是*第3步：查看迁移应用程序的应用程序详细信息的第3步：查看*该[过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。

如果你的应用当前使用的是 Azure AD Graph 客户端库，请切换到[Microsoft Graph .net 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)。

>注意：仅 .NET Framework 4.5 和 .NET Standard 1.1 支持 Microsoft Graph .NET 客户端库。  但请参阅 Microsoft Graph .NET 客户端库，了解最新的支持信息。

在这里，我们将介绍一些将迁移到 Microsoft Graph .NET 客户端库的常规步骤：

- 如何创建 Microsoft Graph 客户端，给定访问令牌（您可以使用 ADAL 或 MSAL 获取）
- 如何表述请求
- 如何使用查询生成器
- 如何处理集合和分页  

## <a name="overview-of-the-migration-steps"></a>迁移步骤概述

以下步骤假定您的应用程序已在使用 ADAL 获取访问令牌以调用 Azure AD Graph，而现在您将继续使用 ADAL。 切换到 MSAL 可作为[迁移到 MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal)中所述的一个单独步骤完成。

1. 若要获取 Microsoft Graph 的访问令牌，请**** 将 resourceUrl `https://graph.windows.net`更新`https://graph.microsoft.com`为。

2. 在您的应用程序中，通过更改以下内容更新对 Microsoft Graph 客户端库的引用：

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    自：

    ``` csharp
    using Microsoft.Graph;
    ```

3. 使用您的程序包管理器下载并更新[Microsoft Graph NuGet 包](https://www.nuget.org/packages/Microsoft.Graph/)并更新依赖项。

4. 更新客户端构造函数`GraphServiceClient`，以创建而不`ActiveDirectoryClient`是。  以下代码段假定应用程序正在使用获取新`AcquireTokenAsyncForUser()`令牌的方法。 您可以在[active directory-dotnet-graphapi 示例](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)中查找此方法的定义。

    更改

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    自：

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    对于 Microsoft Graph 客户端库， `serviceRoot`此值还包括版本号。 目前，该值为`https://graph.microsoft.com/v1.0`。

5. 通过更改以下内容，更新请求以使用 Microsoft Graph 客户端请求生成器语法：

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    自：

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    >Azure AD Graph 客户端库支持基于 LINQ 的查询语法。 但是，Microsoft Graph 客户端库不会。  因此，您需要将相关查询转换为更 RESTful 的表达式。  

    为此，请更改：

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    自：

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. 如果您的代码通过集合进行分页，请进行以下次要调整。 下面的示例比较并对比提取组和对其成员进行分页（一次5次）。 虽然 Azure AD Graph 的代码需要 fetcher 构造才能获取组的成员，但 Microsoft Graph 没有这样的要求。 另一方面，代码相对相似。  为简洁，仅显示用户成员，不显示 try/catch 和错误条件，并且代码段适用于单线程控制台应用程序。

    例如，使用 Azure AD Graph .NET 客户端库更改以下代码：

    ```csharp
    Group retrievedGroup = client.Groups.
        Where(g => g.ObjectId.Equals(id)).ExecuteAsync().Result;
    IGroupFetcher retrievedGroupFetcher = (IGroupFetcher) retrievedGroup;

    var membersPage = retrievedGroupFetcher.Members.Take(5).ExecuteAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<IDirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (IDirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        membersPage = membersPage.GetNextPageAsync().Result;
    } while (membersPage != null);

    ```

    使用 Microsoft Graph .NET 客户端库的以下代码：

    ```csharp
    var membersPage = client.Groups[id].Members.Request().Top(5).GetAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<DirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (DirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        if (membersPage.NextPageRequest != null)
            membersPage = membersPage.NextPageRequest.GetAsync().Result;
        else membersPage = null;
    } while (membersPage != null);

    ```

7. 生成并修复任何资源、属性、导航和服务操作错误，这些错误通常与名称更改有关。

## <a name="see-also"></a>另请参阅

[C # 控制台代码段应用程序](https://github.com/microsoftgraph/console-csharp-snippets-sample)重点介绍了 Microsoft Graph 客户端库和 Azure AD Graph 客户端库之间的差异。

Azure AD Graph 客户端库仅支持 .NET 平台。  但是，Microsoft Graph 客户端库支持其他[平台和语言](/graph)，您可能会发现更适合您的解决方案。

## <a name="next-steps"></a>后续步骤

- 了解如何[部署、测试和扩展](/graph/migrate-azure-ad-graph-deploy-test-extend)已迁移到 Microsoft Graph 的应用程序。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
