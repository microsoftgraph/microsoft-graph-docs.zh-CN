# <a name="get-started-with-microsoft-graph-in-a-xamarin-forms-app"></a><span data-ttu-id="c806f-101">在 Xamarin Forms 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c806f-101">Get started with Microsoft Graph in a Xamarin Forms app</span></span>

> <span data-ttu-id="c806f-p101">**为企业客户生成应用？** 如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。</span><span class="sxs-lookup"><span data-stu-id="c806f-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

<span data-ttu-id="c806f-p102">本文介绍了从 [Azure AD v2.0 终结点](https://developer.microsoft.com/graph/docs/concepts/converged_auth) 获取访问令牌和调用 Microsoft Graph 所需的任务。本文演示了 [适用于 Xamarin Forms 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) 示例中的代码，以说明在使用 Microsoft Graph 的应用中必须实现的主要概念。本文还介绍如何通过使用 [Microsoft Graph 客户端库](http://www.nuget.org/packages/Microsoft.Graph/) 来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="c806f-p102">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) sample to explain the main concepts that you have to implement in an app that uses Microsoft Graph. The article also describes how to access Microsoft Graph by using the [Microsoft Graph Client Library](http://www.nuget.org/packages/Microsoft.Graph/).</span></span>

<span data-ttu-id="c806f-108">这是将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="c806f-108">This is the app you'll create.</span></span>

| <span data-ttu-id="c806f-109">UWP</span><span class="sxs-lookup"><span data-stu-id="c806f-109">UWP</span></span> | <span data-ttu-id="c806f-110">Android</span><span class="sxs-lookup"><span data-stu-id="c806f-110">Android</span></span> | <span data-ttu-id="c806f-111">iOS</span><span class="sxs-lookup"><span data-stu-id="c806f-111">iOS</span></span> |
| --- | ------- | ----|
| <img src="images/UWP.png" alt="Connect sample on UWP" width="100%" /> | <img src="images/Droid.png" alt="Connect sample on Android" width="100%" /> | <img src="images/iOS.png" alt="Connect sample on iOS" width="100%" /> |

<span data-ttu-id="c806f-p103">**不想生成一个应用吗？** 使用 [Microsoft Graph 快速入门](https://developer.microsoft.com/graph/quick-start) 快速准备就绪并开始运行，或下载本文基于的 [Xamarin Forms 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/xamarin-csharp-connect-sample)。</span><span class="sxs-lookup"><span data-stu-id="c806f-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/graph/quick-start) to get up and running fast, or download the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) that this article is based on.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c806f-114">先决条件</span><span class="sxs-lookup"><span data-stu-id="c806f-114">Prerequisites</span></span>

<span data-ttu-id="c806f-115">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="c806f-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="c806f-116">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](https://docs.microsoft.com/zh-CN/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="c806f-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/zh-CN/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="c806f-117">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="c806f-117">Visual Studio 2015</span></span> 
- [<span data-ttu-id="c806f-118">面向 Visual Studio 的 Xamarin</span><span class="sxs-lookup"><span data-stu-id="c806f-118">Xamarin for Visual Studio</span></span>](https://www.xamarin.com/visual-studio)
- <span data-ttu-id="c806f-119">Windows 10（[已启用开发模式](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx)）</span><span class="sxs-lookup"><span data-stu-id="c806f-119">Windows 10 ([development mode enabled](https://msdn.microsoft.com/library/windows/apps/xaml/dn706236.aspx))</span></span>
- <span data-ttu-id="c806f-p104">[适用于 Xamarin Forms 的 Microsoft Graph Connect 初学者项目](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter)。此模板包含多个要向其中添加代码的类。它还包含完整视图和资源字符串。要获取此项目，请克隆或下载 [适用于 Xamarin Forms 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/xamarin-csharp-connect-sample)，并打开“**初学者**”文件夹内的 **XamarinConnect** 解决方案。</span><span class="sxs-lookup"><span data-stu-id="c806f-p104">The [Microsoft Graph Connect Starter Project for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample/tree/master/starter). This template contains several classes that you'll add code to. It also contains complete views and resource strings. To get this project, clone or download the [Microsoft Graph Connect Sample for Xamarin Forms](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) and open the **XamarinConnect** solution inside the **starter** folder.</span></span> 

<span data-ttu-id="c806f-124">如果想要在此示例中运行 iOS 项目，则要求如下：</span><span class="sxs-lookup"><span data-stu-id="c806f-124">If you want to run the iOS project in this sample, you'll need the following:</span></span>

- <span data-ttu-id="c806f-125">最新的 iOS SDK</span><span class="sxs-lookup"><span data-stu-id="c806f-125">The latest iOS SDK</span></span>
- <span data-ttu-id="c806f-126">Xcode 的最新版本</span><span class="sxs-lookup"><span data-stu-id="c806f-126">The latest version of Xcode</span></span>
- <span data-ttu-id="c806f-127">Mac OS X Sierra (10.12) 及更高版本</span><span class="sxs-lookup"><span data-stu-id="c806f-127">Mac OS X Sierra(10.12) & above</span></span> 
- [<span data-ttu-id="c806f-128">Xamarin.iOS</span><span class="sxs-lookup"><span data-stu-id="c806f-128">Xamarin.iOS</span></span>](https://docs.microsoft.com/visualstudio/mac/installation)
- <span data-ttu-id="c806f-129">[已连接到 Visual Studio 的 Xamarin Mac 代理](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)</span><span class="sxs-lookup"><span data-stu-id="c806f-129">A [Xamarin Mac agent connected to Visual Studio](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)</span></span>


## <a name="register-the-app"></a><span data-ttu-id="c806f-130">注册应用</span><span class="sxs-lookup"><span data-stu-id="c806f-130">Register the app</span></span>
 
1. <span data-ttu-id="c806f-131">使用个人或工作或学校帐户登录到[应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="c806f-131">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="c806f-132">选择“添加应用”****。</span><span class="sxs-lookup"><span data-stu-id="c806f-132">Select **Add an app**.</span></span>
3. <span data-ttu-id="c806f-133">输入应用名称，然后选择“创建”****。</span><span class="sxs-lookup"><span data-stu-id="c806f-133">Enter a name for the app, and select **Create**.</span></span>
    
    <span data-ttu-id="c806f-134">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="c806f-134">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="c806f-135">在“平台”**** 下，选择“添加平台”****。</span><span class="sxs-lookup"><span data-stu-id="c806f-135">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="c806f-136">选择“本机应用程序”****。</span><span class="sxs-lookup"><span data-stu-id="c806f-136">Select **Native Application**.</span></span>
6. <span data-ttu-id="c806f-p105">复制应用 ID 值，以及在添加“本机应用”平台时创建的自定义重定向 URI 值（在“本机应用”标头下）。此 URI 应包含应用 ID 值，格式如下：。需要在示例应用中输入这些值。</span><span class="sxs-lookup"><span data-stu-id="c806f-p105">Copy the Application Id value and the Custom Redirect URI value (under the **Native Application** header) that was created for you when you added the **Native Application** platform. This URI should contain your Application Id value and be in this form: `msal[Application Id]://auth` You'll need to enter these values into the sample app.</span></span>

    <span data-ttu-id="c806f-139">应用 ID 是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c806f-139">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="c806f-140">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="c806f-140">Select **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="c806f-141">配置项目</span><span class="sxs-lookup"><span data-stu-id="c806f-141">Configure the project</span></span>

1. <span data-ttu-id="c806f-142">在 Visual Studio 中打开初学者项目的解决方案文件。</span><span class="sxs-lookup"><span data-stu-id="c806f-142">Open the solution file for the starter project in Visual Studio.</span></span>
2. <span data-ttu-id="c806f-p106">打开 **XamarinConnect (可移植)** 项目中的 **App.cs** 文件，然后找到 `ClientId` 字段。使用注册应用的应用程序 ID 替换应用程序 ID 占位符。</span><span class="sxs-lookup"><span data-stu-id="c806f-p106">Open the **App.cs** file inside the **XamarinConnect (Portable)** project and locate the `ClientId` field. Replace the application ID placeholder with the application id of the app you registered.</span></span>

    ```
    public static string ClientID = "ENTER_YOUR_CLIENT_ID";
    public static string RedirectUri = "msal" + ClientID + "://auth";
    public static string[] Scopes = { "User.Read", "Mail.Send", "Files.ReadWrite" };
    ```
    <span data-ttu-id="c806f-p107">当用户进行身份验证时，`Scopes` 值将存储应用需要请求的 Microsoft Graph 权限范围。请注意，`App` 类构造函数使用 ClientID 值来实例化 MSAL `PublicClientApplication` 类的实例。稍后，将使用该类来验证用户身份。</span><span class="sxs-lookup"><span data-stu-id="c806f-p107">The `Scopes` value stores the Microsoft Graph permission scopes that the app will need to request when the user authenticates. Note that the `App` class constructor uses the ClientID value to instantiate an instance of the MSAL `PublicClientApplication` class. You'll use this class later to authenticate the user.</span></span>
    
    ```
    IdentityClientApp = new PublicClientApplication(ClientID);
    ```

3. <span data-ttu-id="c806f-p108">在文本编辑器中，打开 UserDetailsClient.iOS\info.plist 文件。遗憾的是，不能在 Visual Studio 中编辑此文件。在 `CFBundleURLSchemes` 键下查找 `<string>msalENTER_YOUR_CLIENT_ID</string>` 元素。</span><span class="sxs-lookup"><span data-stu-id="c806f-p108">Open the UserDetailsClient.iOS\info.plist file in a text editor. Unfortunately you can't edit this file in Visual Studio. Locate the `<string>msalENTER_YOUR_CLIENT_ID</string>` element under `CFBundleURLSchemes` key.</span></span>

4. <span data-ttu-id="c806f-p109">将 `ENTER_YOUR_CLIENT_ID` 替换成注册应用时获取的应用 ID 值。请务必保留应用 ID 前面的 `msal`。生成的字符串值应如下所示：`<string>msal[application id]</string>`。</span><span class="sxs-lookup"><span data-stu-id="c806f-p109">Replace `ENTER_YOUR_CLIENT_ID` with the application id value that you got when you registered your app. Be sure to retain `msal` before the application id. The resulting string value should look like this: `<string>msal[application id]</string>`.</span></span>

5. <span data-ttu-id="c806f-p110">打开 UserDetailsClient.Droid\Properties\AndroidManifest.xml 文件。查找以下元素：`<data android:scheme="msalENTER_YOUR_CLIENT_ID" android:host="auth" />`。</span><span class="sxs-lookup"><span data-stu-id="c806f-p110">Open the UserDetailsClient.Droid\Properties\AndroidManifest.xml file. Locate this element: `<data android:scheme="msalENTER_YOUR_CLIENT_ID" android:host="auth" />`.</span></span>

6. <span data-ttu-id="c806f-p111">将 `ENTER_YOUR_CLIENT_ID` 替换成注册应用时获取的应用 ID 值。请务必保留应用 ID 前面的 `msal`。生成的字符串值应如下所示：`<data android:scheme="msal[application id]" android:host="auth" />`。</span><span class="sxs-lookup"><span data-stu-id="c806f-p111">Replace `ENTER_YOUR_CLIENT_ID` with the application id value that you got when you registered your app. Be sure to retain `msal` before the application id. The resulting string value should look like this: `<data android:scheme="msal[application id]" android:host="auth" />`.</span></span>

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="c806f-157">使用 Microsoft Graph 发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="c806f-157">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="c806f-158">打开初学者项目中的 MailHelper.cs 文件。</span><span class="sxs-lookup"><span data-stu-id="c806f-158">Open the MailHelper.cs file in your starter project.</span></span> <span data-ttu-id="c806f-159">该文件中包含构建并发送电子邮件的代码。</span><span class="sxs-lookup"><span data-stu-id="c806f-159">This file contains the code that constructs and sends an email.</span></span> <span data-ttu-id="c806f-160">它包含单个方法 ``ComposeAndSendMailAsync``，该方法会构建并将 POST 请求发送到 **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail** 终结点。</span><span class="sxs-lookup"><span data-stu-id="c806f-160">The MailHelper.cs file contains the code that constructs and sends an email. It consists of a single method --  -- that constructs and sends a POST request to the https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail endpoint.</span></span> 

<span data-ttu-id="c806f-p113">``ComposeAndSendMailAsync`` 方法采用三个字符串值 -- ``subject``、``bodyContent`` 和 ``recipients`` -- 通过 MainPage.xaml.cs 文件将这些值传递给它。``subject`` 和 ``bodyContent`` 字符串随所有其他 UI 字符串存储在 AppResources.resx 文件中。``recipients`` 字符串来自应用界面中的地址框中。</span><span class="sxs-lookup"><span data-stu-id="c806f-p113">The ``ComposeAndSendMailAsync`` method takes three string values -- ``subject``, ``bodyContent``, and ``recipients`` -- that are passed to it by the MainPage.xaml.cs file. The ``subject`` and ``bodyContent`` strings are stored, along with all other UI strings, in the AppResources.resx file. The ``recipients`` string comes from the address box in the app's interface.</span></span> 

<span data-ttu-id="c806f-164">**使用声明**</span><span class="sxs-lookup"><span data-stu-id="c806f-164">**Using declarations**</span></span>

<span data-ttu-id="c806f-165">请确保将这些声明置于文件顶部：</span><span class="sxs-lookup"><span data-stu-id="c806f-165">Make sure you have these declarations at the top of the file:</span></span>

```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Reflection;
using System.Threading.Tasks;
using Microsoft.Graph;
```

<span data-ttu-id="c806f-p114">``ComposeAndSendMailAsync`` 方法中的第一个任务是从 Microsoft Graph 中获取当前用户的照片。此行调用无存根 `GetCurrentUserPhotoStreamAsync` 方法：</span><span class="sxs-lookup"><span data-stu-id="c806f-p114">The first task inside the ``ComposeAndSendMailAsync`` method is to get the current user's photo from Microsoft Graph. This line calls the stubbed-out `GetCurrentUserPhotoStreamAsync` method:</span></span>

```
            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();
```

<span data-ttu-id="c806f-168">完整的 `GetCurrentUserPhotoStreamAsync` 方法如下所示：</span><span class="sxs-lookup"><span data-stu-id="c806f-168">This is what the complete `GetCurrentUserPhotoStreamAsync` method looks like:</span></span>

```
        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }
```

<span data-ttu-id="c806f-169">如果用户没有照片，此逻辑会获取项目中包含的其他图像文件：</span><span class="sxs-lookup"><span data-stu-id="c806f-169">If the user doesn't have a photo, this logic gets another image file that has been included with the project:</span></span>

```
            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
            }
```

<span data-ttu-id="c806f-170">现在已拥有图像流，可以通过调用无存根的 `UploadFileToOneDriveAsync` 方法将此文件上载到 OneDrive：</span><span class="sxs-lookup"><span data-stu-id="c806f-170">Now that we have an image stream, we can upload the file to OneDrive by calling the stubbed-out `UploadFileToOneDriveAsync` method:</span></span>

```
            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());
```

<span data-ttu-id="c806f-171">完整的 `UploadFileToOneDriveAsync` 方法如下所示：</span><span class="sxs-lookup"><span data-stu-id="c806f-171">This is what the complete `UploadFileToOneDriveAsync` method looks like:</span></span>

```
        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }
```

<span data-ttu-id="c806f-172">我们还可以使用该流创建可以随消息传递的 `MessageAttachmentsCollectionPage` 对象。</span><span class="sxs-lookup"><span data-stu-id="c806f-172">We can also use this stream to create a `MessageAttachmentsCollectionPage` object that we can pass along with the message:</span></span>

```
            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });
```

<span data-ttu-id="c806f-p115">我们可以通过调用无存根 `GetSharingLinkAsync` 方法获取新上载的 OneDrive 文件的共享链接。`bodyContent` 字符串包含共享链接的占位符。</span><span class="sxs-lookup"><span data-stu-id="c806f-p115">We can get a sharing link for the newly uploaded OneDrive file by calling the stubbed-out `GetSharingLinkAsync` method. The `bodyContent` string contains a placeholder for the sharing link:</span></span>

```
            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);
```

<span data-ttu-id="c806f-175">完整的 `GetSharingLinkAsync` 方法如下所示：</span><span class="sxs-lookup"><span data-stu-id="c806f-175">This is what the complete `GetSharingLinkAsync` method looks like:</span></span>

```
        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }
```

<span data-ttu-id="c806f-176">由于用户可以传递多个地址，因此下一项任务是将 ``recipients`` 字符串拆分为一组可用于构建 `Recipients` 对象列表的 `EmailAddress` 对象，然后能够以请求 POST 正文的形式传递这些对象：</span><span class="sxs-lookup"><span data-stu-id="c806f-176">Since the user can potentially pass more than one address, the next task is to split the ``recipients`` string into a set of `EmailAddress` objects that can then be used to construct the list of `Recipients` objects that will be passed in the POST body of the request:</span></span>

```
            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }
```

<span data-ttu-id="c806f-p116">最后一项任务是构建 `Message` 对象，然后通过 `GraphServiceClient` 将它发送至 **me/microsoft.graph.SendMail** 终结点。由于 ``bodyContent`` 字符串是一个 HTML 文档，因此请求将 **ContentType** 值设置为 HTML。</span><span class="sxs-lookup"><span data-stu-id="c806f-p116">The last task is to construct a `Message` object and send it to the **me/microsoft.graph.SendMail** endpoint through the `GraphServiceClient`. Since the ``bodyContent`` string is an HTML document, the request sets the **ContentType** value to HTML.</span></span>

```
            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
```

<span data-ttu-id="c806f-179">完整的类如下所示：</span><span class="sxs-lookup"><span data-stu-id="c806f-179">The complete class will look like this:</span></span>

```
    public class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        public async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync();


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if (photoStream == null)
            {
                var assembly = typeof(MailHelper).GetTypeInfo().Assembly;
                photoStream = assembly.GetManifestResourceStream("XamarinConnect.test.jpg");
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDriveAsync(photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            // Get the sharing link and insert it into the message body.
            Permission sharingLink = await GetSharingLinkAsync(photoFile.Id);
            string bodyContentWithSharingLink = String.Format(bodyContent, sharingLink.Link.WebUrl);


            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContentWithSharingLink,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                    Attachments = attachments
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync()
        {
            Stream currentUserPhotoStream = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
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
        public async Task<DriveItem> UploadFileToOneDriveAsync(byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(string Id)
        {
            Permission permission = null;

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }


    }
``` 

<span data-ttu-id="c806f-180">现在，已经执行了与 Microsoft Graph 进行交互所需的三个步骤：应用注册、用户身份验证以及进行请求。</span><span class="sxs-lookup"><span data-stu-id="c806f-180">You've now performed the three steps required for interacting with Microsoft Graph: app registration, user authentication, and making a request.</span></span> 

## <a name="run-the-app"></a><span data-ttu-id="c806f-181">运行应用</span><span class="sxs-lookup"><span data-stu-id="c806f-181">Run the app</span></span>
1. <span data-ttu-id="c806f-p117">选择想要运行的项目。如果选择“通用 Windows 平台”选项，则可以在本地计算机上运行示例。如果想要运行 iOS 项目，则需连接到安装在其上的 [具有 Xamarin 工具的 Mac](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/)。（还可以在 Mac 上的 Xamarin Studio 中打开此解决方案并直接从此处运行示例。）如果想要运行 Android 项目，可以使用[适用于 Android 的 Visual Studio 模拟器](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx)。</span><span class="sxs-lookup"><span data-stu-id="c806f-p117">Select the project that you want to run. If you select the Universal Windows Platform option, you can run the sample on the local machine. If you want to run the iOS project, you'll need to connect to a [Mac that has the Xamarin tools](https://developer.xamarin.com/guides/ios/getting_started/installation/windows/connecting-to-mac/) installed on it. (You can also open this solution in Xamarin Studio on a Mac and run the sample directly from there.) You can use the [Visual Studio Emulator for Android](https://www.visualstudio.com/features/msft-android-emulator-vs.aspx) if you want to run the Android project.</span></span> 

    <span data-ttu-id="c806f-186">![](images/SelectProject.png "在 Visual Studio 中选择项目")</span><span class="sxs-lookup"><span data-stu-id="c806f-186">![](images/SelectProject.png "Select project in Visual Studio")</span></span>

2. <span data-ttu-id="c806f-p118">按 F5 进行构建和调试。运行此解决方案并使用个人或工作或学校帐户登录。</span><span class="sxs-lookup"><span data-stu-id="c806f-p118">Press F5 to build and debug. Run the solution and sign in with either your personal or work or school account.</span></span>
    > <span data-ttu-id="c806f-189">**注意**：可能需要打开生成配置管理器，以确保为 UWP 项目选择“生成”和“部署”步骤。</span><span class="sxs-lookup"><span data-stu-id="c806f-189">**Note** You might have to open the Build Configuration Manager to make sure that the Build and Deploy steps are selected for the UWP project.</span></span> 

3. <span data-ttu-id="c806f-190">使用个人帐户、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="c806f-190">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

4. <span data-ttu-id="c806f-p119">选择“发送邮件”**** 按钮。在邮件发送后，将显示成功消息。此邮件包含附件形式的照片，同时还提供到 OneDrive 中上载的文件的共享链接。</span><span class="sxs-lookup"><span data-stu-id="c806f-p119">Choose the **Send mail** button. When the mail is sent, a Success message is displayed. This mail message includes the photo as an attachment and also provides a sharing link to the uploaded file in OneDrive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c806f-194">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c806f-194">Next steps</span></span>
- <span data-ttu-id="c806f-195">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="c806f-195">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="c806f-196">在 [amarin.Forms 的 Microsoft Graph SDK 代码段库](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample) 中查找常见操作示例，或在 GitHub 上浏览我们的其他 [Xamarin 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin)。</span><span class="sxs-lookup"><span data-stu-id="c806f-196">Find examples of common operations in the [Microsoft Graph SDK Snippets Library for Xamarin.Forms](https://github.com/microsoftgraph/xamarin-csharp-snippets-sample), or explore our other [Xamarin samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=xamarin) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="c806f-197">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c806f-197">See also</span></span>
- [<span data-ttu-id="c806f-198">Microsoft Graph.NET 客户端库</span><span class="sxs-lookup"><span data-stu-id="c806f-198">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="c806f-199">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="c806f-199">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="c806f-200">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="c806f-200">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/documentation/articles/active-directory-v2-tokens/)
