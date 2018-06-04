# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a><span data-ttu-id="aabfe-101">在 ASP.NET 4.6 MVC 应用中使用 Microsoft Graph 入门</span><span class="sxs-lookup"><span data-stu-id="aabfe-101">Get started with Microsoft Graph in an ASP.NET 4.6 MVC app</span></span>

<span data-ttu-id="aabfe-p101">本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成[适用于 ASP.NET 4.6 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/aspnet-connect-sample)的步骤，并说明使用 Microsoft Graph 要实施的主要概念。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span>

<span data-ttu-id="aabfe-104">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="aabfe-104">The following image shows the app you'll create.</span></span> 

<span data-ttu-id="aabfe-105">![具备"获取电子邮件地址"和"发送电子邮件"按钮的 Web 应用](images/aspnet-connect-sample.png "具备‘获取电子邮件地址’和‘发送电子邮件’按钮的 Web 应用")</span><span class="sxs-lookup"><span data-stu-id="aabfe-105">![The web app with "Get email address" and "Send email" buttons](images/aspnet-connect-sample.png "The web app with 'Get email address' and 'Send email' buttons")</span></span>

<span data-ttu-id="aabfe-p102">[Azure AD v2.0 终结点](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-appmodel-v2-overview) 允许用户使用 Microsoft 帐户 (MSA) 或工作或学校帐户进行登录。应用使用 [ASP.Net OpenID Connect OWIN 中间件](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/)和 [适用于 .Net 的 Microsoft Authentication Library (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client) 进行登录和令牌管理。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p102">The [Azure AD v2.0 endpoint](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-appmodel-v2-overview) lets users sign in with a Microsoft account (MSA) or a work or school account. The app uses the [ASP.Net OpenID Connect OWIN middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) and the [Microsoft Authentication Library (MSAL) for .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) for sign in and token management.</span></span>

<span data-ttu-id="aabfe-p103">**不想生成一个应用吗？** 使用 [Microsoft Graph 快速入门](https://developer.microsoft.com/zh-CN/graph/quick-start)快速准备就绪并开始运行。此外请注意，我们有[此示例的 REST 版本](https://github.com/microsoftgraph/aspnet-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/zh-CN/graph/quick-start) to get up and running fast. Also note that we have a [REST version of this sample](https://github.com/microsoftgraph/aspnet-connect-rest-sample).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aabfe-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="aabfe-111">Prerequisites</span></span>

<span data-ttu-id="aabfe-112">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="aabfe-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="aabfe-113">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](https://docs.microsoft.com/zh-CN/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="aabfe-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/zh-CN/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="aabfe-114">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="aabfe-114">Visual Studio 2015</span></span> 
- <span data-ttu-id="aabfe-p104">[ASP.NET 4.6 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/aspnet-connect-sample)。将使用示例文件中的 **starter-project** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p104">The [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). You'll use the **starter-project** folder in the sample files.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="aabfe-117">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="aabfe-117">Register the application</span></span>

<span data-ttu-id="aabfe-p105">本步骤中，将会在 Microsoft 应用注册门户上注册一个应用。这会生成在 Visual Studio 中配置此应用时要使用的应用程序 ID 和密码。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p105">In this step, you'll register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="aabfe-120">使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="aabfe-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="aabfe-121">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="aabfe-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="aabfe-122">输入应用的名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="aabfe-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="aabfe-123">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="aabfe-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="aabfe-p106">复制应用程序 ID。这是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p106">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="aabfe-p107">在“**应用程序密码**”下，选择“**生成新密码**”。从“**生成的新密码**”对话框复制密码。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p107">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="aabfe-128">将使用此应用程序 ID 和密码来配置应用。</span><span class="sxs-lookup"><span data-stu-id="aabfe-128">You'll use the application ID and password to configure the app.</span></span> 

6. <span data-ttu-id="aabfe-129">在“平台”**** 下，依次选择“添加平台”**** > “Web”****。</span><span class="sxs-lookup"><span data-stu-id="aabfe-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="aabfe-130">请确保已选中“允许隐式流”**** 复选框，并输入 *http://localhost:55065/* 作为重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="aabfe-130">Make sure the Allow Implicit Flow check box is selected, and enter http://localhost:55065/ as the Redirect URI.</span></span> 

    <span data-ttu-id="aabfe-p108">“允许隐式流”**** 选项可启用 OpenID Connect 混合流。在身份验证过程中，这可使应用同时接收登录信息 (**id_token**) 以及应用用来获取访问令牌的项目（在这种情况下，项目为授权代码）。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the **id_token**) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

8. <span data-ttu-id="aabfe-133">选择“保存”****。</span><span class="sxs-lookup"><span data-stu-id="aabfe-133">Choose **Save**.</span></span>

### <a name="configure-the-project"></a><span data-ttu-id="aabfe-134">配置项目</span><span class="sxs-lookup"><span data-stu-id="aabfe-134">Configure the project</span></span>

1. <span data-ttu-id="aabfe-135">在 Visual Studio 中打开初学者项目的解决方案文件。</span><span class="sxs-lookup"><span data-stu-id="aabfe-135">Open the solution file for the starter project in Visual Studio.</span></span>

2. <span data-ttu-id="aabfe-136">打开项目的 Web.config 文件。</span><span class="sxs-lookup"><span data-stu-id="aabfe-136">Open the project's Web.config file.</span></span>

3. <span data-ttu-id="aabfe-p109">在 **appSettings** 元素中找到应用配置密钥。将 ENTER_YOUR_CLIENT_ID 和 ENTER_YOUR_SECRET 占位符值替换为刚复制的值。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p109">Locate the app configuration keys in the **appSettings** element. Replace the ENTER_YOUR_CLIENT_ID and ENTER_YOUR_SECRET placeholder values with the values you just copied.</span></span>

<span data-ttu-id="aabfe-p110">重定向 URI 是已注册项目的 URL。已请求的[权限范围](https://developer.microsoft.com/zh-CN/graph/docs/concepts/permission_scopes)允许应用获取用户配置文件信息并发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p110">The redirect URI is the URL of the project that you registered. The requested [permission scopes](https://developer.microsoft.com/zh-CN/graph/docs/concepts/permission_scopes) allow the app to get user profile information and send an email.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="aabfe-141">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aabfe-141">Call Microsoft Graph</span></span>

<span data-ttu-id="aabfe-142">在此步骤中，将会关注 **SDKHelper**、**GraphService** 和 **HomeController** 类。</span><span class="sxs-lookup"><span data-stu-id="aabfe-142">In this step, you'll focus on the **SDKHelper**, **GraphService**, and **HomeController** classes.</span></span> 

 - <span data-ttu-id="aabfe-p111">每次调用 Microsoft Graph 之前，**SDKHelper** 会初始化库的 **GraphServiceClient** 实例。在将访问令牌添加到该请求时执行此操作。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p111">**SDKHelper** intializes an instance of the **GraphServiceClient** from the library before each call to the Microsoft Graph. This is when the access token is added to the request.</span></span> 
 - <span data-ttu-id="aabfe-145">**GraphService** 使用库生成请求并将其发送到 Microsoft Graph，然后处理响应。</span><span class="sxs-lookup"><span data-stu-id="aabfe-145">**GraphService** builds and sends requests to the Microsoft Graph using the library, and processes the responses.</span></span>
 - <span data-ttu-id="aabfe-146">**HomeController** 包含初始化库调用以响应 UI 事件的操作。</span><span class="sxs-lookup"><span data-stu-id="aabfe-146">**HomeController** contains actions that initiate the calls to the library in response to UI events.</span></span>

<span data-ttu-id="aabfe-147">初学者项目已为 Microsoft Graph .NET Client Library NuGet 程序包声明依赖项：*Microsoft.Graph*。</span><span class="sxs-lookup"><span data-stu-id="aabfe-147">The starter project already declares a dependency for the Microsoft Graph .NET Client Library NuGet package:  *Microsoft.Graph*.</span></span>

1. <span data-ttu-id="aabfe-148">右键单击“帮助程序”**** 文件夹并选择“添加”**** > “类”****。</span><span class="sxs-lookup"><span data-stu-id="aabfe-148">Right-click the **Helpers** folder and choose **Add** > **Class**.</span></span> 

1. <span data-ttu-id="aabfe-149">命名新类 *SDKHelper* 并选择“添加”****。</span><span class="sxs-lookup"><span data-stu-id="aabfe-149">Name the new class *SDKHelper* and choose **Add**.</span></span>

1. <span data-ttu-id="aabfe-150">用以下代码替换内容。</span><span class="sxs-lookup"><span data-stu-id="aabfe-150">Replace the contents with the following code.</span></span>

        using System.Net.Http.Headers;
        using Microsoft.Graph;

        namespace Microsoft_Graph_SDK_ASPNET_Connect.Helpers
        {
            public class SDKHelper
            {   
                private static GraphServiceClient graphClient = null;

                // Get an authenticated Microsoft Graph Service client.
                public static GraphServiceClient GetAuthenticatedClient()
                {
                    GraphServiceClient graphClient = new GraphServiceClient(
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                                // Append the access token to the request.
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);
                            }));
                    return graphClient;
                }

                public static void SignOutClient()
                {
                    graphClient = null;
                }
            }
        }

  <span data-ttu-id="aabfe-151">请注意，初始化客户端时，调用 **SampleAuthProvider** 以获取令牌。</span><span class="sxs-lookup"><span data-stu-id="aabfe-151">Note the call to **SampleAuthProvider** to get the token when the client is initialized.</span></span>

1. <span data-ttu-id="aabfe-p112">在“模型”**** 文件夹中，打开 GraphService.cs。该服务使用库与 Microsoft Graph 进行交互。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p112">In the **Models** folder, open GraphService.cs. The service uses the library to interact with the Microsoft Graph.</span></span>

1. <span data-ttu-id="aabfe-154">添加以下 **using** 语句。</span><span class="sxs-lookup"><span data-stu-id="aabfe-154">Add the following **using** statement.</span></span>

        using Microsoft.Graph;

1. <span data-ttu-id="aabfe-p113">用以下方法替换 *// GetMyEmailAddress*。可获取当前用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p113">Replace *// GetMyEmailAddress* with the following method. This gets the current user's email address.</span></span> 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  <span data-ttu-id="aabfe-p114">请注意，**Select** 段只能请求要返回的 **mail** 和 **userPrinicipalName**。可以使用 **Select** 和 **Filter** 减少响应数据有效负载的大小。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p114">Note the **Select** segment, which requests only the **mail** and **userPrinicipalName** to be returned. You can use **Select** and **Filter** to reduce the size of the response data payload.</span></span>

1. <span data-ttu-id="aabfe-159">用以下方法替换 *// SendEmail* 以生成和发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="aabfe-159">Replace *// SendEmail* with the following methods to build and send the email.</span></span>

        // Send an email message from the current user.
        public async Task SendEmail(GraphServiceClient graphClient, Message message)
        {
            await graphClient.Me.SendMail(message, true).Request().PostAsync();
        }

        public async Task<Message> BuildEmailMessage(GraphServiceClient graphClient, string recipients, string subject)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync(graphClient);


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if ( photoStream == null)
            {
                photoStream = System.IO.File.OpenRead(System.Web.Hosting.HostingEnvironment.MapPath("/Content/test.jpg"));
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDrive(graphClient, photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            Permission sharingLink = await GetSharingLinkAsync(graphClient, photoFile.Id);

            // Add the sharing link to the email body.
            string bodyContent = string.Format(Resource.Graph_SendMail_Body_Content, sharingLink.Link.WebUrl);

            // Prepare the recipient list.
            string[] splitter = { ";" };
            string[] splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();
            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Address = recipient.Trim()
                    }
                });
            }

            // Build the email message.
            Message email = new Message
            {
                Body = new ItemBody
                {
                    Content = bodyContent,
                    ContentType = BodyType.Html,
                },
                Subject = subject,
                ToRecipients = recipientList,
                Attachments = attachments
            };
            return email;
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync(GraphServiceClient graphClient)
        {
            Stream currentUserPhotoStream = null;

            try
            {
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }

        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(GraphServiceClient graphClient, string Id)
        {
            Permission permission = null;

            try
            {
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

1. <span data-ttu-id="aabfe-160">在“控制器”**** 文件夹中，打开 HomeController.cs。</span><span class="sxs-lookup"><span data-stu-id="aabfe-160">In the **Controllers** folder, open HomeController.cs.</span></span>

1. <span data-ttu-id="aabfe-161">添加以下 **using** 语句。</span><span class="sxs-lookup"><span data-stu-id="aabfe-161">Add the following **using** statement.</span></span>

        using Microsoft.Graph;
  
1. <span data-ttu-id="aabfe-162">用以下操作替换 *// Controller actions*。</span><span class="sxs-lookup"><span data-stu-id="aabfe-162">Replace *// Controller actions* with the following actions.</span></span>

        [Authorize]
        // Get the current user's email address from their profile.
        public async Task<ActionResult> GetMyEmailAddress()
        {
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Get the current user's email address. 
                ViewBag.Email = await graphService.GetMyEmailAddress(graphClient);
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

        [Authorize]
        // Send mail on behalf of the current user.
        public async Task<ActionResult> SendEmail()
        {
            if (string.IsNullOrEmpty(Request.Form["email-address"]))
            {
                ViewBag.Message = Resource.Graph_SendMail_Message_GetEmailFirst;
                return View("Graph");
            }

            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Build the email message.
                Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Code == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

<span data-ttu-id="aabfe-163">现在可以[运行应用](#run-the-app)。</span><span class="sxs-lookup"><span data-stu-id="aabfe-163">Now you're ready to [run the app](#run-the-app).</span></span>

## <a name="run-the-app"></a><span data-ttu-id="aabfe-164">运行应用</span><span class="sxs-lookup"><span data-stu-id="aabfe-164">Run the app</span></span>
1. <span data-ttu-id="aabfe-165">按 F5 生成和运行此应用。</span><span class="sxs-lookup"><span data-stu-id="aabfe-165">Press F5 to build and run the app.</span></span> 

2. <span data-ttu-id="aabfe-166">使用个人、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="aabfe-166">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

3. <span data-ttu-id="aabfe-p115">选择“获取电子邮件地址”**** 按钮。在操作完成后，已登录用户的电子邮件地址会在此页上显示。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p115">Choose the **Get email address** button. When the operation completes, the email address of the signed-in user is displayed on the page.</span></span>

4. <span data-ttu-id="aabfe-p116">还可以编辑收件人列表和电子邮件主题，然后选择“发送电子邮件”**** 按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="aabfe-p116">Optionally edit the recipient list and email subject, and then choose the **Send email** button. When the mail is sent, a Success message is displayed below the button.</span></span>


## <a name="next-steps"></a><span data-ttu-id="aabfe-171">后续步骤</span><span class="sxs-lookup"><span data-stu-id="aabfe-171">Next steps</span></span>
- <span data-ttu-id="aabfe-172">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="aabfe-172">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="aabfe-173">在 [ASP.NET 4.6 的 Microsoft Graph 代码段示例](https://github.com/microsoftgraph/aspnet-snippets-sample)中查找常见操作的示例，或浏览 GitHub 上的其他 [ASP.NET 示例](http://aka.ms/aspnetgraphsamples)。</span><span class="sxs-lookup"><span data-stu-id="aabfe-173">Find examples of common operations in the [Microsoft Graph Snippets Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample), or explore our other [ASP.NET samples](http://aka.ms/aspnetgraphsamples) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="aabfe-174">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aabfe-174">See also</span></span>
- [<span data-ttu-id="aabfe-175">Microsoft Graph.NET 客户端库</span><span class="sxs-lookup"><span data-stu-id="aabfe-175">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="aabfe-176">用于 web API 身份验证方案的 Web 应用程序</span><span class="sxs-lookup"><span data-stu-id="aabfe-176">Web application to web API authentication scenario</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [<span data-ttu-id="aabfe-177">使用 OpenID Connect 将 Microsoft 标识和 Microsoft Graph 集成到 Web 应用程序中</span><span class="sxs-lookup"><span data-stu-id="aabfe-177">Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect</span></span>](https://azure.microsoft.com/zh-CN/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [<span data-ttu-id="aabfe-178">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="aabfe-178">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="aabfe-179">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="aabfe-179">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-tokens/)
