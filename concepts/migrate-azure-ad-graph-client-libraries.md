---
title: 将 Azure AD Graph .NET 应用迁移到 Microsoft Graph
description: 介绍如何将 Azure Active Directory (Azure AD) API 应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 286f631a9d5787d972e8d7db2559b0c359384c75
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761295"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="e63e9-103">将 .NET 客户端库使用迁移到 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e63e9-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="e63e9-104">本文是步骤 *3：查看应用程序迁移*[过程的详细信息的一部分](migrate-azure-ad-graph-planning-checklist.md)。</span><span class="sxs-lookup"><span data-stu-id="e63e9-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="e63e9-105">如果你的应用当前使用 Azure AD Graph 客户端库，请切换到 [Microsoft Graph .NET 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)。</span><span class="sxs-lookup"><span data-stu-id="e63e9-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="e63e9-106">注意：Microsoft Graph .NET 客户端库仅支持 .NET Framework 4.5 和 .NET Standard 1.1。</span><span class="sxs-lookup"><span data-stu-id="e63e9-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="e63e9-107">但是，请参阅 Microsoft Graph .NET 客户端库，获取最新的支持信息。</span><span class="sxs-lookup"><span data-stu-id="e63e9-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="e63e9-108">下面我们将了解迁移到 Microsoft Graph .NET 客户端库的一些常规步骤：</span><span class="sxs-lookup"><span data-stu-id="e63e9-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="e63e9-109">如何创建 Microsoft Graph 客户端（给定访问令牌 (可以使用 ADAL 或 MSAL 令牌获取) </span><span class="sxs-lookup"><span data-stu-id="e63e9-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="e63e9-110">如何制定请求</span><span class="sxs-lookup"><span data-stu-id="e63e9-110">How to formulate requests</span></span>
- <span data-ttu-id="e63e9-111">如何使用查询生成器</span><span class="sxs-lookup"><span data-stu-id="e63e9-111">How to use query builders</span></span>
- <span data-ttu-id="e63e9-112">如何处理集合和分页</span><span class="sxs-lookup"><span data-stu-id="e63e9-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="e63e9-113">迁移步骤概述</span><span class="sxs-lookup"><span data-stu-id="e63e9-113">Overview of the migration steps</span></span>

<span data-ttu-id="e63e9-114">以下步骤假定你的应用已使用 ADAL 获取访问令牌以调用 Azure AD Graph，并且目前你将继续使用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="e63e9-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="e63e9-115">切换到 MSAL 可以迁移到 MSAL 中所述的单独 [步骤完成](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal)。</span><span class="sxs-lookup"><span data-stu-id="e63e9-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal).</span></span>

1. <span data-ttu-id="e63e9-116">若要获取 Microsoft Graph 的访问令牌，请从 **将 resourceUrl** 更新 `https://graph.windows.net` 为 `https://graph.microsoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="e63e9-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="e63e9-117">在应用中，通过以下更改更新对 Microsoft Graph 客户端库的引用：</span><span class="sxs-lookup"><span data-stu-id="e63e9-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="e63e9-118">自：</span><span class="sxs-lookup"><span data-stu-id="e63e9-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="e63e9-119">使用程序包管理器下载和更新 [Microsoft Graph NuGet 程序包](https://www.nuget.org/packages/Microsoft.Graph/) 并更新依赖项。</span><span class="sxs-lookup"><span data-stu-id="e63e9-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="e63e9-120">更新客户端构造函数以创建 `GraphServiceClient` ，而不是 `ActiveDirectoryClient` 。</span><span class="sxs-lookup"><span data-stu-id="e63e9-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="e63e9-121">以下代码段假设你的应用使用 方法 `AcquireTokenAsyncForUser()` 获取新令牌。</span><span class="sxs-lookup"><span data-stu-id="e63e9-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="e63e9-122">作为 [active-directory-dotnet-graphapi-console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)示例的一部分，可以找到此方法的定义。</span><span class="sxs-lookup"><span data-stu-id="e63e9-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="e63e9-123">更改：</span><span class="sxs-lookup"><span data-stu-id="e63e9-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="e63e9-124">自：</span><span class="sxs-lookup"><span data-stu-id="e63e9-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="e63e9-125">对于 Microsoft Graph 客户端库， `serviceRoot` 值还包括版本号。</span><span class="sxs-lookup"><span data-stu-id="e63e9-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="e63e9-126">目前，该值为 `https://graph.microsoft.com/v1.0` 。</span><span class="sxs-lookup"><span data-stu-id="e63e9-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="e63e9-127">更新请求以使用 Microsoft Graph 客户端请求生成器语法，方法为：</span><span class="sxs-lookup"><span data-stu-id="e63e9-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="e63e9-128">自：</span><span class="sxs-lookup"><span data-stu-id="e63e9-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    ><span data-ttu-id="e63e9-129">Azure AD Graph 客户端库支持基于 LINQ 的查询语法。</span><span class="sxs-lookup"><span data-stu-id="e63e9-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="e63e9-130">但是，Microsoft Graph 客户端库没有。</span><span class="sxs-lookup"><span data-stu-id="e63e9-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="e63e9-131">因此，您需要将相关查询转换为更 RESTful 表达式。</span><span class="sxs-lookup"><span data-stu-id="e63e9-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="e63e9-132">为此，请更改：</span><span class="sxs-lookup"><span data-stu-id="e63e9-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="e63e9-133">自：</span><span class="sxs-lookup"><span data-stu-id="e63e9-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="e63e9-134">如果代码浏览集合，请进行以下细微的调整。</span><span class="sxs-lookup"><span data-stu-id="e63e9-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="e63e9-135">以下示例将一个组提取和分页及其成员（一次 5 个）进行比较。</span><span class="sxs-lookup"><span data-stu-id="e63e9-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="e63e9-136">虽然 Azure AD Graph 的代码需要提取器构造才能提取组的成员，但 Microsoft Graph 没有此类要求。</span><span class="sxs-lookup"><span data-stu-id="e63e9-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="e63e9-137">除了这一点外，代码相对类似。</span><span class="sxs-lookup"><span data-stu-id="e63e9-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="e63e9-138">为简洁明了，只显示用户成员，不显示尝试/捕获和错误条件，并且代码段适用于单线程控制台应用。</span><span class="sxs-lookup"><span data-stu-id="e63e9-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="e63e9-139">例如，使用 Azure AD Graph .NET 客户端库更改以下代码：</span><span class="sxs-lookup"><span data-stu-id="e63e9-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

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

    <span data-ttu-id="e63e9-140">对于以下使用 Microsoft Graph .NET 客户端库的代码：</span><span class="sxs-lookup"><span data-stu-id="e63e9-140">To the following code using the Microsoft Graph .NET client library:</span></span>

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

7. <span data-ttu-id="e63e9-141">生成并修复任何资源、属性、导航和服务操作错误，通常与名称更改相关。</span><span class="sxs-lookup"><span data-stu-id="e63e9-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="e63e9-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e63e9-142">See also</span></span>

<span data-ttu-id="e63e9-143">此 [C#代码](https://github.com/microsoftgraph/console-csharp-snippets-sample) 段应用重点介绍了 Microsoft Graph 客户端库和 Azure AD Graph 客户端库之间的更多差异。</span><span class="sxs-lookup"><span data-stu-id="e63e9-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="e63e9-144">Azure AD Graph 客户端库仅支持 .NET 平台。</span><span class="sxs-lookup"><span data-stu-id="e63e9-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="e63e9-145">但是，Microsoft Graph 客户端库支持 [其他平台和语言](/graph) ，你可能会发现这些平台和语言对解决方案更有用。</span><span class="sxs-lookup"><span data-stu-id="e63e9-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e63e9-146">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e63e9-146">Next Steps</span></span>

- <span data-ttu-id="e63e9-147">了解如何 [部署、测试和扩展](./migrate-azure-ad-graph-deploy-test-extend.md) 已迁移到 Microsoft Graph 的应用。</span><span class="sxs-lookup"><span data-stu-id="e63e9-147">Learn how to [deploy, test, and extend](./migrate-azure-ad-graph-deploy-test-extend.md) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="e63e9-148">再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。</span><span class="sxs-lookup"><span data-stu-id="e63e9-148">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
