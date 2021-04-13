---
title: 结合使用 Postman 和 Microsoft Graph API
description: 使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 41c6768097a2c0b001b5b9b7c691b0488bed018a
ms.sourcegitcommit: e96b98849cfc3aa915df63696a0b9f30c0a52cfd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2021
ms.locfileid: "51654105"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="15f67-103">结合使用 Postman 和 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="15f67-103">Use Postman with the Microsoft Graph API</span></span>
<span data-ttu-id="15f67-104">使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="15f67-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Postman 图像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="15f67-106">本文介绍了如何快速掌握 Postman 和 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="15f67-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="15f67-107">此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="15f67-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="15f67-108">有关如何操作的详细信息，请跟随此文章中的步骤或观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。</span><span class="sxs-lookup"><span data-stu-id="15f67-108">For details about how to do this, follow the steps in this article or watch the [Getting started with Microsoft Graph Postman workspace](https://youtu.be/3RTHY3jScmA) video.</span></span>


## <a name="step-1---forking-the-microsoft-graph-postman-collection"></a><span data-ttu-id="15f67-109">第一步 - 创建 Microsoft Graph Postman 集合分支</span><span class="sxs-lookup"><span data-stu-id="15f67-109">Step 1 - Forking the Microsoft Graph Postman collection</span></span>
<span data-ttu-id="15f67-110">要使用 Postman 集合，请创建其分支到你的 Postman 工作区。</span><span class="sxs-lookup"><span data-stu-id="15f67-110">To use the Postman collection, fork it to your own Postman workspace.</span></span> <span data-ttu-id="15f67-111">在 web 浏览器中进行该操作。</span><span class="sxs-lookup"><span data-stu-id="15f67-111">Do this from the web browser.</span></span>

1. <span data-ttu-id="15f67-112">转到 [Postman](https://www.postman.com/) 并登录。</span><span class="sxs-lookup"><span data-stu-id="15f67-112">Go to [Postman](https://www.postman.com/) and sign in.</span></span>
2. <span data-ttu-id="15f67-113">转到标签名为 [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork) 的 Postman 集合。</span><span class="sxs-lookup"><span data-stu-id="15f67-113">Go to the Postman collection labeled [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork).</span></span>
3. <span data-ttu-id="15f67-114">为你的分支填充标签。</span><span class="sxs-lookup"><span data-stu-id="15f67-114">Fill in a label for your own fork.</span></span> <span data-ttu-id="15f67-115">此值可以是任何文本。</span><span class="sxs-lookup"><span data-stu-id="15f67-115">This can be any text.</span></span>
4. <span data-ttu-id="15f67-116">在工作区下，请确保在下拉列表中选中 **我的工作区**。</span><span class="sxs-lookup"><span data-stu-id="15f67-116">Under Workspace, ensure that **My Workspace** is selected in the drop-down list.</span></span> 
5. <span data-ttu-id="15f67-117">单击 **分支集合**。</span><span class="sxs-lookup"><span data-stu-id="15f67-117">Click **Fork Collection**.</span></span>

<span data-ttu-id="15f67-118">随后会重定向至你的工作区中主要 Microsoft Graph Postman 集合的一个分支。</span><span class="sxs-lookup"><span data-stu-id="15f67-118">You will be redirected to a fork of the main Microsoft Graph Postman collection in your own workspace.</span></span>

## <a name="step-2---optional---postman-web-browser-only-download-the-postman-agent"></a><span data-ttu-id="15f67-119">第二步 - （可选 - 仅针对 Postman web 浏览器）下载 Postman 代理。</span><span class="sxs-lookup"><span data-stu-id="15f67-119">Step 2 - (Optional - Postman Web browser only) Download the Postman Agent</span></span>
<span data-ttu-id="15f67-120">要在 web 浏览器中使用此 Postman 集合，请下载 [Postman 桌面代理](https://www.postman.com/downloads)。</span><span class="sxs-lookup"><span data-stu-id="15f67-120">To use this particular Postman collection in your web browser, download the [Postman Desktop Agent](https://www.postman.com/downloads).</span></span> <span data-ttu-id="15f67-121">由于 web 浏览器的限制，无法在未下载此代理的情况下在 web 上使用 Postman。</span><span class="sxs-lookup"><span data-stu-id="15f67-121">You can't use Postman for the web without this due to CORS restrictions in the web browser.</span></span> 

<span data-ttu-id="15f67-122">如果你正在使用 Postman for Windows 应用，则不需要此代理。</span><span class="sxs-lookup"><span data-stu-id="15f67-122">You don't need the agent if you're using the Postman for Windows app.</span></span> <span data-ttu-id="15f67-123">打开 Postman for Windows 后，你会在工作区中看到这个分支集合。</span><span class="sxs-lookup"><span data-stu-id="15f67-123">If you open Postman for Windows, you will see this forked collection in your workspace.</span></span>

## <a name="step-3---create-an-azure-ad-application"></a><span data-ttu-id="15f67-124">第三步 - 创建 Azure AD 应用程序</span><span class="sxs-lookup"><span data-stu-id="15f67-124">Step 3 - Create an Azure AD application</span></span>
<span data-ttu-id="15f67-125">要在你的开发者租户中使用此集合，请创建一个 Azure AD 应用程序并根据想要调用的请求给予其合适的权限。</span><span class="sxs-lookup"><span data-stu-id="15f67-125">To use this collection in your own developer tenant, create an Azure AD application and give it the appropriate permissions for the requests you want to call.</span></span> <span data-ttu-id="15f67-126">如果没有开发者租户，你可以通过 [Microsoft 365 开发人员计划](https://developer.microsoft.com/zh-CN/microsoft-365/dev-program)注册一个。</span><span class="sxs-lookup"><span data-stu-id="15f67-126">If you don't have a developer tenant, you can sign up for one through the [Microsoft 365 Developer Program](https://developer.microsoft.com/zh-CN/microsoft-365/dev-program).</span></span>

1. <span data-ttu-id="15f67-127">转到 [portal.azure.com](https://portal.azure.com/) 并使用开发者租户管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="15f67-127">Go to [portal.azure.com](https://portal.azure.com/) and sign in with your developer tenant administrator account.</span></span>
2. <span data-ttu-id="15f67-128">单击 “**Azure Services**” 下的 “**Azure Active Directory**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-128">Under **Azure Services**, click **Azure Active Directory**.</span></span>
3. <span data-ttu-id="15f67-129">在左侧菜单中，单击“**应用注册**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-129">On the left menu, click **App registrations**.</span></span>
4. <span data-ttu-id="15f67-130">在水平菜单中，单击“**新建注册**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-130">On the horizontal menu, click **New registration**.</span></span>
5. <span data-ttu-id="15f67-131">将“**应用名称**”设置为“`Postman`”。</span><span class="sxs-lookup"><span data-stu-id="15f67-131">Set the **Application name** to `Postman`.</span></span>
6. <span data-ttu-id="15f67-132">将“**重定向 URI**”设置为“`https://oauth.pstmn.io/v1/browser-callback`”。</span><span class="sxs-lookup"><span data-stu-id="15f67-132">Set the **Redirect URI** to `https://oauth.pstmn.io/v1/browser-callback`.</span></span>
7. <span data-ttu-id="15f67-133">单击“**注册**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-133">Click **Register**.</span></span>
8. <span data-ttu-id="15f67-134">在左侧菜单中，单击 “**API 权限**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-134">On the left menu, click **API Permissions**.</span></span>
9. <span data-ttu-id="15f67-135">在水平菜单中，单击“**添加权限**”，选择 “**Microsoft Graph**”，然后选择“**委派权限**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-135">In the horizontal menu, click **Add a permission**, select **Microsoft Graph**, and then select **Delegated Permissions**.</span></span>
10. <span data-ttu-id="15f67-136">键入“`Mail.`”，展开“**邮件**”选项，然后检查 **Mail.Read**.</span><span class="sxs-lookup"><span data-stu-id="15f67-136">Type `Mail.`, expand the **Mail** options, and check **Mail.Read**.</span></span>
11. <span data-ttu-id="15f67-137">单击“**应用权限**”然后键入“`User.`”，随后检查“**应用权限**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-137">Click **Application permissions** and type `User.`, and check **Application Permissions**.</span></span>
12. <span data-ttu-id="15f67-138">展开“**用户**”选项并检查 **User.Read.All**。</span><span class="sxs-lookup"><span data-stu-id="15f67-138">Expand the **User** options and check **User.Read.All**.</span></span>
13. <span data-ttu-id="15f67-139">单击“**添加权限**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-139">Click **Add permissions**.</span></span>
14. <span data-ttu-id="15f67-140">在水平菜单中，单击“**授予管理员许可**”，并单击“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-140">In the horizontal menu, click **Grant admin consent for**, and click **Yes**.</span></span>
15. <span data-ttu-id="15f67-141">在左侧菜单中，单击“**概述**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-141">In the left menu, click **Overview**.</span></span> <span data-ttu-id="15f67-142">你可以从这里获取“**应用程序（客户端）ID**” 和“**目录（客户端）ID**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-142">From here, you can get the **Application (client) ID** and **Directory (tenant) ID**.</span></span> <span data-ttu-id="15f67-143">这些会在第四步中用到。</span><span class="sxs-lookup"><span data-stu-id="15f67-143">You will need these in step 4.</span></span>
16. <span data-ttu-id="15f67-144">单击左侧菜单中的“**证书和机密**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-144">In the left menu, click **Certificates & secrets**.</span></span> 
17. <span data-ttu-id="15f67-145">单击“**新建客户端机密**”，并输入简短说明，然后单击“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-145">Click **New client secret**, enter a description, and click **Add**.</span></span> <span data-ttu-id="15f67-146">将鼠标光标悬浮在新的客户端机密 **值** 上并复制。</span><span class="sxs-lookup"><span data-stu-id="15f67-146">Hover over the new client secret **Value** and copy it.</span></span> <span data-ttu-id="15f67-147">第四步中会用到它。</span><span class="sxs-lookup"><span data-stu-id="15f67-147">You will need this in step 4.</span></span>

<span data-ttu-id="15f67-148">Azure AD 应用程序现已具有代表用户提出调用 Mail.Read 请求的权限并成为 User.Read.All 的一个应用。</span><span class="sxs-lookup"><span data-stu-id="15f67-148">The Azure AD application now has permissions to make requests on behalf of a user to call Mail.Read and as an application for User.Read.All.</span></span>

## <a name="step-4---configuring-authentication-in-postman"></a><span data-ttu-id="15f67-149">步骤 4 - 在 Postman 中配置身份验证</span><span class="sxs-lookup"><span data-stu-id="15f67-149">Step 4 - Configuring authentication in Postman</span></span>
<span data-ttu-id="15f67-150">在此步骤中，将设置用于检索访问令牌的环境变量。</span><span class="sxs-lookup"><span data-stu-id="15f67-150">In this step, you set up the environment variables used to retrieve an access token.</span></span>

1. <span data-ttu-id="15f67-151">转到 [分叉](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/environment/455214-efbc69b2-69bd-402e-9e72-850b3a49bb21/fork)。</span><span class="sxs-lookup"><span data-stu-id="15f67-151">Go to [Fork environment](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/environment/455214-efbc69b2-69bd-402e-9e72-850b3a49bb21/fork).</span></span>
2. <span data-ttu-id="15f67-152">添加标签分叉。</span><span class="sxs-lookup"><span data-stu-id="15f67-152">Add a label for fork.</span></span> <span data-ttu-id="15f67-153">此值可以是任何文本。</span><span class="sxs-lookup"><span data-stu-id="15f67-153">This can be any text.</span></span>
3. <span data-ttu-id="15f67-154">在工作区下，请确保在下拉列表中选中 **我的工作区**。</span><span class="sxs-lookup"><span data-stu-id="15f67-154">Under Workspace, ensure that **My Workspace** is selected in the drop-down list.</span></span> 
4. <span data-ttu-id="15f67-155">单击 **分叉环境**。</span><span class="sxs-lookup"><span data-stu-id="15f67-155">Click **Fork Environment**.</span></span>
5. <span data-ttu-id="15f67-156">在 `ClientID`中， **步骤 3.15** 应用程序（客户端）ID 值设置当前值。</span><span class="sxs-lookup"><span data-stu-id="15f67-156">In `ClientID`, set the **Current value** to the application (client) ID value from step 3.15.</span></span>
6. <span data-ttu-id="15f67-157">在 `ClientSecret`中， **3.17** 客户端密码值设置当前值。</span><span class="sxs-lookup"><span data-stu-id="15f67-157">In `ClientSecret`, set the **Current value** to the client secret value from step 3.17.</span></span>
6. <span data-ttu-id="15f67-158">在 `TenantID`中， **3.15** 目录（租户）ID 值设置当前值。</span><span class="sxs-lookup"><span data-stu-id="15f67-158">In `TenantID`, set the **Current value** to the directory (tenant) ID value from step 3.15.</span></span>
7. <span data-ttu-id="15f67-159">在右上方，单击 **保存**。</span><span class="sxs-lookup"><span data-stu-id="15f67-159">On the top right, click **Save**.</span></span> 
8. <span data-ttu-id="15f67-160">关闭" **"选项卡** "。</span><span class="sxs-lookup"><span data-stu-id="15f67-160">Close the **Manage Environments** tab.</span></span> 
9. <span data-ttu-id="15f67-161">在右上方眼睛图标旁边，验证是否选择了 **"M365 环境** "，而不是" **没有**。</span><span class="sxs-lookup"><span data-stu-id="15f67-161">On the top right, next to the eye icon, verify that **M365 Environment** is selected in the drop down and not **No environment**.</span></span>

## <a name="step-5---get-a-delegated-access-token"></a><span data-ttu-id="15f67-162">第五步 - 获取委派的访问令牌</span><span class="sxs-lookup"><span data-stu-id="15f67-162">Step 5 - Get a delegated access token</span></span>
<span data-ttu-id="15f67-163">由于这是你第一次通过委派身份验证流程运行请求，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="15f67-163">Because this is the first time you are running a request as a delegated authentication flow, you need to get an access token.</span></span>

1. <span data-ttu-id="15f67-164">将鼠标光标悬浮在“**委派**”文件夹上，单击省略号，然后选择“**编辑**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-164">Hover over the **Delegated** folder, click the ellipsis, and select **Edit**</span></span>
2. <span data-ttu-id="15f67-165">单击“**授权**”选项卡。</span><span class="sxs-lookup"><span data-stu-id="15f67-165">Click the **Authorization** tab.</span></span>
3. <span data-ttu-id="15f67-166">在右侧下滑并单击“**获取新的访问令牌**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-166">Scroll down on the right and click **Get New Access Token**.</span></span>
4. <span data-ttu-id="15f67-167">登录你的开发者租户管理员账户。</span><span class="sxs-lookup"><span data-stu-id="15f67-167">Sign in with your developer tenant adminstrator account.</span></span>
5. <span data-ttu-id="15f67-168">单击“**继续**”，然后单击“**使用令牌**”按钮。</span><span class="sxs-lookup"><span data-stu-id="15f67-168">Click **Proceed**, and then click the **Use Token** button.</span></span>
6. <span data-ttu-id="15f67-169">在该对话框的右下角，单击“**更新**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-169">On the botton right of the dialog, click **Update**.</span></span>

<span data-ttu-id="15f67-170">你现在已具有用于委派请求的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="15f67-170">You now have a valid access token to use for delegated requests.</span></span>

## <a name="step-6---run-your-first-delegated-request"></a><span data-ttu-id="15f67-171">第六步 - 运行你的第一个委派请求</span><span class="sxs-lookup"><span data-stu-id="15f67-171">Step 6 - Run your first delegated request</span></span>
<span data-ttu-id="15f67-172">在 **"委派** 文件夹内是各种您可以呼叫的 Microsoft Graph 工作负载的请求。</span><span class="sxs-lookup"><span data-stu-id="15f67-172">Inside the **Delegated** folder are requests for various Microsoft Graph workloads you can call.</span></span>

1. <span data-ttu-id="15f67-173">展开 **的** 文件夹，然后展开 **邮件** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="15f67-173">Expand the **Delegated** folder and then expand the **Mail** folder.</span></span>
2. <span data-ttu-id="15f67-174">双击“**获取我的邮件**”来打开请求。</span><span class="sxs-lookup"><span data-stu-id="15f67-174">Double-click **Get my messages** to open the request.</span></span>
3. <span data-ttu-id="15f67-175">在右上角，单击“**发送**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-175">On the top right, click **Send**.</span></span>

<span data-ttu-id="15f67-176">你已经成功地使用委派身份验证完成了一次 Microsoft Graph 调用。</span><span class="sxs-lookup"><span data-stu-id="15f67-176">You have now successfully made a Microsoft Graph call using delegated authentication.</span></span>

## <a name="step-7---get-an-application-access-token"></a><span data-ttu-id="15f67-177">第七步 - 获取应用程序访问令牌</span><span class="sxs-lookup"><span data-stu-id="15f67-177">Step 7 - Get an application access token</span></span>
<span data-ttu-id="15f67-178">由于这是你第一次通过应用程序身份验证流程运行请求，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="15f67-178">Because this is the first time you are running a request as a application authentication flow, you need to get an access token.</span></span>

1. <span data-ttu-id="15f67-179">将鼠标光标悬浮在“**应用程序**”文件夹上，单击省略号，然后选择“**编辑**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-179">Hover over the **Application** folder, click the ellipsis, and select **Edit**.</span></span>
2. <span data-ttu-id="15f67-180">单击“**授权**”选项卡。</span><span class="sxs-lookup"><span data-stu-id="15f67-180">Click the **Authorization** tab</span></span>
3. <span data-ttu-id="15f67-181">在右侧下滑并单击“**获取新的访问令牌**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-181">Scroll down on the right side and click **Get New Access Token**.</span></span>
5. <span data-ttu-id="15f67-182">单击“**继续**”，然后单击“**使用令牌**”按钮。</span><span class="sxs-lookup"><span data-stu-id="15f67-182">Click **Proceed**, and then click the **Use Token** button.</span></span>
6. <span data-ttu-id="15f67-183">在该对话框的右下角，单击“**更新**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-183">On the bottom right of the dialog, click **Update**.</span></span>

<span data-ttu-id="15f67-184">你现在已具有用于委派请求的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="15f67-184">You now have a valid access token to use for application requests.</span></span>

## <a name="step-8---run-your-first-application-request"></a><span data-ttu-id="15f67-185">第八步 - 运行你的第一个应用程序请求</span><span class="sxs-lookup"><span data-stu-id="15f67-185">Step 8 - Run your first application request</span></span>
<span data-ttu-id="15f67-186">“**应用程序**”文件夹中是你可以调用的各种 Microsoft Graph 工作负载请求。</span><span class="sxs-lookup"><span data-stu-id="15f67-186">Inside the **Application** folder are requests for various Microsoft Graph workloads you can call.</span></span>

1. <span data-ttu-id="15f67-187">展开“**应用程序**”文件夹，然后展开“**用户**”文件夹。</span><span class="sxs-lookup"><span data-stu-id="15f67-187">Expand the **Application** folder and then expand the **User** folder.</span></span>
2. <span data-ttu-id="15f67-188">双击“**获取用户**”来打开请求。</span><span class="sxs-lookup"><span data-stu-id="15f67-188">Double-click **Get Users** to open the request.</span></span>
3. <span data-ttu-id="15f67-189">在右上角，单击“**发送**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-189">On the top right, click **Send**.</span></span>

<span data-ttu-id="15f67-190">你已经成功地使用应用程序身份验证完成了一次 Microsoft Graph 调用。</span><span class="sxs-lookup"><span data-stu-id="15f67-190">You have now successfully made a Microsoft Graph call using application authentication.</span></span>

<span data-ttu-id="15f67-191">你可以按照这些步骤向 Microsoft Graph 发出其他请求。</span><span class="sxs-lookup"><span data-stu-id="15f67-191">You can follow these steps to make other requests to Microsoft Graph.</span></span> <span data-ttu-id="15f67-192">请记住，你需要向你的 Azure AD 应用程序添加权限来使其他请求正常运行；否则，你将在响应中收到权限被拒的错误。</span><span class="sxs-lookup"><span data-stu-id="15f67-192">Remember that you have to add permissions to your Azure AD application for other requests to work; Otherwise, you will get permission denied errors in your responses.</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="15f67-193">参与集合</span><span class="sxs-lookup"><span data-stu-id="15f67-193">Contribute to the collection</span></span>
<span data-ttu-id="15f67-194">若要贡献你自己的请求，需要 Postman 许可。</span><span class="sxs-lookup"><span data-stu-id="15f67-194">If you want to contribute your own requests, you will need a Postman license.</span></span> <span data-ttu-id="15f67-195">你可以对分支集合做出更改，然后将鼠标光标悬浮在集合的顶端节点，然后选择“**创建拉取请求**”。</span><span class="sxs-lookup"><span data-stu-id="15f67-195">You can make your changes to the forked collection, and then hover over the collection top node and select **Create pull request**.</span></span>

## <a name="see-also"></a><span data-ttu-id="15f67-196">另请参阅</span><span class="sxs-lookup"><span data-stu-id="15f67-196">See also</span></span>

<span data-ttu-id="15f67-197">有关如何操作的详细信息，请观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。</span><span class="sxs-lookup"><span data-stu-id="15f67-197">For details about how to do this, watch the [Getting started with Microsoft Graph Postman collection](https://youtu.be/3RTHY3jScmA) video.</span></span>


