---
title: 结合使用 Postman 和 Microsoft Graph API
description: 使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: c7029a68314c0a093e0943bcdad46be27155ca25
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556213"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="d7d5a-103">结合使用 Postman 和 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="d7d5a-103">Use Postman with the Microsoft Graph API</span></span>

<span data-ttu-id="d7d5a-104">使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Postman 图像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="d7d5a-106">本文介绍了如何快速掌握 Postman 和 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="d7d5a-107">此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="d7d5a-108">访问集合</span><span class="sxs-lookup"><span data-stu-id="d7d5a-108">Accessing the collection</span></span>
<span data-ttu-id="d7d5a-109">可通过以下两种方法来访问 Postman 中的集合：使用集合或参与集合。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="d7d5a-110">必须先在计算机上运行 [Postman](https://www.getpostman.com/)。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="d7d5a-111">使用集合</span><span class="sxs-lookup"><span data-stu-id="d7d5a-111">Consume the collection</span></span>
<span data-ttu-id="d7d5a-112">使用集合是开始使用 Microsoft Graph API 的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="d7d5a-113">若要导入 Postman 集合，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="d7d5a-113">To import the Postman collections:</span></span>

1. <span data-ttu-id="d7d5a-114">下载并注册 [Postman](https://www.getpostman.com/)。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-114">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="d7d5a-115">依次选择“文件 | 导入”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-115">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="d7d5a-116">选择“从链接导入”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-116">Select **Import From Link**.</span></span>
4. <span data-ttu-id="d7d5a-117">粘贴以下两个 URL，再选择每个 URL 后面的“导入”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-117">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_environment.json

    ```

<span data-ttu-id="d7d5a-118">现在，应该会在右上角的环境下拉列表中看到“Microsoft Graph 环境”（以眼睛图标为标识）。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-118">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="d7d5a-119">现在需要[创建环境](#using-the-collection)。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-119">Now you need to  [set up your environment](#using-the-collection).</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="d7d5a-120">使用集合</span><span class="sxs-lookup"><span data-stu-id="d7d5a-120">Using the collection</span></span>
<span data-ttu-id="d7d5a-121">在 Postman 中创建 **Microsoft Graph** 集合和 **Microsoftr Graph 环境** 后，请按照以下步骤操作。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-121">After you have the **Microsoft Graph** collection and the **Microsoft Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="d7d5a-122">设置应用程序 API 调用</span><span class="sxs-lookup"><span data-stu-id="d7d5a-122">Set up application API calls</span></span>

1. <span data-ttu-id="d7d5a-123">选择右上角的下拉列表中的“无环境”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-123">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="d7d5a-124">选择“Microsoft Graph 环境”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-124">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="d7d5a-125">依次选择右侧的 **眼睛** 图标和“编辑”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-125">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="d7d5a-126">在 **当前** （而不是 **初始** ）变量中，输入你的 Microsoft 标识应用程序： **ClientID** 、 **ClientSecret** 和 **TenantID** 。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-126">Enter your Microsoft Identity Application in the **current** (not **initial** ) variables: **ClientID** , **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="d7d5a-127">若要详细了解如何创建应用程序，以及如何让管理员同意仅限应用的流，请参阅[使用 Postman 执行 Microsoft Graph 调用](https://developer.microsoft.com/zh-CN/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/)博客文章。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-127">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/zh-CN/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="d7d5a-128">选择“更新”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-128">Select **Update**.</span></span> <span data-ttu-id="d7d5a-129">关闭“管理环境”对话框。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-129">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="d7d5a-130">在左侧的“ **MicrosoftGraph | 应用程序** ”集合中，选择“ **获取仅限应用的访问令牌** ”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-130">In the **MicrosoftGraph | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="d7d5a-131">然后，选择右侧的“发送”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-131">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="d7d5a-132">依次展开“应用程序 | 用户”文件夹，再选择“获取用户”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-132">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="d7d5a-133">然后，选择“发送”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-133">Then choose **Send**.</span></span>

<span data-ttu-id="d7d5a-134">现在，你可以开始使用 Microsoft Graph 集合了。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-134">You are now up and running with the Microsoft Graph collections.</span></span>

><span data-ttu-id="d7d5a-135">**注意：** 若要在集合中运行其他 API，需要同意应用程序拥有必需权限。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-135">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="d7d5a-136">设置代表 API 调用</span><span class="sxs-lookup"><span data-stu-id="d7d5a-136">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="d7d5a-137">设置代表 API 调用的最简单方法是，在环境设置中提供 **UserName** 和 **UserPassword** ，并使用“代表用户 | 获取用户访问令牌”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-137">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="d7d5a-138">**重要提示** ：不建议使用生产用户帐户，因为此信息直接存储在 Postman 中。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-138">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="d7d5a-139">也不建议使用这种方法在生产中获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-139">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="d7d5a-140">只能用于测试目的。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-140">Use it only for testing purposes.</span></span>

<span data-ttu-id="d7d5a-141">如果不希望在同步到 Postman 云帐户的环境变量中存储用户名和密码，可使用“获取新访问令牌”功能来获取令牌，而无需离开 Postman。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-141">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="d7d5a-142">选择“代表用户 | 使用 Postman 获取访问令牌”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-142">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="d7d5a-143">选择“授权”选项卡。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-143">Choose the **Authorization** tab.</span></span>
3. <span data-ttu-id="d7d5a-144">选择“获取新访问令牌”按钮。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-144">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="d7d5a-145">使用真实的租户和应用程序值填写以下框。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-145">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="d7d5a-146">请注意，不能在此处使用环境变量；必须使用实际值。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-146">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="d7d5a-147">若要查找这些值，可以选择 portal.azure.com 上“应用程序”边栏选项卡中的“终结点”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-147">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="d7d5a-148">回调 URL：https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="d7d5a-148">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="d7d5a-149">验证 URL：https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="d7d5a-149">Auth URL: https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="d7d5a-150">访问令牌 URL：https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="d7d5a-150">Access Token URL: https://login.microsoftonline.com/**TENANTID** /oauth2/v2.0/token</span></span>
    - <span data-ttu-id="d7d5a-151">客户端 ID： **CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="d7d5a-151">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="d7d5a-152">客户端密码： **CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="d7d5a-152">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="d7d5a-153">作用域：https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="d7d5a-153">Scope: https://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="d7d5a-154">状态： **RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="d7d5a-154">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="d7d5a-155">选择“请求令牌”。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-155">Choose **Request Token**.</span></span> <span data-ttu-id="d7d5a-156">应该会看到 UI 提示，提示你登录和同意权限。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-156">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="d7d5a-157">复制访问令牌，打开环境变量，并将它粘贴到“UserAccessToken”字段中。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-157">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="d7d5a-158">现在，所有请求都将可以正常运行。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-158">Now all your requests will work.</span></span>


### <a name="contribute-to-the-collection"></a><span data-ttu-id="d7d5a-159">参与集合</span><span class="sxs-lookup"><span data-stu-id="d7d5a-159">Contribute to the collection</span></span>
<span data-ttu-id="d7d5a-160">若要贡献你自己的请求，需要为 [Microsoft Graph Postman 集合](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github 存储库创建分支。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-160">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="d7d5a-161">若要详细了解如何执行此操作，请观看以下视频。</span><span class="sxs-lookup"><span data-stu-id="d7d5a-161">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]
