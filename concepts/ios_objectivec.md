# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a><span data-ttu-id="e893d-101">在 Objective-C iOS 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e893d-101">Get started with Microsoft Graph in an Objectve C iOS App</span></span>

> <span data-ttu-id="e893d-p101">**为企业客户生成应用？** 如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。</span><span class="sxs-lookup"><span data-stu-id="e893d-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="e893d-p102">若要跨**所有企业方案**支持**全部企业客户**，必须使用 Azure AD 终结点，并使用 [Azure 门户](https://aka.ms/aadapplist)管理应用。有关详细信息，请参阅[在 Azure AD 和 Azure AD v2.0 终结点之间进行选择](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="e893d-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="e893d-p103">本文介绍了从 [Azure AD v2.0 终结点](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) 获取访问令牌和调用 Microsoft Graph 所需的任务。本文演示了 [适用于 iOS 的 Office 365 Connect 示例 (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) 中的代码，以说明你在使用 Microsoft Graph 的应用中必须实现的主要概念。本文介绍了如何通过使用 [适用于 iOS 的Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios) 来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="e893d-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="e893d-110">可以在以下 GitHub 存储库中下载要创建的应用版本：</span><span class="sxs-lookup"><span data-stu-id="e893d-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="e893d-111">使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例</span><span class="sxs-lookup"><span data-stu-id="e893d-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="e893d-112">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="e893d-112">The following image shows the app you'll create.</span></span>

![Connect 示例演练演示了在应用中进行连接和发送邮件](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="e893d-114">将工作流连接到 Microsoft Graph 并进行身份验证，通过工作或个人帐户登录，最后向收件人发送邮件。</span><span class="sxs-lookup"><span data-stu-id="e893d-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="e893d-p104">**不想生成一个应用吗？** 使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/en-us/getting-started) 快速准备就绪并开始运行。</span><span class="sxs-lookup"><span data-stu-id="e893d-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e893d-117">先决条件</span><span class="sxs-lookup"><span data-stu-id="e893d-117">Prerequisites</span></span>

<span data-ttu-id="e893d-118">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="e893d-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="e893d-119">Apple 的 [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="e893d-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="e893d-120">安装 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) 作为依存关系管理器。</span><span class="sxs-lookup"><span data-stu-id="e893d-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="e893d-121">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="e893d-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
* <span data-ttu-id="e893d-122">[适用于 iOS 的 Microsoft Graph 初学者项目](https://github.com/microsoftgraph/ios-objectivec-connect-sample)</span><span class="sxs-lookup"><span data-stu-id="e893d-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="e893d-123">本模板包含可向其添加代码的类。</span><span class="sxs-lookup"><span data-stu-id="e893d-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="e893d-124">若要获取此项目，请在此位置克隆或下载示例项目，然后可以使用 **starter-project** 文件夹中的工作区 (**ios-objectivec-connect-sample.xcworkspace**)。</span><span class="sxs-lookup"><span data-stu-id="e893d-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="e893d-125">注册应用</span><span class="sxs-lookup"><span data-stu-id="e893d-125">Register the app</span></span>
 
1. <span data-ttu-id="e893d-126">使用个人或工作或学校帐户登录到 [应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="e893d-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="e893d-127">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="e893d-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="e893d-128">为应用输入名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="e893d-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="e893d-129">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="e893d-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="e893d-130">在“平台”**** 下，选择“添加平台”****。</span><span class="sxs-lookup"><span data-stu-id="e893d-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="e893d-131">选择“本机平台”****。</span><span class="sxs-lookup"><span data-stu-id="e893d-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="e893d-p106">将客户端 ID 复制到剪贴板。将需要在示例应用中输入该值。</span><span class="sxs-lookup"><span data-stu-id="e893d-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="e893d-134">应用 ID 是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e893d-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="e893d-135">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="e893d-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="e893d-136">导入项目依赖项</span><span class="sxs-lookup"><span data-stu-id="e893d-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="e893d-137">克隆该存储库，[使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例](https://github.com/microsoftgraph/ios-objectivec-connect-sample)。</span><span class="sxs-lookup"><span data-stu-id="e893d-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="e893d-138">重要说明：使用的是 starter-project 文件夹中的示例，而不是项目根目录中的示例。</span><span class="sxs-lookup"><span data-stu-id="e893d-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="e893d-p107">使用 CocoaPods 导入 Microsoft Graph SDK 和身份验证依赖项。该示例应用已包含可将 pod 导入到项目中的 pod 文件。导航至“**终端**”应用中的“**starter-project**”文件夹，然后在“**终端**”中运行：</span><span class="sxs-lookup"><span data-stu-id="e893d-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="e893d-p108">将收到已将 pod 导入到项目的确认消息。有关详细信息，请参阅 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="e893d-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="e893d-144">启用密钥链共享</span><span class="sxs-lookup"><span data-stu-id="e893d-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="e893d-p109">对于 Xcode 8，将需要添加密钥链组，否则应用将无法访问密钥链。添加密钥链组：</span><span class="sxs-lookup"><span data-stu-id="e893d-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="e893d-p110">在 Xcode 项目管理器面板上选择项目。(⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="e893d-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="e893d-149">选择“iOS-ObjectiveC-Connect-Sample”****。</span><span class="sxs-lookup"><span data-stu-id="e893d-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="e893d-150">在“功能”选项卡上启用“密钥链共享”****。</span><span class="sxs-lookup"><span data-stu-id="e893d-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="e893d-151">将 **com.microsoft.ios-objectivec-connect-sample** 添加到钥匙链组。</span><span class="sxs-lookup"><span data-stu-id="e893d-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="e893d-152">使用 Microsoft Graph 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="e893d-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="e893d-p111">若要重新访问 UI 工作流，应用需要验证用户身份，然后他们就可以向特定用户发送邮件。若要生成对 Microsoft Graph 服务的请求，必须提供身份验证提供程序（它能够使用适当的 OAuth 2.0 持有者令牌对 HTTPS 请求进行身份验证）。在示例项目中，具有已作为存根的名为 **AuthenticationProvider.m** 的身份验证类。我们将向请求添加一个函数，然后获取一个调用 Microsoft Graph API 的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e893d-p111">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="e893d-157">打开“**starter-project**”文件夹中的 Xcode 项目工作区 (**iOS-ObjectiveC-Connect-Sample.xcworkspace**)，然后导航至“**身份验证**”文件夹并打开文件 **AuthenticationProvider.m**。</span><span class="sxs-lookup"><span data-stu-id="e893d-157">Open the Xcode project workspace (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.**</span></span> <span data-ttu-id="e893d-158">将下列代码添加至该类。</span><span class="sxs-lookup"><span data-stu-id="e893d-158">Add the following code to that class.</span></span>

```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)    (NSError *))completion{
      [NXOAuth2AuthenticationProvider setClientId:kClientId scopes:scopes];
      /**
      Obtains access token by performing login with UI, where viewController specifies the parent view controller.
      @param viewController The view controller to present the UI on.
      @param completionHandler The completion handler to be called when the authentication has completed.
      error should be non nil if there was no error, and should contain any error(s) that occurred.
      */

      if ([[NXOAuth2AuthenticationProvider sharedAuthProvider] loginSilent]) {
         completion(nil);
      }
      else {
         [[NXOAuth2AuthenticationProvider sharedAuthProvider] loginWithViewController:nil completion:^(NSError *error) {
            if (!error) {
               NSLog(@"Authentication successful.");
               completion(nil);
            }
            else {
               NSLog(@"Authentication failed - %@", error.localizedDescription);
               completion(error);
            }
         }];
      }
   }
```     

2. <span data-ttu-id="e893d-p113">接下来，将此方法添加至头文件。打开文件 **AuthenticationProvider.h**，然后将下列代码添加至此类。</span><span class="sxs-lookup"><span data-stu-id="e893d-p113">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. <span data-ttu-id="e893d-p114">最后，我们将从 **ConnectViewController.m** 中调用此方法。该控制器是应用加载的默认视图，其中存在名称为“**连接**”的单个按钮，用户将点按此按钮启动身份验证流程。此方法采用两个参数，即 **Client ID** 和 **scopes**，我们将在后续部分详细介绍它们。将以下操作添加到 **ConnectViewController.m**。</span><span class="sxs-lookup"><span data-stu-id="e893d-p114">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

```objectivec
- (IBAction)connectTapped:(id)sender {
   [self showLoadingUI:YES];
   NSArray *scopes = [kScopes componentsSeparatedByString:@","];
   [self.authProvider connectToGraphWithClientId:kClientId scopes:scopes completion:^(NSError *error) {
   if (!error) {
      [self performSegueWithIdentifier:@"showSendMail" sender:nil];
      [self showLoadingUI:NO];
      NSLog(@"Authentication successful.");
   }
   else{
      NSLog(NSLocalizedString(@"CHECK_LOG_ERROR", error.localizedDescription));
      [self showLoadingUI:NO];
   };
  }];
}
```     

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="e893d-165">使用 Microsoft Graph 发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="e893d-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="e893d-p115">将项目配置为可以进行身份验证后，下一项任务则是使用 Microsoft Graph API 向用户发送邮件。默认情况下，将已登录用户视作收件人，但是可以将其更改为其他任何收件人。我们在此处要使用的代码位于“**控制器**”文件夹和 **SendMailViewController.m** 类中。将看到在此处展示了用于 UI 的其他代码，还有一个用来从 Microsoft Graph 服务检索用户个人资料信息的 Helper 方法。我们将着重介绍创建邮件并发送邮件的方法。</span><span class="sxs-lookup"><span data-stu-id="e893d-p115">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="e893d-171">打开“控制器”文件夹中的 **SendMailViewController.m**，并在 `self.graphClient = [MSGraphClient client]` 后将以下代码添加到 **viewDidLoad** 方法。</span><span class="sxs-lookup"><span data-stu-id="e893d-171">Open **SendMailViewController.m** in the Controllers folder and add the following code to the **viewDidLoad** method, after `self.graphClient = [MSGraphClient client]`</span></span>
   ```objectivec
       [self getUserInfo:(self.emailAddress) completion:^( NSError *error) {
        if (!error) {
            [self getUserPicture:(self.emailAddress)  completion:^(UIImage *image, NSError *error) {
                if (!error) {
                    self.userPicture = image;
                } else {
                    //get the test image out of the project resources
                    self.userPicture = [UIImage imageNamed:(@"test.png")];
                }
                [self uploadPictureToOneDrive:(self.userPicture) completion:^(NSString *webUrl, NSError *error) {
                    if (!error) {
                        self.pictureWebUrl = webUrl;
                        dispatch_async(dispatch_get_main_queue(), ^{
                            self.sendMailButton.enabled = true;
                        });
                    } else {
                        dispatch_async(dispatch_get_main_queue(), ^{
                            NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                            self.statusTextView.text = NSLocalizedString(@"PICTURE_UPLOAD_FAILURE", comment: "");
                        });
                    }
                }];
            }];
        }
    }];
   ```

1. <span data-ttu-id="e893d-172">打开“控制器”文件夹中的 **SendMailViewController.m**</span><span class="sxs-lookup"><span data-stu-id="e893d-172">Open **SendMailViewController.m.**</span></span> <span data-ttu-id="e893d-173">，将下列 Helper 方法添加到类中</span><span class="sxs-lookup"><span data-stu-id="e893d-173">in the Controllers folder and add the following helper method to the class</span></span>
```objectivec
  //Create a sample test message to send to specified user account
  -(MSGraphMessage*) getSampleMessage{
      MSGraphMessage *message = [[MSGraphMessage alloc]init];
      MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
      MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
      //need to get email text field for send to!
    
      email.address = self.emailAddress;
      toRecipient.emailAddress = email;
    
      NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
      [toRecipients addObject:toRecipient];
    
      message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
      MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
      NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
      NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
      emailBody.content = htmlContentString;
      NSString *replaceString = @"a href=";
      replaceString = [replaceString stringByAppendingString:(self.pictureWebUrl)];
      emailBody.content = [emailBody.content stringByReplacingOccurrencesOfString:(@"a href=%s") withString:(replaceString)];
      emailBody.contentType = [MSGraphBodyType html];
      message.body = emailBody;
    
      message.toRecipients = toRecipients;
    
      MSGraphFileAttachment *fileAttachment= [[MSGraphFileAttachment alloc]init];
      fileAttachment.oDataType = @"#microsoft.graph.fileAttachment";
      fileAttachment.contentType = @"image/png";
    
      NSString *decodedString = [UIImagePNGRepresentation(self.userPicture) base64EncodedStringWithOptions:NSDataBase64EncodingEndLineWithCarriageReturn];
    
      fileAttachment.contentBytes = decodedString;
      fileAttachment.name = @"me.png";
      message.attachments = [message.attachments arrayByAddingObject:(fileAttachment)];
      return message;
    
    }
```
3. <span data-ttu-id="e893d-174">打开 **SendMailViewController.m** 并将以下方法添加到类中。</span><span class="sxs-lookup"><span data-stu-id="e893d-174">Open **SendMailViewController.m** Add the following method to the class.</span></span>
<span data-ttu-id="e893d-175">**uploadPictureToOneDrive** 从用户的[用户](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)信息上传[用户](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)的个人资料图片，并返回由示例发送的要嵌入电子邮件正文中的 Web 共享 URL。</span><span class="sxs-lookup"><span data-stu-id="e893d-175">**uploadPictureToOneDrive** uploads the [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)'s profile picture from their [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) information and returns the web sharing Url to be embedded in the body of the email that is sent by the sample.</span></span>

  ```objectivec
  -(void) uploadPictureToOneDrive: (UIImage *) image completion:(void(^) (NSString*, NSError*))completionBlock{
    
    NSData *data = UIImagePNGRepresentation(image);
    [[[[[[[self.graphClient me]
          drive]
         root]
        children]
       driveItem:(@"me.png")]
      contentRequest]
     uploadFromData:(data) completion:^(MSGraphDriveItem *response, NSError *error) {
         
         if (!error) {
             NSString *webUrl = response.webUrl;
             completionBlock(webUrl, error);
         } else {
             dispatch_async(dispatch_get_main_queue(), ^{
                 self.statusTextView.text =  NSLocalizedString(@"USER_GET_PICTURE_FAILURE", comment: "");
                 NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
             });
         }
     }];
    }
  ```
4. <span data-ttu-id="e893d-176">打开 **SendMailViewController.m** 并将以下方法添加到类中。</span><span class="sxs-lookup"><span data-stu-id="e893d-176">Open **SendMailViewController.m** and add the following method to the class.</span></span> 
<span data-ttu-id="e893d-177">**getUserPicture** 返回[用户](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)的个人资料图片（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="e893d-177">**getUserPicture** returns the [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)'s profile picture if it is available.</span></span>
   ```objectivec
   -(void) getUserPicture: (NSString *)url completion:(void(^) (UIImage*, NSError*))completionBlock {
    
    [[[self.graphClient me] photoValue] downloadWithCompletion:^(NSURL *location, NSURLResponse *response, NSError *error) {
        //code
        if (!error) {
            NSData *data = [NSData dataWithContentsOfURL:location];
            UIImage *img = [[UIImage alloc] initWithData:data];
            completionBlock(img, error);
        } else{
            completionBlock(nil, error);

        }
    }];
    }

   ```
3. <span data-ttu-id="e893d-178">打开 **SendMailViewcontroller.m** 并将以下方法添加到类中。</span><span class="sxs-lookup"><span data-stu-id="e893d-178">Open **SendMailViewcontroller.m** and add the following method to the class.</span></span>
<span data-ttu-id="e893d-179">此方法获取可表示经过身份验证的用户的 [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) 资源，并缓存必要的字段以获取用户的个人资料图片并发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e893d-179">This method gets the [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) resource representing the authenticated user and caches the fields necessary to get the user's profile picture and send an email.</span></span>
   ```objectivec
   //Retrieve the logged in user's display name and email address
   -(void) getUserInfo: (NSString *)url completion:(void(^) ( NSError*))completionBlock{
    
    [[[self.graphClient me]request]getWithCompletion:^(MSGraphUser *response, NSError *error) {
        if(!error){
            dispatch_async(dispatch_get_main_queue(), ^{
                self.emailAddress = response.userPrincipalName;
                self.emailTextField.text = self.emailAddress;
                self.headerLabel.text = [NSString stringWithFormat:(NSLocalizedString(@"HI_USER", comment "")), response.displayName];
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_SUCCESS", comment: "");
            });

            completionBlock(nil);
        }
        else{
            dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_FAILURE", comment: "");
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            });
            completionBlock(error);
        }
    }];
    
   }

   ```
3. <span data-ttu-id="e893d-180">打开 **SendMailViewController.m** 将以下发送邮件方法添加到类中。</span><span class="sxs-lookup"><span data-stu-id="e893d-180">Open **SendMailViewController.m** Add the following send mail method to the class.</span></span>
<span data-ttu-id="e893d-181">**getSampleMessage** 创建 HTML 示例邮件草稿以用于演示目的。</span><span class="sxs-lookup"><span data-stu-id="e893d-181">**getSampleMessage** creates a draft HTML sample mail to use for demo purposes.</span></span> <span data-ttu-id="e893d-182">下一个方法 **sendMail** 将获取该邮件，然后执行该请求发送邮件。</span><span class="sxs-lookup"><span data-stu-id="e893d-182">The next method, **sendMail**, then takes that message and executes the request to send it.</span></span> <span data-ttu-id="e893d-183">同样，默认收件人为登录用户。</span><span class="sxs-lookup"><span data-stu-id="e893d-183">Again the default recipient is the signed-in user.</span></span>


  ```objectivec
   //Send mail to the specified user in the email text field
   -(void) sendMail {
    MSGraphMessage *message = [self getSampleMessage];
    MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
    NSLog(@"%@", requestBuilder);
    MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
    [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
        if(!error){
            NSLog(@"response %@", response);
             dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                self.descriptionLabel.text = @"Check your inbox. You have a new message :)";
            });
        }
        else {
            dispatch_async(dispatch_get_main_queue(), ^{
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
            });
        }
    }];
   }
   ```



## <a name="run-the-app"></a><span data-ttu-id="e893d-184">运行应用</span><span class="sxs-lookup"><span data-stu-id="e893d-184">Run the app</span></span>
1. <span data-ttu-id="e893d-p121">运行示例前需要提供在“**注册应用**”部分的注册过程中收到的客户端 ID。打开“**应用程序**”文件夹下的 **AuthenticationConstants.m**。你会发现，注册过程中的 ClientID 可以被添加到文件顶部：</span><span class="sxs-lookup"><span data-stu-id="e893d-p121">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

><span data-ttu-id="e893d-p122">注意：你会注意到为该项目配置了以下权限范围：**“https://graph.microsoft.com/Mail.Send”、“https://graph.microsoft.com/User.Read”和“offline_access”**。如果此项目中使用的服务调用要向你的邮件帐户发送邮件并检索一些个人资料信息（显示名称、电子邮件地址），则需要这些应用权限才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="e893d-p122">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="e893d-190">运行示例，点击“**连接**”，使用你的个人帐户、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="e893d-190">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="e893d-p123">选择“**发送电子邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="e893d-p123">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e893d-193">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e893d-193">Next steps</span></span>
- <span data-ttu-id="e893d-194">使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="e893d-194">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="e893d-195">可在 [Microsoft Graph iOS Objective C 代码段示例](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample) 中找到 REST 和 SDK 操作的常见操作示例。</span><span class="sxs-lookup"><span data-stu-id="e893d-195">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="e893d-196">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e893d-196">See also</span></span>
- [<span data-ttu-id="e893d-197">适用于 iOS 的 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="e893d-197">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="e893d-198">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="e893d-198">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="e893d-199">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="e893d-199">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
