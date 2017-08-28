# <a name="get-started-with-microsoft-graph-in-an-ios-app"></a><span data-ttu-id="9ac20-101">在 iOS 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9ac20-101">Get started with Microsoft Graph in an iOS App</span></span>

> <span data-ttu-id="9ac20-p101">**为企业客户生成应用？**如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="9ac20-p102">若要在**所有企业方案**中支持**所有企业客户**，必须使用 Azure AD 终结点并使用 [Azure 管理门户](https://aka.ms/aadapplist)管理应用。有关详细信息，请参阅 [在 Azure AD 和 Azure AD v2.0 终结点之间进行选择](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="9ac20-p103">本文介绍了从 [Azure AD v2.0 终结点](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) 获取访问令牌和调用 Microsoft Graph 所需的任务。本文演示了 [适用于 iOS 的 Office 365 Connect 示例 (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) 中的代码，以说明你在使用 Microsoft Graph 的应用中必须实现的主要概念。本文介绍了如何通过使用 [适用于 iOS 的Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios) 来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="9ac20-110">可以在以下 GitHub 存储库中下载要创建的应用版本：</span><span class="sxs-lookup"><span data-stu-id="9ac20-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="9ac20-111">使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例</span><span class="sxs-lookup"><span data-stu-id="9ac20-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="9ac20-112">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="9ac20-112">The following image shows the app you'll create.</span></span>

![Connect 示例演练演示了在应用中进行连接和发送邮件](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="9ac20-114">将工作流连接到 Microsoft Graph 并进行身份验证，通过工作或个人帐户登录，最后向收件人发送邮件。</span><span class="sxs-lookup"><span data-stu-id="9ac20-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="9ac20-p104">**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/en-us/getting-started) 快速准备就绪并开始运行。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac20-117">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ac20-117">Prerequisites</span></span>

<span data-ttu-id="9ac20-118">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="9ac20-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="9ac20-119">Apple 的 [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="9ac20-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="9ac20-120">安装 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) 作为依存关系管理器。</span><span class="sxs-lookup"><span data-stu-id="9ac20-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="9ac20-121">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="9ac20-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="9ac20-p105">[适用于 iOS 的 Microsoft Graph 初学者项目](https://github.com/microsoftgraph/ios-objectivec-connect-sample)本模板包含可向其添加代码的类。若要获取此项目，请在此位置克隆或下载示例项目，然后可以使用 **starter-project** 文件夹中的工作区 (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**)。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p105">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample). This template contains classes that you'll add code to. To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="9ac20-125">注册应用</span><span class="sxs-lookup"><span data-stu-id="9ac20-125">Register the app</span></span>
 
1. <span data-ttu-id="9ac20-126">使用个人或工作或学校帐户登录到 [应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="9ac20-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="9ac20-127">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="9ac20-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="9ac20-128">为应用输入名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="9ac20-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="9ac20-129">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="9ac20-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="9ac20-130">在“**平台**”下，选择“**添加平台**”。</span><span class="sxs-lookup"><span data-stu-id="9ac20-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="9ac20-131">选择“**移动平台**”。</span><span class="sxs-lookup"><span data-stu-id="9ac20-131">Select **Mobile platform**.</span></span>
6. <span data-ttu-id="9ac20-p106">将客户端 ID 复制到剪贴板。将需要在示例应用中输入该值。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="9ac20-134">应用 ID 是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9ac20-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="9ac20-135">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="9ac20-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="9ac20-136">导入项目依赖项</span><span class="sxs-lookup"><span data-stu-id="9ac20-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="9ac20-p107">克隆该存储库，[使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例](https://github.com/microsoftgraph/ios-objectivec-connect-sample)。**请记住要使用的是 starter-project 文件夹中的示例，而不是项目根目录中的示例。**</span><span class="sxs-lookup"><span data-stu-id="9ac20-p107">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample). **Remember you will use the sample in the starter-project folder and not the sample at the root of the project.**</span></span>
2. <span data-ttu-id="9ac20-p108">使用 CocoaPods 导入 Microsoft Graph SDK 和身份验证依赖项。该示例应用已包含可将 pod 导入到项目中的 pod 文件。导航至“**终端**”应用中的“**starter-project**”文件夹，然后在“**终端**”中运行：</span><span class="sxs-lookup"><span data-stu-id="9ac20-p108">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="9ac20-p109">将收到已将 pod 导入到项目的确认消息。有关详细信息，请参阅 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="9ac20-p109">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="9ac20-144">启用密钥链共享</span><span class="sxs-lookup"><span data-stu-id="9ac20-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="9ac20-p110">对于 Xcode 8，将需要添加密钥链组，否则应用将无法访问密钥链。添加密钥链组：</span><span class="sxs-lookup"><span data-stu-id="9ac20-p110">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="9ac20-p111">在 Xcode 项目管理器面板上选择项目。(⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p111">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="9ac20-149">选择“**O365-iOS-Microsoft-Graph-SDK**”。</span><span class="sxs-lookup"><span data-stu-id="9ac20-149">Select **O365-iOS-Microsoft-Graph-SDK**.</span></span>
 
3. <span data-ttu-id="9ac20-150">在“功能”选项卡上启用**密钥链共享**。</span><span class="sxs-lookup"><span data-stu-id="9ac20-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="9ac20-151">将 **com.microsoft.O365-iOS-Microsoft-Graph-SDK** 添加到密钥链组。</span><span class="sxs-lookup"><span data-stu-id="9ac20-151">Add **com.microsoft.O365-iOS-Microsoft-Graph-SDK** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="9ac20-152">使用 Microsoft Graph 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="9ac20-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="9ac20-p112">若要重新访问 UI 工作流，应用需要验证用户身份，然后他们就可以向特定用户发送邮件。若要生成对 Microsoft Graph 服务的请求，必须提供身份验证提供程序（它能够使用适当的 OAuth 2.0 持有者令牌对 HTTPS 请求进行身份验证）。在示例项目中，具有已作为存根的名为 **AuthenticationProvider.m** 的身份验证类。我们将向请求添加一个函数，然后获取一个调用 Microsoft Graph API 的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p112">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="9ac20-p113">打开“**starter-project**”文件夹中的 Xcode 项目工作区 (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**)，然后导航至“**身份验证**”文件夹并打开文件 **AuthenticationProvider.m**。将下列代码添加至该类。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p113">Open the Xcode project workspace (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.** Add the following code to that class.</span></span>

        -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)   (NSError *))completion{
            [NXOAuth2AuthenticationProvider setClientId:kClientId
                                              scopes:scopes];
    
    
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

2. <span data-ttu-id="9ac20-p114">接下来，将此方法添加至头文件。打开文件 **AuthenticationProvider.h**，然后将下列代码添加至此类。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p114">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>

        -(void) connectToGraphWithClientId:(NSString *)clientId
                            scopes:(NSArray *)scopes
                        completion:(void (^)(NSError *error))completion;



2. <span data-ttu-id="9ac20-p115">最后，我们将从 **ConnectViewController.m** 中调用此方法。该控制器是应用加载的默认视图，其中存在名称为“**连接**”的单个按钮，用户将点按此按钮启动身份验证流程。此方法采用两个参数，即 **Client ID** 和 **scopes**，我们将在后续部分详细介绍它们。将以下操作添加到 **ConnectViewController.m**。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p115">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

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

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="9ac20-165">使用 Microsoft Graph 发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="9ac20-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="9ac20-p116">将项目配置为可以进行身份验证后，下一项任务则是使用 Microsoft Graph API 向用户发送邮件。默认情况下，将已登录用户视作收件人，但是可以将其更改为其他任何收件人。我们在此处要使用的代码位于“**控制器**”文件夹和 **SendMailViewController.m** 类中。将看到在此处展示了用于 UI 的其他代码，还有一个用来从 Microsoft Graph 服务检索用户个人资料信息的 Helper 方法。我们将着重介绍创建邮件并发送邮件的方法。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p116">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="9ac20-p117">打开“控制器”文件夹中的 **SendMailViewController.m**，然后将下列 Helper 方法添加到类中：</span><span class="sxs-lookup"><span data-stu-id="9ac20-p117">Open **SendMailViewController.m.** in the Controllers folder and add the following helper method to the class:</span></span>

        // Create a sample test message to send to specified user account
        -(MSGraphMessage*) getSampleMessage{
            MSGraphMessage *message = [[MSGraphMessage alloc]init];
            MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
            MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
            email.address = self.emailAddress;
            toRecipient.emailAddress = email;
    
            NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
            [toRecipients addObject:toRecipient];
    
            message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
            MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
            NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
            NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
            emailBody.content = htmlContentString;
            emailBody.contentType = [MSGraphBodyType html];
            message.body = emailBody;
    
            message.toRecipients = toRecipients;
    
            return message;
    
        }


2. <span data-ttu-id="9ac20-p118">打开 **SendMailViewController.m。**将以下发送邮件方法添加到类中。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p118">Open **SendMailViewController.m.** Add the following send mail method to the class.</span></span>  

        //Send mail to the specified user in the email text field
        -(void) sendMail {   
            MSGraphMessage *message = [self getSampleMessage];
            MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
            NSLog(@"%@", requestBuilder);
            MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
            [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
                if(!error){
                    NSLog(@"response %@", response);
                    NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            
                    dispatch_async(dispatch_get_main_queue(), ^{
                        self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                });
            }
            else {
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
                }
            }];
    
        }

<span data-ttu-id="9ac20-p119">由此 **getSampleMessage** 将创建 HTML 示例邮件草稿以用于演示目的。下一个方法 **sendMail** 将获取该邮件，然后执行该请求以将其发送出去。同样，默认收件人为登录用户。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p119">So **getSampleMessage** creates a draft HTML sample mail to use for demo purposes. The next method, **sendMail**, then takes that message and executes the request to send it. Again the default recipient is the signed-in user.</span></span>


## <a name="run-the-app"></a><span data-ttu-id="9ac20-178">运行应用</span><span class="sxs-lookup"><span data-stu-id="9ac20-178">Run the app</span></span>
1. <span data-ttu-id="9ac20-p120">运行示例前需要提供在“**注册应用**”部分的注册过程中收到的客户端 ID。打开“**应用程序**”文件夹下的 **AuthenticationConstants.m**。你会发现，注册过程中的 ClientID 可以被添加到文件顶部：</span><span class="sxs-lookup"><span data-stu-id="9ac20-p120">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  

        // You will set your application's clientId
        NSString * const kClientId    = @"ENTER_CLIENT_ID_HERE";
        NSString * const kScopes = @"https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/User.Read, offline_access";
<span data-ttu-id="9ac20-p121">注意：你会注意到为该项目配置了以下权限范围：**https://graph.microsoft.com/Mail.Send”、 “https://graph.microsoft.com/User.Read”、 “offline_access”**。该项目中所使用的服务调用，向你的邮件帐户发送邮件并检索一些个人资料信息（显示名称、电子邮件地址）需要这些应用的权限以正常运行。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p121">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="9ac20-184">运行示例，点击“**连接**”，使用你的个人帐户、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="9ac20-184">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="9ac20-p122">选择“**发送电子邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="9ac20-p122">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9ac20-187">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9ac20-187">Next steps</span></span>
- <span data-ttu-id="9ac20-188">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="9ac20-188">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="9ac20-189">可在 [Microsoft Graph iOS Objective C 代码段示例](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample) 中找到 REST 和 SDK 操作的常见操作示例。</span><span class="sxs-lookup"><span data-stu-id="9ac20-189">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="9ac20-190">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9ac20-190">See also</span></span>
- [<span data-ttu-id="9ac20-191">适用于 iOS 的 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="9ac20-191">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="9ac20-192">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="9ac20-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="9ac20-193">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="9ac20-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
