---
title: 将 Azure AD Graph .NET 应用迁移到 Microsoft Graph
description: 介绍如何将 Azure AD Azure Active Directory (API) 迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: f4c85cd926ee75b7442ece4f6b113d63eb525937bc51550601d56dd41f83fc9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163493"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>将 .NET 客户端库使用迁移到 Microsoft Graph

本文是步骤 *3：查看应用程序迁移*[过程的详细信息的一部分](migrate-azure-ad-graph-planning-checklist.md)。

如果你的应用当前使用 Azure AD Graph客户端库，请切换到 Microsoft [Graph .NET 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)。

>注意：Microsoft Graph .NET 客户端库仅适用于 .NET Framework 4.5 和 .NET Standard 1.1。  但是，请咨询 Microsoft Graph .NET 客户端库，获取最新的支持信息。

下面我们将了解迁移到 Microsoft Graph .NET 客户端库的一些常规步骤：

- 如何创建 Microsoft Graph 客户端，假设 (ADAL 或 MSAL 令牌获取) 
- 如何制定请求
- 如何使用查询生成器
- 如何处理集合和分页  

## <a name="overview-of-the-migration-steps"></a>迁移步骤概述

以下步骤假定你的应用已使用 ADAL 获取访问令牌以调用 Azure AD Graph，并且目前你将继续使用 ADAL。 切换到 MSAL 可以迁移到 MSAL 中所述的单独 [步骤完成](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal)。

1. 若要获取 Microsoft Graph访问令牌，请从 **将 resourceUrl** 更新 `https://graph.windows.net` 为 `https://graph.microsoft.com` 。

2. 在应用中，通过更改以下Graph Microsoft 客户端库的引用：

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    自：

    ``` csharp
    using Microsoft.Graph;
    ```

3. 使用程序包管理器下载和更新 Microsoft Graph NuGet[程序包](https://www.nuget.org/packages/Microsoft.Graph/)和更新依赖项。

4. 更新客户端构造函数以创建 `GraphServiceClient` ，而不是 `ActiveDirectoryClient` 。  以下代码段假设你的应用使用 方法 `AcquireTokenAsyncForUser()` 获取新令牌。 作为 [active-directory-dotnet-graphapi-console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)示例的一部分，可以找到此方法的定义。

    更改：

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

    对于 Microsoft Graph客户端库， `serviceRoot` 该值还包括版本号。 目前，该值为 `https://graph.microsoft.com/v1.0` 。

5. 更新请求以使用 Microsoft Graph客户端请求生成器语法，方法为：

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    自：

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    >Azure AD Graph客户端库支持基于 LINQ 的查询语法。 但是，Microsoft Graph客户端库不会。  因此，您需要将相关查询转换为更 RESTful 表达式。  

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

6. 如果代码浏览集合，请进行以下细微的调整。 以下示例将一个组提取和分页及其成员（一次 5 个）进行比较。 虽然 Azure AD Graph需要提取程序结构才能提取组的成员，但 Microsoft Graph没有此类要求。 除了这一点外，代码相对类似。  为简洁明了，只显示用户成员，不显示尝试/捕获和错误条件，并且代码段适用于单线程控制台应用。

    例如，使用 Azure AD 和 .NET 客户端库Graph以下代码：

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

    对于以下使用 Microsoft Graph .NET 客户端库的代码：

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

7. 生成并修复任何资源、属性、导航和服务操作错误，通常与名称更改相关。

## <a name="see-also"></a>另请参阅

此[C#控制台代码](https://github.com/microsoftgraph/console-csharp-snippets-sample)段应用重点介绍了 Microsoft Graph 客户端库和 Azure AD Graph客户端库之间的更多差异。

Azure AD Graph客户端库仅支持 .NET 平台。  但是，microsoft Graph 客户端库支持[其他平台](/graph)和语言，您可能会发现这些平台和语言对解决方案更有用。

## <a name="next-steps"></a>后续步骤

- 了解如何[部署、测试和扩展](./migrate-azure-ad-graph-deploy-test-extend.md)已迁移到 Microsoft Graph。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
