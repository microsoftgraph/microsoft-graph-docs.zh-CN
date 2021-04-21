---
title: 使用 Microsoft Graph API 在 Visual Studio 2017 中调用 Microsoft 365 服务
description: 你可以使用 Visual Studio 中的连接服务配置应用，从而调用 Microsoft Graph API。本文介绍如何获取登录用户的个人资料照片、将其上载至 OneDrive，和发送一封包含指向照片的共享链接的电子邮件。
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.openlocfilehash: 95fbe544edff9543d694f5fa024929fd7e241160
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921663"
---
# <a name="call-microsoft-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a><span data-ttu-id="f9a72-104">使用 Microsoft Graph API 在 Visual Studio 2017 中调用 Microsoft 365 服务</span><span class="sxs-lookup"><span data-stu-id="f9a72-104">Call Microsoft 365 services in Visual Studio 2017 with the Microsoft Graph API</span></span>

<span data-ttu-id="f9a72-p102">你可以使用 Visual Studio 中的连接服务配置应用，从而调用 Microsoft Graph API。本文介绍如何获取登录用户的个人资料照片、将其上载至 OneDrive，和发送一封包含指向照片的共享链接的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p102">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span></span>

## <a name="get-set-up"></a><span data-ttu-id="f9a72-107">开始设置</span><span class="sxs-lookup"><span data-stu-id="f9a72-107">Get set up</span></span>

<span data-ttu-id="f9a72-108">若要通过 Microsoft Graph 使用 Office 365 连接服务，你需要执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="f9a72-108">To use the Office 365 Connected Services with Microsoft Graph, you'll need to do the following:</span></span>

- <span data-ttu-id="f9a72-p103">如果未下载，请下载 [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/)。如果你使用的是 Visual Studio 的早期版本，你可以将 Visual Studio 2017 Preview 与你的当前版本并排使用。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p103">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already. If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span></span>

- <span data-ttu-id="f9a72-p104">获取 Microsoft 365 订阅。若要获取免费试用版，请加入 [Microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p104">Get a Microsoft 365 subscription. To get a free trial, join the [Microsoft 365 Developer program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="get-the-starter-project"></a><span data-ttu-id="f9a72-113">获取初学者项目</span><span class="sxs-lookup"><span data-stu-id="f9a72-113">Get the starter project</span></span>

<span data-ttu-id="f9a72-p105">下载 [Microsoft Graph ASP.NET 已连接服务示例](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip)。此示例包括针对 Microsoft Graph 进行身份验证所需的引用。下载初学者项目后，请解压，然后在 Visual Studio 2017 Preview 中打开示例。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p105">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). This sample includes the references that you need to authenticate against Microsoft Graph. After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span></span>

## <a name="add-the-connected-service"></a><span data-ttu-id="f9a72-117">添加已连接服务</span><span class="sxs-lookup"><span data-stu-id="f9a72-117">Add the Connected Service</span></span>

<span data-ttu-id="f9a72-118">你现在可以将 Microsoft Graph 服务添加到 Visual Studio 项目中。</span><span class="sxs-lookup"><span data-stu-id="f9a72-118">You're now ready to add the Microsoft Graph service to your Visual Studio project.</span></span> 

1. <span data-ttu-id="f9a72-119">在解决方案资源管理器中，选择“连接的服务”打开“连接的服务”选项卡。</span><span class="sxs-lookup"><span data-stu-id="f9a72-119">In Solution Explorer, choose **Connected Services** to open the Connected Services tab.</span></span> 

2. <span data-ttu-id="f9a72-120">选择“**使用 Microsoft Graph 访问 Microsoft 365 服务**”提供程序。</span><span class="sxs-lookup"><span data-stu-id="f9a72-120">Choose the **Access Microsoft 365 services with Microsoft Graph** provider.</span></span> <span data-ttu-id="f9a72-121">按照向导操作。</span><span class="sxs-lookup"><span data-stu-id="f9a72-121">Follow the wizard.</span></span> <span data-ttu-id="f9a72-122">选择以下权限（你可以在以后更改）：</span><span class="sxs-lookup"><span data-stu-id="f9a72-122">Select the following permissions (you can change the permissions later):</span></span>

    - <span data-ttu-id="f9a72-123">对于“文件”API，将权限设置为“拥有对文件的完全访问权限”。</span><span class="sxs-lookup"><span data-stu-id="f9a72-123">For the **File** APIs, set permissions to **Have full access to your files**.</span></span>
    - <span data-ttu-id="f9a72-124">对于“邮件”API，将权限设置为“以你的身份发送邮件”。</span><span class="sxs-lookup"><span data-stu-id="f9a72-124">For the **Mail** APIs, set permissions to **Send mail as you**.</span></span>
    - <span data-ttu-id="f9a72-125">对于“用户”API，将权限设置为“登录并读取你的个人资料”。</span><span class="sxs-lookup"><span data-stu-id="f9a72-125">For the **User** APIs, set permissions to **Sign you in and read your profile**.</span></span>

## <a name="call-the-microsoft-graph-api"></a><span data-ttu-id="f9a72-126">调用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="f9a72-126">Call the Microsoft Graph API</span></span>

<span data-ttu-id="f9a72-p107">初学者示例被配置为发送简单的电子邮件。你可以使用 Microsoft Graph 更新示例，从而发送一封包含指向 OneDrive 中已登录用户的个人资料照片的链接的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p107">The starter sample is configured to send a simple email. You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span></span>

1. <span data-ttu-id="f9a72-129">转到托管可调用 Microsoft Graph 的代码的“Models\GraphService.cs”。</span><span class="sxs-lookup"><span data-stu-id="f9a72-129">Go to 'Models\GraphService.cs', which hosts the code to call Microsoft Graph.</span></span>

2. <span data-ttu-id="f9a72-p108">按以下方法查找对 SDK 的调用并 **取消评论**。这演示了如何调用 Microsoft Graph 以获取个人资料照片、将文件上载至 OneDrive 和获取共享链接。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p108">Find and **Uncomment** calls to the SDK in the following methods. This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span></span>

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> <span data-ttu-id="f9a72-132">**提示：** 每条评论均以“//Uncomment:”开头</span><span class="sxs-lookup"><span data-stu-id="f9a72-132">**Tip:** Each comment starts with '//Uncomment:'</span></span>
 

## <a name="run-the-sample"></a><span data-ttu-id="f9a72-133">运行示例</span><span class="sxs-lookup"><span data-stu-id="f9a72-133">Run the sample</span></span>
<span data-ttu-id="f9a72-134">生成和运行示例</span><span class="sxs-lookup"><span data-stu-id="f9a72-134">Build and run the sample.</span></span> <span data-ttu-id="f9a72-135">接下来，选择右上角的“登录”链接，然后依次选择“获取电子邮件地址”和“发送电子邮件”</span><span class="sxs-lookup"><span data-stu-id="f9a72-135">Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span></span>

<span data-ttu-id="f9a72-136">这将发送一封电子邮件，其中包含指向你的个人资料照片的链接。</span><span class="sxs-lookup"><span data-stu-id="f9a72-136">This will send an email that includes a link to your profile photo.</span></span>

><span data-ttu-id="f9a72-137">**注意：**</span><span class="sxs-lookup"><span data-stu-id="f9a72-137">**Notes:**</span></span>

>- <span data-ttu-id="f9a72-138">如果停止并从 Visual Studio 中重新运行示例，你可能需要明确注销才能使示例运行。</span><span class="sxs-lookup"><span data-stu-id="f9a72-138">If you stop and rerun the sample from Visual Studio, you might need to explicitly sign out for the sample to work.</span></span>
>- <span data-ttu-id="f9a72-139">如果你收到异常，指示用户未通过身份验证，则你可能需要重复[添加连接的服务](#add-the-connected-service)步骤。</span><span class="sxs-lookup"><span data-stu-id="f9a72-139">If you get an exception that indicates that the User is not authenticated, you might need to repeat the [Add the Connected Service](#add-the-connected-service) step.</span></span>
>- <span data-ttu-id="f9a72-140">确保使用与你在向导的 **选择域** 步骤中选择的相同域中的帐户登录。</span><span class="sxs-lookup"><span data-stu-id="f9a72-140">Make sure to sign in using an account in the same domain as the one you selected in the **Select Domain** step of the wizard.</span></span>

## <a name="explore-the-code"></a><span data-ttu-id="f9a72-141">浏览代码</span><span class="sxs-lookup"><span data-stu-id="f9a72-141">Explore the code</span></span>

<span data-ttu-id="f9a72-p110">你现在可以使用 Visual Studio 2017 连接并配置你的服务。初学者示例为你创建基架和引用。</span><span class="sxs-lookup"><span data-stu-id="f9a72-p110">You can now use Visual Studio 2017 to connect to and configure your services. The starter sample creates the scaffolding and references for you.</span></span>  

<span data-ttu-id="f9a72-144">初学者示例包括以下文件：</span><span class="sxs-lookup"><span data-stu-id="f9a72-144">The starter sample includes the following files:</span></span>

- <span data-ttu-id="f9a72-145">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - 对当前用户进行身份验证并初始化该示例的令牌缓存。</span><span class="sxs-lookup"><span data-stu-id="f9a72-145">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - Authenticates the current user and initializes the sample's token cache.</span></span>

- <span data-ttu-id="f9a72-146">TokenStorage\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - 存储用户的令牌信息。</span><span class="sxs-lookup"><span data-stu-id="f9a72-146">TokenStorage\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information.</span></span> <span data-ttu-id="f9a72-147">可以使用你自己的自定义令牌缓存来替换此信息。</span><span class="sxs-lookup"><span data-stu-id="f9a72-147">You can replace this with your own custom token cache.</span></span> <span data-ttu-id="f9a72-148">有关详细信息，请参阅[在多租户应用程序中缓存访问令牌](/azure/architecture/multitenant-identity/token-cache)。</span><span class="sxs-lookup"><span data-stu-id="f9a72-148">For more information, see [Caching access tokens in a multitenant application](/azure/architecture/multitenant-identity/token-cache).</span></span>

- <span data-ttu-id="f9a72-149">Helpers\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - 实施本地 IAuthProvider 接口，并获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="f9a72-149">Helpers\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - Implements the local IAuthProvider interface, and gets an access token.</span></span> 

- <span data-ttu-id="f9a72-150">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - 初始化来自用于与 Microsoft Graph 交互的 [Microsoft Graph .NET 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)中的 **GraphServiceClient**。</span><span class="sxs-lookup"><span data-stu-id="f9a72-150">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - Initializes the **GraphServiceClient** from the [Microsoft Graph .NET Client Library](https://github.com/microsoftgraph/msgraph-sdk-dotnet) that is used to interact with the Microsoft Graph.</span></span>

- <span data-ttu-id="f9a72-151">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - 包含使用 **GraphServiceClient** 生成和发送对 Microsoft Graph 服务的调用并处理响应的方法。</span><span class="sxs-lookup"><span data-stu-id="f9a72-151">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - Contains methods that use the **GraphServiceClient** to build and send calls to the Microsoft Graph service and to process the response.</span></span>

- <span data-ttu-id="f9a72-152">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - 包含示例的 UI。</span><span class="sxs-lookup"><span data-stu-id="f9a72-152">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - Contains the UI for the sample.</span></span> 


## <a name="need-help"></a><span data-ttu-id="f9a72-153">需要帮助?</span><span class="sxs-lookup"><span data-stu-id="f9a72-153">Need help?</span></span>

<span data-ttu-id="f9a72-154">如果需要帮助，请在 [Microsoft Q&A](/answers/products/m365#microsoft-graph) 上发布你的问题。</span><span class="sxs-lookup"><span data-stu-id="f9a72-154">If you need help, post your questions on [Microsoft Q&A](/answers/products/m365#microsoft-graph).</span></span> <span data-ttu-id="f9a72-155">使用 {microsoft-graph-identity} 标记你发布的问题。</span><span class="sxs-lookup"><span data-stu-id="f9a72-155">Tag your post with {microsoft-graph-identity}.</span></span>
