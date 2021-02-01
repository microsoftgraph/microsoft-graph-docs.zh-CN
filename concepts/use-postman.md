---
title: 结合使用 Postman 和 Microsoft Graph API
description: 使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 34be5bab88acbd7545caa958db0809a010660fb4
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059684"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="2f0f0-103">结合使用 Postman 和 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="2f0f0-103">Use Postman with the Microsoft Graph API</span></span>
<span data-ttu-id="2f0f0-104">使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Postman 图像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="2f0f0-106">本文介绍了如何快速掌握 Postman 和 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="2f0f0-107">此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="2f0f0-108">有关如何操作的详细信息，请跟随此文章中的步骤或观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-108">For details about how to do this, follow the steps in this article or watch the [Getting started with Microsoft Graph Postman workspace](https://youtu.be/3RTHY3jScmA) video.</span></span>


## <a name="step-1---forking-the-microsoft-graph-postman-collection"></a><span data-ttu-id="2f0f0-109">第一步 - 创建 Microsoft Graph Postman 集合分支</span><span class="sxs-lookup"><span data-stu-id="2f0f0-109">Step 1 - Forking the Microsoft Graph Postman collection</span></span>
<span data-ttu-id="2f0f0-110">要使用 Postman 集合，请创建其分支到你的 Postman 工作区。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-110">To use the Postman collection, fork it to your own Postman workspace.</span></span> <span data-ttu-id="2f0f0-111">在 web 浏览器中进行该操作。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-111">Do this from the web browser.</span></span>

1. <span data-ttu-id="2f0f0-112">转到 [Postman](https://www.postman.com/) 并登录。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-112">Go to [Postman](https://www.postman.com/) and sign in.</span></span>
2. <span data-ttu-id="2f0f0-113">转到标签名为 [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork) 的 Postman 集合。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-113">Go to the Postman collection labeled [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork).</span></span>
3. <span data-ttu-id="2f0f0-114">为你的分支填充标签。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-114">Fill in a label for your own fork.</span></span> <span data-ttu-id="2f0f0-115">此值可以是任何文本。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-115">This can be any text.</span></span>
4. <span data-ttu-id="2f0f0-116">在工作区下，请确保在下拉列表中选中 **我的工作区**。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-116">Under Workspace, ensure that **My Workspace** is selected in the drop-down list.</span></span> 
5. <span data-ttu-id="2f0f0-117">单击 **分支集合**。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-117">Click **Fork Collection**.</span></span>

<span data-ttu-id="2f0f0-118">随后会重定向至你的工作区中主要 Microsoft Graph Postman 集合的一个分支。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-118">You will be redirected to a fork of the main Microsoft Graph Postman collection in your own workspace.</span></span>

## <a name="step-2---optional---postman-web-browser-only-download-the-postman-agent"></a><span data-ttu-id="2f0f0-119">第二步 - （可选 - 仅针对 Postman web 浏览器）下载 Postman 代理。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-119">Step 2 - (Optional - Postman Web browser only) Download the Postman Agent</span></span>
<span data-ttu-id="2f0f0-120">要在 web 浏览器中使用此 Postman 集合，请下载 [Postman 桌面代理](https://www.postman.com/downloads)。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-120">To use this particular Postman collection in your web browser, download the [Postman Desktop Agent](https://www.postman.com/downloads).</span></span> <span data-ttu-id="2f0f0-121">由于 web 浏览器的限制，无法在未下载此代理的情况下在 web 上使用 Postman。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-121">You can't use Postman for the web without this due to CORS restrictions in the web browser.</span></span> 

<span data-ttu-id="2f0f0-122">如果你正在使用 Postman for Windows 应用，则不需要此代理。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-122">You don't need the agent if you're using the Postman for Windows app.</span></span> <span data-ttu-id="2f0f0-123">打开 Postman for Windows 后，你会在工作区中看到这个分支集合。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-123">If you open Postman for Windows, you will see this forked collection in your workspace.</span></span>

## <a name="step-3---create-an-azure-ad-application"></a><span data-ttu-id="2f0f0-124">第三步 - 创建 Azure AD 应用程序</span><span class="sxs-lookup"><span data-stu-id="2f0f0-124">Step 3 - Create an Azure AD application</span></span>
<span data-ttu-id="2f0f0-125">要在你的开发者租户中使用此集合，请创建一个 Azure AD 应用程序并根据想要调用的请求给予其合适的权限。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-125">To use this collection in your own developer tenant, create an Azure AD application and give it the appropriate permissions for the requests you want to call.</span></span> <span data-ttu-id="2f0f0-126">如果没有开发者租户，你可以通过 [Microsoft 365 开发人员计划](https://developer.microsoft.com/zh-CN/microsoft-365/dev-program)注册一个。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-126">If you don't have a developer tenant, you can sign up for one through the [Microsoft 365 Developer Program](https://developer.microsoft.com/zh-CN/microsoft-365/dev-program).</span></span>

1. <span data-ttu-id="2f0f0-127">转到 [portal.azure.com](https://portal.azure.com/) 并使用开发者租户管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-127">Go to [portal.azure.com](https://portal.azure.com/) and sign in with your developer tenant administrator account.</span></span>
2. <span data-ttu-id="2f0f0-128">单击 “**Azure Services**” 下的 “**Azure Active Directory**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-128">Under **Azure Services**, click **Azure Active Directory**.</span></span>
3. <span data-ttu-id="2f0f0-129">在左侧菜单中，单击“**应用注册**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-129">On the left menu, click **App registrations**.</span></span>
4. <span data-ttu-id="2f0f0-130">在水平菜单中，单击“**新建注册**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-130">On the horizontal menu, click **New registration**.</span></span>
5. <span data-ttu-id="2f0f0-131">将“**应用名称**”设置为“`Postman`”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-131">Set the **Application name** to `Postman`.</span></span>
6. <span data-ttu-id="2f0f0-132">将“**重定向 URI**”设置为“`https://oauth.pstmn.io/v1/browser-callback`”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-132">Set the **Redirect URI** to `https://oauth.pstmn.io/v1/browser-callback`.</span></span>
7. <span data-ttu-id="2f0f0-133">单击“**注册**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-133">Click **Register**.</span></span>
8. <span data-ttu-id="2f0f0-134">在左侧菜单中，单击 “**API 权限**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-134">On the left menu, click **API Permissions**.</span></span>
9. <span data-ttu-id="2f0f0-135">在水平菜单中，单击“**添加权限**”，选择 “**Microsoft Graph**”，然后选择“**委派权限**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-135">In the horizontal menu, click **Add a permission**, select **Microsoft Graph**, and then select **Delegated Permissions**.</span></span>
10. <span data-ttu-id="2f0f0-136">键入“`Mail.`”，展开“**邮件**”选项，然后检查 **Mail.Read**.</span><span class="sxs-lookup"><span data-stu-id="2f0f0-136">Type `Mail.`, expand the **Mail** options, and check **Mail.Read**.</span></span>
11. <span data-ttu-id="2f0f0-137">单击“**应用权限**”然后键入“`User.`”，随后检查“**应用权限**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-137">Click **Application permissions** and type `User.`, and check **Application Permissions**.</span></span>
12. <span data-ttu-id="2f0f0-138">展开“**用户**”选项并检查 **User.Read.All**。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-138">Expand the **User** options and check **User.Read.All**.</span></span>
13. <span data-ttu-id="2f0f0-139">单击“**添加权限**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-139">Click **Add permissions**.</span></span>
14. <span data-ttu-id="2f0f0-140">在水平菜单中，单击“**授予管理员许可**”，并单击“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-140">In the horizontal menu, click **Grant admin consent for**, and click **Yes**.</span></span>
15. <span data-ttu-id="2f0f0-141">在左侧菜单中，单击“**概述**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-141">In the left menu, click **Overview**.</span></span> <span data-ttu-id="2f0f0-142">你可以从这里获取“**应用程序（客户端）ID**” 和“**目录（客户端）ID**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-142">From here, you can get the **Application (client) ID** and **Directory (tenant) ID**.</span></span> <span data-ttu-id="2f0f0-143">这些会在第四步中用到。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-143">You will need these in step 4.</span></span>
16. <span data-ttu-id="2f0f0-144">单击左侧菜单中的“**证书和机密**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-144">In the left menu, click **Certificates & secrets**.</span></span> 
17. <span data-ttu-id="2f0f0-145">单击“**新建客户端机密**”，并输入简短说明，然后单击“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-145">Click **New client secret**, enter a description, and click **Add**.</span></span> <span data-ttu-id="2f0f0-146">将鼠标光标悬浮在新的客户端机密 **值** 上并复制。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-146">Hover over the new client secret **Value** and copy it.</span></span> <span data-ttu-id="2f0f0-147">第四步中会用到它。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-147">You will need this in step 4.</span></span>

<span data-ttu-id="2f0f0-148">Azure AD 应用程序现已具有代表用户提出调用 Mail.Read 请求的权限并成为 User.Read.All 的一个应用。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-148">The Azure AD application now has permissions to make requests on behalf of a user to call Mail.Read and as an application for User.Read.All.</span></span>

## <a name="step-4---configuring-authentication"></a><span data-ttu-id="2f0f0-149">第四步 - 配置身份验证</span><span class="sxs-lookup"><span data-stu-id="2f0f0-149">Step 4 - Configuring authentication</span></span>
<span data-ttu-id="2f0f0-150">设置一些环境变量来检索访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-150">Set up some environment variables used to retrieve an access token.</span></span>

1. <span data-ttu-id="2f0f0-151">单击右上角“**无环境**”下拉菜单旁边的眼睛图标。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-151">Click the eye icon in the top right next to the **No environment** drop down.</span></span>
2. <span data-ttu-id="2f0f0-152">单击弹出窗口右上角的“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-152">Click **Add** in the top right of that pop up.</span></span>
3. <span data-ttu-id="2f0f0-153">将“**新环境**”更改为“**M365 环境**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-153">Change **New Environment** to **M365 Environment**.</span></span>
4. <span data-ttu-id="2f0f0-154">创建名为`ClientID`的变量并将“**当前值**”设置为步骤 3.15 中的应用程序（客户端）ID 值。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-154">Create a new variable called `ClientID` and set the **Current value** to the Application (client) ID value from step 3.15.</span></span>
5. <span data-ttu-id="2f0f0-155">创建名为`ClientSecret`的变量并将“**当前值**”设置为步骤 3.17 中的客户端机密值。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-155">Create a new variable called `ClientSecret` and  set the **Current value** to the Client Secret value from step 3.17.</span></span>
6. <span data-ttu-id="2f0f0-156">创建名为`TenantID`的变量并将“**当前值**”设置为步骤 3.15 中的目录（租户）ID 值。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-156">Create a new variable called `TenantID` and set the **Current value** to the Directory (tenant) ID value from step 3.15.</span></span>
7. <span data-ttu-id="2f0f0-157">选择“**保存**”/“**更新**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-157">Select **Save**/**Update**.</span></span> 
8. <span data-ttu-id="2f0f0-158">关闭“**管理环境**”对话框。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-158">Close the **Manage Environments** dialog box.</span></span> 
9. <span data-ttu-id="2f0f0-159">仔细检查是否在下拉菜单中选中了 “**M365 环境**” 而不是 “**无环境**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-159">Double check that **M365 Environment** is selected in the drop down and not **No environment**.</span></span>

## <a name="step-5---get-a-delegated-access-token"></a><span data-ttu-id="2f0f0-160">第五步 - 获取委派的访问令牌</span><span class="sxs-lookup"><span data-stu-id="2f0f0-160">Step 5 - Get a delegated access token</span></span>
<span data-ttu-id="2f0f0-161">由于这是你第一次通过委派身份验证流程运行请求，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-161">Because this is the first time you are running a request as a delegated authentication flow, you need to get an access token.</span></span>

1. <span data-ttu-id="2f0f0-162">将鼠标光标悬浮在“**代表用户**”文件夹上，单击省略号，然后选择“**编辑**”</span><span class="sxs-lookup"><span data-stu-id="2f0f0-162">Hover over the **On behalf of a User** folder, click the ellipsis, and select **Edit**</span></span>
2. <span data-ttu-id="2f0f0-163">单击“**授权**”选项卡。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-163">Click the **Authorization** tab.</span></span>
3. <span data-ttu-id="2f0f0-164">在右侧下滑并单击“**获取新的访问令牌**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-164">Scroll down on the right and click **Get New Access Token**.</span></span>
4. <span data-ttu-id="2f0f0-165">登录你的开发者租户管理员账户。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-165">Sign in with your developer tenant adminstrator account.</span></span>
5. <span data-ttu-id="2f0f0-166">单击“**继续**”，然后单击“**使用令牌**”按钮。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-166">Click **Proceed**, and then click the **Use Token** button.</span></span>
6. <span data-ttu-id="2f0f0-167">在该对话框的右下角，单击“**更新**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-167">On the botton right of the dialog, click **Update**.</span></span>

<span data-ttu-id="2f0f0-168">你现在已具有用于委派请求的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-168">You now have a valid access token to use for delegated requests.</span></span>

## <a name="step-6---run-your-first-delegated-request"></a><span data-ttu-id="2f0f0-169">第六步 - 运行你的第一个委派请求</span><span class="sxs-lookup"><span data-stu-id="2f0f0-169">Step 6 - Run your first delegated request</span></span>
<span data-ttu-id="2f0f0-170">“**代表用户**”文件夹中是你可以调用的各种 Microsoft Graph 工作负载请求。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-170">Inside the **On Behalf of a User** folder are requests for various Microsoft Graph workloads you can call.</span></span>

1. <span data-ttu-id="2f0f0-171">展开 “**代表用户**”文件夹，然后展开“**邮件**”文件夹。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-171">Expand the **On behalf of a User** folder and then expand the **Mail** folder.</span></span>
2. <span data-ttu-id="2f0f0-172">双击“**获取我的邮件**”来打开请求。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-172">Double-click **Get my messages** to open the request.</span></span>
3. <span data-ttu-id="2f0f0-173">在右上角，单击“**发送**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-173">On the top right, click **Send**.</span></span>

<span data-ttu-id="2f0f0-174">你已经成功地使用委派身份验证完成了一次 Microsoft Graph 调用。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-174">You have now successfully made a Microsoft Graph call using delegated authentication.</span></span>

## <a name="step-7---get-an-application-access-token"></a><span data-ttu-id="2f0f0-175">第七步 - 获取应用程序访问令牌</span><span class="sxs-lookup"><span data-stu-id="2f0f0-175">Step 7 - Get an application access token</span></span>
<span data-ttu-id="2f0f0-176">由于这是你第一次通过应用程序身份验证流程运行请求，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-176">Because this is the first time you are running a request as a application authentication flow, you need to get an access token.</span></span>

1. <span data-ttu-id="2f0f0-177">将鼠标光标悬浮在“**应用程序**”文件夹上，单击省略号，然后选择“**编辑**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-177">Hover over the **Application** folder, click the ellipsis, and select **Edit**.</span></span>
2. <span data-ttu-id="2f0f0-178">单击“**授权**”选项卡。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-178">Click the **Authorization** tab</span></span>
3. <span data-ttu-id="2f0f0-179">在右侧下滑并单击“**获取新的访问令牌**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-179">Scroll down on the right side and click **Get New Access Token**.</span></span>
5. <span data-ttu-id="2f0f0-180">单击“**继续**”，然后单击“**使用令牌**”按钮。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-180">Click **Proceed**, and then click the **Use Token** button.</span></span>
6. <span data-ttu-id="2f0f0-181">在该对话框的右下角，单击“**更新**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-181">On the bottom right of the dialog, click **Update**.</span></span>

<span data-ttu-id="2f0f0-182">你现在已具有用于委派请求的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-182">You now have a valid access token to use for application requests.</span></span>

## <a name="step-8---run-your-first-application-request"></a><span data-ttu-id="2f0f0-183">第八步 - 运行你的第一个应用程序请求</span><span class="sxs-lookup"><span data-stu-id="2f0f0-183">Step 8 - Run your first application request</span></span>
<span data-ttu-id="2f0f0-184">“**应用程序**”文件夹中是你可以调用的各种 Microsoft Graph 工作负载请求。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-184">Inside the **Application** folder are requests for various Microsoft Graph workloads you can call.</span></span>

1. <span data-ttu-id="2f0f0-185">展开“**应用程序**”文件夹，然后展开“**用户**”文件夹。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-185">Expand the **Application** folder and then expand the **User** folder.</span></span>
2. <span data-ttu-id="2f0f0-186">双击“**获取用户**”来打开请求。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-186">Double-click **Get Users** to open the request.</span></span>
3. <span data-ttu-id="2f0f0-187">在右上角，单击“**发送**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-187">On the top right, click **Send**.</span></span>

<span data-ttu-id="2f0f0-188">你已经成功地使用应用程序身份验证完成了一次 Microsoft Graph 调用。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-188">You have now successfully made a Microsoft Graph call using application authentication.</span></span>

<span data-ttu-id="2f0f0-189">你可以按照这些步骤向 Microsoft Graph 发出其他请求。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-189">You can follow these steps to make other requests to Microsoft Graph.</span></span> <span data-ttu-id="2f0f0-190">请记住，你需要向你的 Azure AD 应用程序添加权限来使其他请求正常运行；否则，你将在响应中收到权限被拒的错误。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-190">Remember that you have to add permissions to your Azure AD application for other requests to work; Otherwise, you will get permission denied errors in your responses.</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="2f0f0-191">参与集合</span><span class="sxs-lookup"><span data-stu-id="2f0f0-191">Contribute to the collection</span></span>
<span data-ttu-id="2f0f0-192">若要贡献你自己的请求，需要 Postman 许可。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-192">If you want to contribute your own requests, you will need a Postman license.</span></span> <span data-ttu-id="2f0f0-193">你可以对分支集合做出更改，然后将鼠标光标悬浮在集合的顶端节点，然后选择“**创建拉取请求**”。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-193">You can make your changes to the forked collection, and then hover over the collection top node and select **Create pull request**.</span></span>

## <a name="see-also"></a><span data-ttu-id="2f0f0-194">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2f0f0-194">See also</span></span>

<span data-ttu-id="2f0f0-195">有关如何操作的详细信息，请观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。</span><span class="sxs-lookup"><span data-stu-id="2f0f0-195">For details about how to do this, watch the [Getting started with Microsoft Graph Postman workspace](https://youtu.be/3RTHY3jScmA) video.</span></span>


