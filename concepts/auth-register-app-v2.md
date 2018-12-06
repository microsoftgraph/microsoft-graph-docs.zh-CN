---
title: 使用 Azure AD v2.0 终结点注册应用
description: '应用必须使用 Azure AD 注册。注册应用会建立一个唯一的应用程序 ID 和其他值，你的应用可使用这些值通过 Azure AD 进行身份验证并获取令牌。对于 Azure AD v2.0 终结点，请使用 Microsoft 应用程序注册门户注册应用。你可以使用 Microsoft 帐户或工作或学校帐户注册应用。为应用配置身份验证或授权时，你需要根据开发的应用类型复制一个或多个要在注册期间使用的属性。 '
ms.openlocfilehash: 552ae1c98a401589345f3dc78fbe40dc7cd70ca9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091779"
---
# <a name="register-your-app-with-the-azure-ad-v20-endpoint"></a><span data-ttu-id="b48cb-107">使用 Azure AD v2.0 终结点注册应用</span><span class="sxs-lookup"><span data-stu-id="b48cb-107">Register your app with the Azure AD v2.0 endpoint</span></span>

<span data-ttu-id="b48cb-p102">应用必须使用 Azure AD 注册。注册应用会建立一个唯一的应用程序 ID 和其他值，你的应用可使用这些值通过 Azure AD 进行身份验证并获取令牌。对于 Azure AD v2.0 终结点，请使用 [Microsoft 应用程序注册门户](https://apps.dev.microsoft.com)注册应用。你可以使用 Microsoft 帐户或工作或学校帐户注册应用。为应用配置身份验证或授权时，你需要根据开发的应用类型复制一个或多个要在注册期间使用的属性。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p102">Your app must be registered with Azure AD. Registering your app establishes a unique application ID and other values that your app uses to authenticate with Azure AD and get tokens. For the Azure AD v2.0 endpoint, you register your app with the [Microsoft App Registration Portal](https://apps.dev.microsoft.com). You can use either a Microsoft account or a work or school account to register your app. Depending on the type of app you are developing, you will need to copy one or more properties during registration to use when you configure authentication and authorization for your app.</span></span> 


> <span data-ttu-id="b48cb-p103">**注意：** 本文主要介绍了使用 Azure AD v2.0 终结点注册应用的内容。有关使用 Azure AD 终结点注册应用的信息，请参阅下面的 [Azure AD 终结点注意事项](#azure-ad-endpoint-considerations)。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p103">**Note:** This article primarily covers registering apps with the Azure AD v2.0 endpoint. For information about registering your app with the Azure AD endpoint, see [Azure AD endpoint considerations](#azure-ad-endpoint-considerations) below.</span></span>
> 
> <span data-ttu-id="b48cb-115">此外，还请注意，如果之前已在 Microsoft Azure 门户中注册过应用，应用注册门户中不会列出这些应用。</span><span class="sxs-lookup"><span data-stu-id="b48cb-115">Also, be aware that if you've previously registered apps in the Microsoft Azure portal, those apps will not be listed in the App Registration Portal.</span></span> <span data-ttu-id="b48cb-116">在 Azure 门户中管理这些应用。</span><span class="sxs-lookup"><span data-stu-id="b48cb-116">Manage those apps in the Azure portal.</span></span> 


<span data-ttu-id="b48cb-p105">下面的屏幕截图显示了已使用密码和隐式流配置的 Web 应用注册示例。![使用密码和隐式授予进行 Web 应用注册。](./images/v2-web-registration.png)</span><span class="sxs-lookup"><span data-stu-id="b48cb-p105">The following screenshot shows an example web app registration that has been configured with a password and implicit flow. ![Web app registration with password and implicit grant.](./images/v2-web-registration.png)</span></span>

<span data-ttu-id="b48cb-119">若要注册应用，请遵循以下步骤；配置应用的授权时，务必复制要使用的指示值：</span><span class="sxs-lookup"><span data-stu-id="b48cb-119">To register your app, follow these steps; be sure to copy the indicated values to use when configuring authorization for your app:</span></span>

1. <span data-ttu-id="b48cb-120">登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="b48cb-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/).</span></span>
   
    <span data-ttu-id="b48cb-121">你可以使用 Microsoft 帐户或工作或学校帐户登录。</span><span class="sxs-lookup"><span data-stu-id="b48cb-121">You can sign in with either a Microsoft account or a work or school account.</span></span> 

2. <span data-ttu-id="b48cb-122">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="b48cb-122">Choose **Add an app**.</span></span>
    > <span data-ttu-id="b48cb-123">注意：如果使用工作或学校帐户登录，请选择**聚合应用程序**的“添加应用程序”\*\*\*\* 按钮。</span><span class="sxs-lookup"><span data-stu-id="b48cb-123">Note: If you signed in with a work or school account, select the **Add an app** button for **Converged applications**.</span></span> 

3. <span data-ttu-id="b48cb-124">输入应用的名称，并选择“创建应用程序”\*\*\*\*”。</span><span class="sxs-lookup"><span data-stu-id="b48cb-124">Enter a name for the app and choose **Create application**.</span></span>

    <span data-ttu-id="b48cb-125">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="b48cb-125">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="b48cb-p106">复制应用程序 ID。这是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p106">Copy the application ID. This is the unique identifier for your app.</span></span>

    <span data-ttu-id="b48cb-128">你将使用该应用程序 ID 配置应用。</span><span class="sxs-lookup"><span data-stu-id="b48cb-128">You'll use the application ID to configure the app.</span></span>

5. <span data-ttu-id="b48cb-129">在“平台”\*\*\*\* 下，选择“添加平台”\*\*\*\*，然后为应用选择合适的平台：</span><span class="sxs-lookup"><span data-stu-id="b48cb-129">Under **Platforms**, choose **Add Platform**, and select the appropriate platform for your app:</span></span>
    
    <span data-ttu-id="b48cb-130">**对于本机或移动应用**：</span><span class="sxs-lookup"><span data-stu-id="b48cb-130">**For native or mobile apps**:</span></span>

    1. <span data-ttu-id="b48cb-131">选择“本机应用程序”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b48cb-131">Select **Native Application**.</span></span>

    2. <span data-ttu-id="b48cb-p107">复制**内置重定向 URI** 值。你将需要这些来配置应用。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p107">Copy the **Built-in redirect URI** value. You'll need this to configure your app.</span></span>

        <span data-ttu-id="b48cb-134">重定向 URL 是向应用程序提供的唯一的 URI，以确保发送到此 URI 的邮件只发送到该应用程序。</span><span class="sxs-lookup"><span data-stu-id="b48cb-134">The redirect URI is a unique URI provided for your application to ensure that messages sent to that URI are only sent to that application.</span></span> 

    <span data-ttu-id="b48cb-135">**对于 Web 应用**：</span><span class="sxs-lookup"><span data-stu-id="b48cb-135">**For web apps**:</span></span>

    1. <span data-ttu-id="b48cb-136">选择“Web”\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="b48cb-136">Select **Web**.</span></span>

    2. <span data-ttu-id="b48cb-137">根据正在使用的身份验证流类型，必须确保选中“允许隐式流”复选框。</span><span class="sxs-lookup"><span data-stu-id="b48cb-137">Depending on the type of authentication flow you're using, you may have to make sure the **Allow Implicit Flow** check box is selected.</span></span> 
        
        <span data-ttu-id="b48cb-p108">“允许隐式流”选项可启用 OpenID Connect 混合流和隐式流。混合流可使应用同时接收登录信息（id 令牌）以及应用用来获取访问令牌的项目（在这种情况下，项目为授权代码）。混合流是 OWIN OpenID Connect 中间件使用的默认流。对于单页应用 (SPA)，隐式流可使应用接收登录信息和访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid and implicit flows. The hybrid flow enables the app to receive both sign-in info (the id token) and artifacts (in this case, an authorization code) that the app uses to obtain an access token. The hybrid flow is the default flow used by the OWIN OpenID Connect middleware. For single page apps (SPA), the implicit flow enables the app to receive sign-in info and the access token.</span></span> 

    3. <span data-ttu-id="b48cb-142">指定重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="b48cb-142">Specify a Redirect URL.</span></span>
        
        <span data-ttu-id="b48cb-143">重定向 URI 是 Azure AD v2.0 终结点处理身份验证请求后在应用中调用的位置。</span><span class="sxs-lookup"><span data-stu-id="b48cb-143">The redirect URL is the location in your app that the Azure AD v2.0 endpoint calls when it has processed the authentication request.</span></span>

    4. <span data-ttu-id="b48cb-p109">在“**应用程序机密**”下，选择“**生成新密码**”。从“**生成的新密码**”对话框复制应用机密。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>
        > <span data-ttu-id="b48cb-p110">**重要信息** 关闭“生成的新密码”\*\*\*\* 对话框之前，必须复制应用密钥。关闭该对话框后，将无法检索密钥。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p110">**Important** You must copy the app secret before you close the **New password generated** dialog. After you close the dialog, you cannot retrieve the secret.</span></span> 
            
6. <span data-ttu-id="b48cb-148">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="b48cb-148">Choose **Save**.</span></span>


<span data-ttu-id="b48cb-p111">下表显示了针对不同类型的应用需要配置和复制的属性。_已分配_表示你应该使用由 Azure AD 分配的值。</span><span class="sxs-lookup"><span data-stu-id="b48cb-p111">The following table shows the properties that you need to configure and copy for different kinds of apps. _Assigned_ means that you should use the value assigned by Azure AD.</span></span>


| <span data-ttu-id="b48cb-151">应用类型</span><span class="sxs-lookup"><span data-stu-id="b48cb-151">App type</span></span> | <span data-ttu-id="b48cb-152">平台</span><span class="sxs-lookup"><span data-stu-id="b48cb-152">Platform</span></span> | <span data-ttu-id="b48cb-153">应用程序 ID</span><span class="sxs-lookup"><span data-stu-id="b48cb-153">Application ID</span></span> | <span data-ttu-id="b48cb-154">应用程序密码</span><span class="sxs-lookup"><span data-stu-id="b48cb-154">Application Secret</span></span> | <span data-ttu-id="b48cb-155">重定向 URI/URL</span><span class="sxs-lookup"><span data-stu-id="b48cb-155">Redirect URI/URL</span></span> | <span data-ttu-id="b48cb-156">隐式流</span><span class="sxs-lookup"><span data-stu-id="b48cb-156">Implicit Flow</span></span> 
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="b48cb-157">本机/移动</span><span class="sxs-lookup"><span data-stu-id="b48cb-157">Native/Mobile</span></span> | <span data-ttu-id="b48cb-158">本机</span><span class="sxs-lookup"><span data-stu-id="b48cb-158">Native</span></span> | <span data-ttu-id="b48cb-159">已分配</span><span class="sxs-lookup"><span data-stu-id="b48cb-159">Assigned</span></span>  | <span data-ttu-id="b48cb-160">否</span><span class="sxs-lookup"><span data-stu-id="b48cb-160">No</span></span> | <span data-ttu-id="b48cb-161">已分配</span><span class="sxs-lookup"><span data-stu-id="b48cb-161">Assigned</span></span> | <span data-ttu-id="b48cb-162">否</span><span class="sxs-lookup"><span data-stu-id="b48cb-162">No</span></span> |
| <span data-ttu-id="b48cb-163">Web 应用</span><span class="sxs-lookup"><span data-stu-id="b48cb-163">Web App</span></span> | <span data-ttu-id="b48cb-164">Web</span><span class="sxs-lookup"><span data-stu-id="b48cb-164">Web</span></span> | <span data-ttu-id="b48cb-165">已分配</span><span class="sxs-lookup"><span data-stu-id="b48cb-165">Assigned</span></span> | <span data-ttu-id="b48cb-166">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-166">Yes</span></span> | <span data-ttu-id="b48cb-167">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-167">Yes</span></span> | <span data-ttu-id="b48cb-168">可选</span><span class="sxs-lookup"><span data-stu-id="b48cb-168">Optional</span></span> <br/><span data-ttu-id="b48cb-169">Open ID Connect 中间件默认使用混合流（是）</span><span class="sxs-lookup"><span data-stu-id="b48cb-169">Open ID Connect middleware uses hybrid flow by default (Yes)</span></span> | 
| <span data-ttu-id="b48cb-170">单页应用 (SPA)</span><span class="sxs-lookup"><span data-stu-id="b48cb-170">Single Page App (SPA)</span></span> | <span data-ttu-id="b48cb-171">Web</span><span class="sxs-lookup"><span data-stu-id="b48cb-171">Web</span></span> | <span data-ttu-id="b48cb-172">已分配</span><span class="sxs-lookup"><span data-stu-id="b48cb-172">Assigned</span></span> | <span data-ttu-id="b48cb-173">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-173">Yes</span></span> | <span data-ttu-id="b48cb-174">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-174">Yes</span></span> | <span data-ttu-id="b48cb-175">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-175">Yes</span></span> <br/> <span data-ttu-id="b48cb-176">SPA 使用 Open ID Connect 隐式流</span><span class="sxs-lookup"><span data-stu-id="b48cb-176">SPAs use Open ID Connect implicit Flow</span></span> |
| <span data-ttu-id="b48cb-177">服务/守护程序</span><span class="sxs-lookup"><span data-stu-id="b48cb-177">Service/Daemon</span></span> | <span data-ttu-id="b48cb-178">Web</span><span class="sxs-lookup"><span data-stu-id="b48cb-178">Web</span></span> | <span data-ttu-id="b48cb-179">已分配</span><span class="sxs-lookup"><span data-stu-id="b48cb-179">Assigned</span></span> | <span data-ttu-id="b48cb-180">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-180">Yes</span></span> | <span data-ttu-id="b48cb-181">是</span><span class="sxs-lookup"><span data-stu-id="b48cb-181">Yes</span></span> | <span data-ttu-id="b48cb-182">否</span><span class="sxs-lookup"><span data-stu-id="b48cb-182">No</span></span> |

<span data-ttu-id="b48cb-183">提供管理员同意体验的应用可能需要用于 Azure AD 的其他重定向 URL 返回响应。</span><span class="sxs-lookup"><span data-stu-id="b48cb-183">Apps that provide an administrator consent experience may need an additional Redirect URL for Azure AD to return the response to.</span></span>

<span data-ttu-id="b48cb-184">有关应用注册门户以及你可以为应用配置的属性的详细信息，请参阅[应用注册引用](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-v2-registration-portal)。</span><span class="sxs-lookup"><span data-stu-id="b48cb-184">For more detail about the App Registration Portal and the properties you can configure for your App, see [App registration reference](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-v2-registration-portal).</span></span>  

## <a name="azure-ad-endpoint-considerations"></a><span data-ttu-id="b48cb-185">Azure AD 终结点注意事项</span><span class="sxs-lookup"><span data-stu-id="b48cb-185">Azure AD endpoint considerations</span></span>

<span data-ttu-id="b48cb-p112">可使用 [Azure 门户](https://aka.ms/aadapplist)为 Azure AD 终结点注册应用。可以和 v2.0 终结点一样配置相同的基本属性（例如，应用程序 ID、应用程序密码和重定向 URI/URL），但是请注意以下不同之处：</span><span class="sxs-lookup"><span data-stu-id="b48cb-p112">You use the [Azure portal](https://aka.ms/aadapplist) to register your app for the Azure AD endpoint. You configure the same basic properties like Application ID, Application Secret, and Redirect URI/URL, as you would for the v2.0 endpoint; however, there are some important differences to be aware of:</span></span> 

- <span data-ttu-id="b48cb-188">只能使用工作或学校帐户注册应用。</span><span class="sxs-lookup"><span data-stu-id="b48cb-188">You can only use a work or school account to register an app.</span></span>
- <span data-ttu-id="b48cb-189">应用将需要每个平台具有不同的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="b48cb-189">Your app will require a different Application ID for each platform.</span></span>
- <span data-ttu-id="b48cb-190">如果应用是多租户应用，则必须在门户中将其显式配置为多租户。</span><span class="sxs-lookup"><span data-stu-id="b48cb-190">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant at the portal.</span></span>
- <span data-ttu-id="b48cb-191">必须在门户中预配置应用需要的所有权限（包括 Microsoft Graph 权限）。</span><span class="sxs-lookup"><span data-stu-id="b48cb-191">You must pre-configure all the permissions (including Microsoft Graph permissions) that your app needs at the portal.</span></span> 

<span data-ttu-id="b48cb-192">有关使用 Azure 门户添加应用的指导，请参阅[使用 Azure Active Directory 集成应用程序：添加应用程序](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)。</span><span class="sxs-lookup"><span data-stu-id="b48cb-192">For guidance on using the Azure portal to add an app, see [Integrating applications with Azure Active Directory: Adding an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application).</span></span>
