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
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="6ba50-103">将 .NET 客户端库使用迁移到 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6ba50-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="6ba50-104">本文是*第3步：查看迁移应用程序的应用程序详细信息的第3步：查看*该[过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6ba50-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="6ba50-105">如果你的应用当前使用的是 Azure AD Graph 客户端库，请切换到[Microsoft Graph .net 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)。</span><span class="sxs-lookup"><span data-stu-id="6ba50-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="6ba50-106">注意：仅 .NET Framework 4.5 和 .NET Standard 1.1 支持 Microsoft Graph .NET 客户端库。</span><span class="sxs-lookup"><span data-stu-id="6ba50-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="6ba50-107">但请参阅 Microsoft Graph .NET 客户端库，了解最新的支持信息。</span><span class="sxs-lookup"><span data-stu-id="6ba50-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="6ba50-108">在这里，我们将介绍一些将迁移到 Microsoft Graph .NET 客户端库的常规步骤：</span><span class="sxs-lookup"><span data-stu-id="6ba50-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="6ba50-109">如何创建 Microsoft Graph 客户端，给定访问令牌（您可以使用 ADAL 或 MSAL 获取）</span><span class="sxs-lookup"><span data-stu-id="6ba50-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="6ba50-110">如何表述请求</span><span class="sxs-lookup"><span data-stu-id="6ba50-110">How to formulate requests</span></span>
- <span data-ttu-id="6ba50-111">如何使用查询生成器</span><span class="sxs-lookup"><span data-stu-id="6ba50-111">How to use query builders</span></span>
- <span data-ttu-id="6ba50-112">如何处理集合和分页</span><span class="sxs-lookup"><span data-stu-id="6ba50-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="6ba50-113">迁移步骤概述</span><span class="sxs-lookup"><span data-stu-id="6ba50-113">Overview of the migration steps</span></span>

<span data-ttu-id="6ba50-114">以下步骤假定您的应用程序已在使用 ADAL 获取访问令牌以调用 Azure AD Graph，而现在您将继续使用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="6ba50-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="6ba50-115">切换到 MSAL 可作为[迁移到 MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal)中所述的一个单独步骤完成。</span><span class="sxs-lookup"><span data-stu-id="6ba50-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).</span></span>

1. <span data-ttu-id="6ba50-116">若要获取 Microsoft Graph 的访问令牌，请\*\*\*\* 将 resourceUrl `https://graph.windows.net`更新`https://graph.microsoft.com`为。</span><span class="sxs-lookup"><span data-stu-id="6ba50-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="6ba50-117">在您的应用程序中，通过更改以下内容更新对 Microsoft Graph 客户端库的引用：</span><span class="sxs-lookup"><span data-stu-id="6ba50-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="6ba50-118">自：</span><span class="sxs-lookup"><span data-stu-id="6ba50-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="6ba50-119">使用您的程序包管理器下载并更新[Microsoft Graph NuGet 包](https://www.nuget.org/packages/Microsoft.Graph/)并更新依赖项。</span><span class="sxs-lookup"><span data-stu-id="6ba50-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="6ba50-120">更新客户端构造函数`GraphServiceClient`，以创建而不`ActiveDirectoryClient`是。</span><span class="sxs-lookup"><span data-stu-id="6ba50-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="6ba50-121">以下代码段假定应用程序正在使用获取新`AcquireTokenAsyncForUser()`令牌的方法。</span><span class="sxs-lookup"><span data-stu-id="6ba50-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="6ba50-122">您可以在[active directory-dotnet-graphapi 示例](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)中查找此方法的定义。</span><span class="sxs-lookup"><span data-stu-id="6ba50-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="6ba50-123">更改</span><span class="sxs-lookup"><span data-stu-id="6ba50-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="6ba50-124">自：</span><span class="sxs-lookup"><span data-stu-id="6ba50-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="6ba50-125">对于 Microsoft Graph 客户端库， `serviceRoot`此值还包括版本号。</span><span class="sxs-lookup"><span data-stu-id="6ba50-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="6ba50-126">目前，该值为`https://graph.microsoft.com/v1.0`。</span><span class="sxs-lookup"><span data-stu-id="6ba50-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="6ba50-127">通过更改以下内容，更新请求以使用 Microsoft Graph 客户端请求生成器语法：</span><span class="sxs-lookup"><span data-stu-id="6ba50-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="6ba50-128">自：</span><span class="sxs-lookup"><span data-stu-id="6ba50-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    ><span data-ttu-id="6ba50-129">Azure AD Graph 客户端库支持基于 LINQ 的查询语法。</span><span class="sxs-lookup"><span data-stu-id="6ba50-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="6ba50-130">但是，Microsoft Graph 客户端库不会。</span><span class="sxs-lookup"><span data-stu-id="6ba50-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="6ba50-131">因此，您需要将相关查询转换为更 RESTful 的表达式。</span><span class="sxs-lookup"><span data-stu-id="6ba50-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="6ba50-132">为此，请更改：</span><span class="sxs-lookup"><span data-stu-id="6ba50-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="6ba50-133">自：</span><span class="sxs-lookup"><span data-stu-id="6ba50-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="6ba50-134">如果您的代码通过集合进行分页，请进行以下次要调整。</span><span class="sxs-lookup"><span data-stu-id="6ba50-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="6ba50-135">下面的示例比较并对比提取组和对其成员进行分页（一次5次）。</span><span class="sxs-lookup"><span data-stu-id="6ba50-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="6ba50-136">虽然 Azure AD Graph 的代码需要 fetcher 构造才能获取组的成员，但 Microsoft Graph 没有这样的要求。</span><span class="sxs-lookup"><span data-stu-id="6ba50-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="6ba50-137">另一方面，代码相对相似。</span><span class="sxs-lookup"><span data-stu-id="6ba50-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="6ba50-138">为简洁，仅显示用户成员，不显示 try/catch 和错误条件，并且代码段适用于单线程控制台应用程序。</span><span class="sxs-lookup"><span data-stu-id="6ba50-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="6ba50-139">例如，使用 Azure AD Graph .NET 客户端库更改以下代码：</span><span class="sxs-lookup"><span data-stu-id="6ba50-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

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

    <span data-ttu-id="6ba50-140">使用 Microsoft Graph .NET 客户端库的以下代码：</span><span class="sxs-lookup"><span data-stu-id="6ba50-140">To the following code using the Microsoft Graph .NET client library:</span></span>

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

7. <span data-ttu-id="6ba50-141">生成并修复任何资源、属性、导航和服务操作错误，这些错误通常与名称更改有关。</span><span class="sxs-lookup"><span data-stu-id="6ba50-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="6ba50-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6ba50-142">See also</span></span>

<span data-ttu-id="6ba50-143">[C # 控制台代码段应用程序](https://github.com/microsoftgraph/console-csharp-snippets-sample)重点介绍了 Microsoft Graph 客户端库和 Azure AD Graph 客户端库之间的差异。</span><span class="sxs-lookup"><span data-stu-id="6ba50-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="6ba50-144">Azure AD Graph 客户端库仅支持 .NET 平台。</span><span class="sxs-lookup"><span data-stu-id="6ba50-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="6ba50-145">但是，Microsoft Graph 客户端库支持其他[平台和语言](/graph)，您可能会发现更适合您的解决方案。</span><span class="sxs-lookup"><span data-stu-id="6ba50-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6ba50-146">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6ba50-146">Next Steps</span></span>

- <span data-ttu-id="6ba50-147">了解如何[部署、测试和扩展](/graph/migrate-azure-ad-graph-deploy-test-extend)已迁移到 Microsoft Graph 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6ba50-147">Learn how to [deploy, test, and extend](/graph/migrate-azure-ad-graph-deploy-test-extend) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="6ba50-148">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="6ba50-148">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="6ba50-149">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6ba50-149">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
