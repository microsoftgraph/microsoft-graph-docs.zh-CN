---
title: 结合使用 Postman 和 Microsoft Graph API
description: 使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: e548fed509bcf26ce7c733354a5ab3c52ab551c1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868483"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="f5f09-103">结合使用 Postman 和 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="f5f09-103">Use Postman with the Microsoft Graph API</span></span>

<span data-ttu-id="f5f09-104">使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="f5f09-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Postman 图像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="f5f09-106">本文介绍了如何快速掌握 Postman 和 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="f5f09-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="f5f09-107">此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="f5f09-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="f5f09-108">访问集合</span><span class="sxs-lookup"><span data-stu-id="f5f09-108">Accessing the collection</span></span>
<span data-ttu-id="f5f09-109">可通过以下两种方法来访问 Postman 中的集合：使用集合或参与集合。</span><span class="sxs-lookup"><span data-stu-id="f5f09-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="f5f09-110">必须先在计算机上运行 [Postman](https://www.getpostman.com/)。</span><span class="sxs-lookup"><span data-stu-id="f5f09-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="f5f09-111">使用集合</span><span class="sxs-lookup"><span data-stu-id="f5f09-111">Consume the collection</span></span>
<span data-ttu-id="f5f09-112">使用集合是开始使用 Microsoft Graph API 的最简单方法。</span><span class="sxs-lookup"><span data-stu-id="f5f09-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="f5f09-113">单击 [Postman 共享链接](https://www.getpostman.com/collections/d89a737b5f0c0825898a)将启动 Postman。</span><span class="sxs-lookup"><span data-stu-id="f5f09-113">The [Postman sharing link](https://www.getpostman.com/collections/d89a737b5f0c0825898a) will launch Postman.</span></span>

<span data-ttu-id="f5f09-114">使用共享集合的优点是，无需执行其他任何步骤，就会自动看到新请求。</span><span class="sxs-lookup"><span data-stu-id="f5f09-114">The advantage to using the shared collection is that new requests will automatically show for you without any additional steps.</span></span>

<span data-ttu-id="f5f09-115">有了集合后，就需要创建环境变量：</span><span class="sxs-lookup"><span data-stu-id="f5f09-115">After you have the collection, you'll need to set up the environment variables:</span></span>

1. <span data-ttu-id="f5f09-116">依次选择“文件 | 导入”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-116">Choose **File | Import ...**.</span></span>
2. <span data-ttu-id="f5f09-117">选择“从链接导入”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-117">Select **Import From Link**.</span></span>
3. <span data-ttu-id="f5f09-118">复制并粘贴下面的 URL，再选择“导入”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-118">Copy and paste the following URL and choose **Import**.</span></span>
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_environment.json
    ```

<span data-ttu-id="f5f09-119">现在，应该会在右上角的环境下拉列表中看到“Microsoft Graph 环境”\*\*\*\*（以眼睛图标为标识）。</span><span class="sxs-lookup"><span data-stu-id="f5f09-119">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="f5f09-120">现在需要[创建环境](#using-the-collection)。</span><span class="sxs-lookup"><span data-stu-id="f5f09-120">Now you need to  [set up your environment](#using-the-collection).</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="f5f09-121">参与集合</span><span class="sxs-lookup"><span data-stu-id="f5f09-121">Contribute to the collection</span></span>
<span data-ttu-id="f5f09-122">若要贡献你自己的请求，需要为 [Microsoft Graph Postman 集合](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github 存储库创建分支。</span><span class="sxs-lookup"><span data-stu-id="f5f09-122">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="f5f09-123">若要详细了解如何执行此操作，请观看以下视频。</span><span class="sxs-lookup"><span data-stu-id="f5f09-123">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

<span data-ttu-id="f5f09-124">若要导入 Postman 集合，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="f5f09-124">To import the Postman collections:</span></span>

1. <span data-ttu-id="f5f09-125">下载并注册 [Postman](https://www.getpostman.com/)。</span><span class="sxs-lookup"><span data-stu-id="f5f09-125">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="f5f09-126">依次选择“文件 | 导入”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-126">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="f5f09-127">选择“从链接导入”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-127">Select **Import From Link**.</span></span>
4. <span data-ttu-id="f5f09-128">粘贴以下两个 URL，再选择每个 URL 后面的“导入”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-128">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_environment.json

    ```

<span data-ttu-id="f5f09-129">现在，应该会在“**集合**”窗格中看到“**Microsoft Graph**”集合。</span><span class="sxs-lookup"><span data-stu-id="f5f09-129">You should now see the **Microsoft Graph v1.0** collection on the **Collections** pane.</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="f5f09-130">使用集合</span><span class="sxs-lookup"><span data-stu-id="f5f09-130">Using the collection</span></span>
<span data-ttu-id="f5f09-131">在 Postman 中创建 **Microsoft Graph** 集合和 **Microsoftr Graph 环境**后，请按照以下步骤操作。</span><span class="sxs-lookup"><span data-stu-id="f5f09-131">After you have the **Microsoft Graph v1.0** collection and the **Microsoftr Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="f5f09-132">设置应用程序 API 调用</span><span class="sxs-lookup"><span data-stu-id="f5f09-132">Set up application API calls</span></span>

1. <span data-ttu-id="f5f09-133">选择右上角的下拉列表中的“无环境”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-133">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="f5f09-134">选择“Microsoft Graph 环境”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-134">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="f5f09-135">依次选择右侧的**眼睛**图标和“编辑”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-135">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="f5f09-136">在**当前**（而不是**初始**）变量中，输入你的 Microsoft 标识应用程序：**ClientID**、**ClientSecret** 和 **TenantID**。</span><span class="sxs-lookup"><span data-stu-id="f5f09-136">Enter your Microsoft Identity Application in the **current** (not **initial**) variables: **ClientID**, **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="f5f09-137">若要详细了解如何创建应用程序，以及如何让管理员同意仅限应用的流，请参阅[使用 Postman 执行 Microsoft Graph 调用](https://developer.microsoft.com/zh-CN/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/)博客文章。</span><span class="sxs-lookup"><span data-stu-id="f5f09-137">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/zh-CN/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="f5f09-138">选择“更新”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-138">Select **Update**.</span></span> <span data-ttu-id="f5f09-139">关闭“管理环境”\*\*\*\* 对话框。</span><span class="sxs-lookup"><span data-stu-id="f5f09-139">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="f5f09-140">在左侧的“**MicrosoftGraph | 应用程序**”集合中，选择“**获取仅限应用的访问令牌**”。</span><span class="sxs-lookup"><span data-stu-id="f5f09-140">In the **MicrosoftGraph v1.0 | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="f5f09-141">然后，选择右侧的“发送”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-141">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="f5f09-142">依次展开“应用程序 | 用户”\*\*\*\* 文件夹，再选择“获取用户”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-142">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="f5f09-143">然后，选择“发送”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-143">Then choose **Send**.</span></span>

<span data-ttu-id="f5f09-144">现在，你可以开始使用 Microsoft Graph 集合了。</span><span class="sxs-lookup"><span data-stu-id="f5f09-144">You are now up and running with the Microsoft Graph v1.0 collections.</span></span>

><span data-ttu-id="f5f09-145">**注意：** 若要在集合中运行其他 API，需要同意应用程序拥有必需权限。</span><span class="sxs-lookup"><span data-stu-id="f5f09-145">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="f5f09-146">设置代表 API 调用</span><span class="sxs-lookup"><span data-stu-id="f5f09-146">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="f5f09-147">设置代表 API 调用的最简单方法是，在环境设置中提供 **UserName** 和 **UserPassword**，并使用“代表用户 | 获取用户访问令牌”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-147">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="f5f09-148">**重要提示**：不建议使用生产用户帐户，因为此信息直接存储在 Postman 中。</span><span class="sxs-lookup"><span data-stu-id="f5f09-148">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="f5f09-149">也不建议使用这种方法在生产中获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="f5f09-149">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="f5f09-150">只能用于测试目的。</span><span class="sxs-lookup"><span data-stu-id="f5f09-150">Use it only for testing purposes.</span></span>

<span data-ttu-id="f5f09-151">如果不希望在同步到 Postman 云帐户的环境变量中存储用户名和密码，可使用“获取新访问令牌”\*\*\*\* 功能来获取令牌，而无需离开 Postman。</span><span class="sxs-lookup"><span data-stu-id="f5f09-151">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="f5f09-152">选择“代表用户 | 使用 Postman 获取访问令牌”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-152">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="f5f09-153">选择“授权”\*\*\*\* 选项卡。</span><span class="sxs-lookup"><span data-stu-id="f5f09-153">Choose the **Authorization** tab.</span></span>
3. <span data-ttu-id="f5f09-154">选择“获取新访问令牌”\*\*\*\* 按钮。</span><span class="sxs-lookup"><span data-stu-id="f5f09-154">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="f5f09-155">使用真实的租户和应用程序值填写以下框。</span><span class="sxs-lookup"><span data-stu-id="f5f09-155">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="f5f09-156">请注意，不能在此处使用环境变量；必须使用实际值。</span><span class="sxs-lookup"><span data-stu-id="f5f09-156">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="f5f09-157">若要查找这些值，可以选择 portal.azure.com 上“应用程序”\*\*\*\* 边栏选项卡中的“终结点”。</span><span class="sxs-lookup"><span data-stu-id="f5f09-157">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="f5f09-158">回调 URL：https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="f5f09-158">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="f5f09-159">验证 URL：https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="f5f09-159">Auth URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="f5f09-160">访问令牌 URL：https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="f5f09-160">Access Token URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span></span>
    - <span data-ttu-id="f5f09-161">客户端 ID：**CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="f5f09-161">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="f5f09-162">客户端密码：**CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="f5f09-162">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="f5f09-163">作用域：https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="f5f09-163">Scope: https://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="f5f09-164">状态：**RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="f5f09-164">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="f5f09-165">选择“请求令牌”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="f5f09-165">Choose **Request Token**.</span></span> <span data-ttu-id="f5f09-166">应该会看到 UI 提示，提示你登录和同意权限。</span><span class="sxs-lookup"><span data-stu-id="f5f09-166">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="f5f09-167">复制访问令牌，打开环境变量，并将它粘贴到“UserAccessToken”\*\*\*\* 字段中。</span><span class="sxs-lookup"><span data-stu-id="f5f09-167">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="f5f09-168">现在，所有请求都将可以正常运行。</span><span class="sxs-lookup"><span data-stu-id="f5f09-168">Now all your requests will work.</span></span>
