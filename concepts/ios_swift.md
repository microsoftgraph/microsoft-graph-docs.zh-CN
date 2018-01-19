# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="1fd00-101">在 Swift iOS 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1fd00-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="1fd00-p101">**为企业客户生成应用？**如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="1fd00-p102">若要跨**所有企业方案**支持**全部企业客户**，必须使用 Azure AD 终结点，并使用 [Azure 门户](https://aka.ms/aadapplist)管理应用。有关详细信息，请参阅[在 Azure AD 和 Azure AD v2.0 终结点之间进行选择](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="1fd00-p103">本文介绍了从 [Azure AD v2.0 终结点](https://developer.microsoft.com/zh-CN/graph/docs/concepts/converged_auth) 获取访问令牌和调用 Microsoft Graph 所需的任务。本文演示了 [适用于 iOS 的 Office 365 Connect 示例 (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) 中的代码，以说明你在使用 Microsoft Graph 的应用中必须实现的主要概念。本文介绍了如何通过使用 [适用于 iOS 的Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-ios) 来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/zh-CN/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="1fd00-110">可以在以下 GitHub 存储库中下载要创建的应用版本：</span><span class="sxs-lookup"><span data-stu-id="1fd00-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="1fd00-111">使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例</span><span class="sxs-lookup"><span data-stu-id="1fd00-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="1fd00-112">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="1fd00-112">The following image shows the app you'll create.</span></span>

![Connect 示例演练演示了在应用中进行连接和发送邮件](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="1fd00-114">将工作流连接到 Microsoft Graph 并进行身份验证，通过工作或个人帐户登录，最后向收件人发送邮件。</span><span class="sxs-lookup"><span data-stu-id="1fd00-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="1fd00-p104">**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/zh-CN/getting-started) 快速准备就绪并开始运行。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/zh-CN/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fd00-117">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fd00-117">Prerequisites</span></span>

<span data-ttu-id="1fd00-118">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="1fd00-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="1fd00-119">Apple 的 [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="1fd00-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="1fd00-120">安装 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) 作为依存关系管理器。</span><span class="sxs-lookup"><span data-stu-id="1fd00-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="1fd00-121">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="1fd00-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="1fd00-122">[适用于 iOS 的 Microsoft Graph 初学者项目](https://github.com/microsoftgraph/ios-objectivec-connect-sample)</span><span class="sxs-lookup"><span data-stu-id="1fd00-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="1fd00-123">本模板包含可向其添加代码的类。</span><span class="sxs-lookup"><span data-stu-id="1fd00-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="1fd00-124">若要获取此项目，请在此位置克隆或下载示例项目，然后可以使用 **starter-project** 文件夹中的工作区 (**ios-objectivec-connect-sample.xcworkspace**)。</span><span class="sxs-lookup"><span data-stu-id="1fd00-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="1fd00-125">注册应用</span><span class="sxs-lookup"><span data-stu-id="1fd00-125">Register the app</span></span>
 
1. <span data-ttu-id="1fd00-126">使用个人或工作或学校帐户登录到 [应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="1fd00-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="1fd00-127">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="1fd00-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="1fd00-128">为应用输入名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="1fd00-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="1fd00-129">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="1fd00-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="1fd00-130">在“平台”****下，选择“添加平台”****。</span><span class="sxs-lookup"><span data-stu-id="1fd00-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="1fd00-131">选择“本机平台”****。</span><span class="sxs-lookup"><span data-stu-id="1fd00-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="1fd00-p106">将客户端 ID 复制到剪贴板。将需要在示例应用中输入该值。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="1fd00-134">应用 ID 是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1fd00-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="1fd00-135">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="1fd00-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="1fd00-136">导入项目依赖项</span><span class="sxs-lookup"><span data-stu-id="1fd00-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="1fd00-137">克隆该存储库，[使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例](https://github.com/microsoftgraph/ios-objectivec-connect-sample)。</span><span class="sxs-lookup"><span data-stu-id="1fd00-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="1fd00-138">重要说明：使用的是 starter-project 文件夹中的示例，而不是项目根目录中的示例。</span><span class="sxs-lookup"><span data-stu-id="1fd00-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="1fd00-p107">使用 CocoaPods 导入 Microsoft Graph SDK 和身份验证依赖项。该示例应用已包含可将 pod 导入到项目中的 pod 文件。导航至“**终端**”应用中的“**starter-project**”文件夹，然后在“**终端**”中运行：</span><span class="sxs-lookup"><span data-stu-id="1fd00-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="1fd00-p108">将收到已将 pod 导入到项目的确认消息。有关详细信息，请参阅 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="1fd00-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="1fd00-144">启用密钥链共享</span><span class="sxs-lookup"><span data-stu-id="1fd00-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="1fd00-p109">对于 Xcode 8，将需要添加密钥链组，否则应用将无法访问密钥链。添加密钥链组：</span><span class="sxs-lookup"><span data-stu-id="1fd00-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="1fd00-p110">在 Xcode 项目管理器面板上选择项目。(⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="1fd00-149">选择“iOS-ObjectiveC-Connect-Sample”****。</span><span class="sxs-lookup"><span data-stu-id="1fd00-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="1fd00-150">在“功能”选项卡上启用“密钥链共享”****。</span><span class="sxs-lookup"><span data-stu-id="1fd00-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="1fd00-151">将 **com.microsoft.ios-objectivec-connect-sample** 添加到钥匙链组。</span><span class="sxs-lookup"><span data-stu-id="1fd00-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="1fd00-152">使用 Microsoft Graph 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="1fd00-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="1fd00-153">若要重新访问 UI 工作流，应用需要验证用户身份，然后他们就可以向特定用户发送邮件。</span><span class="sxs-lookup"><span data-stu-id="1fd00-153">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user.</span></span> <span data-ttu-id="1fd00-154">若要生成对 Microsoft Graph 服务的请求，必须提供身份验证提供程序（它能够使用适当的 OAuth 2.0 持有者令牌对 HTTPS 请求进行身份验证）。</span><span class="sxs-lookup"><span data-stu-id="1fd00-154">To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="1fd00-155">在示例项目中，具有已作为存根的名为 **Authentication.swift** 的身份验证结构。</span><span class="sxs-lookup"><span data-stu-id="1fd00-155">In the sample project there's an authentication structure already stubbed out called **Authentication.swift.**</span></span> <span data-ttu-id="1fd00-156">我们将向请求添加一个函数，然后获取一个调用 Microsoft Graph API 的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="1fd00-156">We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="1fd00-157">打开 Xcode 项目工作区 (**Graph-iOS-Swift-Connect.xcworkspace**)，然后打开结构扩展文件 **Authentication.swift**。在该扩展中找到以下代码。</span><span class="sxs-lookup"><span data-stu-id="1fd00-157">Open the Xcode project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the structure extension file **Authentication.swift** Find the following code in that extension.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph. 
     If a user has previously signed in before and not disconnected, silent log in
     will take place. 
     If not, authentication will ask for credentials
     */
    func connectToGraph(withClientId clientId: String,
                                     scopes: [String],
                                     completion:@escaping (_ error: MSGraphError?) -> Void) {
    
        // Set client ID
        NXOAuth2AuthenticationProvider.setClientId(clientId, scopes: scopes)
        
        // Try silent log in. This will attempt to sign in if there is a previous successful
        // sign in user information.
        if NXOAuth2AuthenticationProvider.sharedAuth().loginSilent() == true {
            completion(nil)
        }
        // Otherwise, present log in controller.
        else {
            NXOAuth2AuthenticationProvider.sharedAuth()
                .login(with: nil) { (error: Error?) in
                    
                    if let nserror = error {
                        completion(MSGraphError.nsErrorType(error: nserror as NSError))
                    }
                    else {
                        completion(nil)
                    }
            }
        }
    }
  ```


2. <span data-ttu-id="1fd00-158">我们将从 **ConnectViewController.swift** 中调用此方法。</span><span class="sxs-lookup"><span data-stu-id="1fd00-158">We'll call this method from **ConnectViewController.swift**.</span></span> <span data-ttu-id="1fd00-159">此控制器是应用加载的默认视图，其中存在名称为“连接”****的单个按钮，用户将点击此按钮启动身份验证过程。</span><span class="sxs-lookup"><span data-stu-id="1fd00-159">This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process.</span></span> <span data-ttu-id="1fd00-160">此方法采用一个参数 **scopes**，我们将在下面讨论有关 scopes 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1fd00-160">This method takes in one parameter, the **scopes**, we'll discuss scopes in more detail below.</span></span> <span data-ttu-id="1fd00-161">将以下操作添加到 **ConnectViewController.swift**。</span><span class="sxs-lookup"><span data-stu-id="1fd00-161">Add the following action to **ConnectViewController.swift**.</span></span>

  ```swift
  // MARK: Authentication
  private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        
        let clientId = ApplicationConstants.clientId
        let scopes = ApplicationConstants.scopes
        
        authentication.connectToGraph(withClientId: clientId, scopes: scopes) {
            (error) in
            
            defer {self.loadingUI(show: false)}
            
            if let graphError = error {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
            }
            else {
                self.performSegue(withIdentifier: "showSendMail", sender: nil)
            }
        }
    }
  }

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="1fd00-162">使用 Microsoft Graph 发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="1fd00-162">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="1fd00-163">将项目配置为能够进行身份验证后，下一个任务是获取已经过身份验证的用户的电子邮件地址、显示名称和个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="1fd00-163">After configuring the project to be able to authenticate, the next tasks are getting the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="1fd00-164">示例在获取这些值后将向 OneDrive 上传个人资料图片，并获取图片的共享 URL。</span><span class="sxs-lookup"><span data-stu-id="1fd00-164">After the sample gets these values it uploads the profile picture to OneDrive and gets the sharing Url of the picture.</span></span> <span data-ttu-id="1fd00-165">最后，它向使用 Microsoft Graph API 的用户发送一封邮件。</span><span class="sxs-lookup"><span data-stu-id="1fd00-165">Finally, it sends a mail to a user using the Microsoft Graph API.</span></span> 

<span data-ttu-id="1fd00-166">默认情况下，将已登录用户视作收件人，但是可以将其更改为其他任何收件人。</span><span class="sxs-lookup"><span data-stu-id="1fd00-166">By default the logged in user will be the recipient, but you have the ability to change it to any other recipient.</span></span> <span data-ttu-id="1fd00-167">我们将在此处使用的代码位于 **SendMailViewController.swift** 类中。</span><span class="sxs-lookup"><span data-stu-id="1fd00-167">The code we'll work with here is in the class **SendMailViewController.swift.**</span></span> <span data-ttu-id="1fd00-168">可以看到，在此处展示了用于 UI 的其他代码，还有一个用来从 Microsoft Graph 服务检索用户个人资料信息的 Helper 方法。</span><span class="sxs-lookup"><span data-stu-id="1fd00-168">You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service.</span></span> <span data-ttu-id="1fd00-169">我们将着重介绍创建邮件并发送邮件的方法。</span><span class="sxs-lookup"><span data-stu-id="1fd00-169">We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="1fd00-170">打开 **SendMailViewController.swift**</span><span class="sxs-lookup"><span data-stu-id="1fd00-170">Open **SendMailViewController.swift.**</span></span>  <span data-ttu-id="1fd00-171">并在该类中查找可创建 Helper 方法的邮件正文：</span><span class="sxs-lookup"><span data-stu-id="1fd00-171">and find the mail body creating helper method in the class:</span></span>

  ```swift
    /**
     Creates sample email message
     
     - parameter emailAddress: recipient email address
     
     - returns: MSGraphMessage object with given recipient. The body is created from EmailBody.html
     */
    func createSampleMessage(to emailAddress: String, picLink pictureUrl: String) -> MSGraphMessage? {
        let message = MSGraphMessage()
        
        // set recipients
        
        let _ = self.userPicture
        let toRecipient = MSGraphRecipient()
        let msEmailAddress = MSGraphEmailAddress()
        msEmailAddress.address = emailAddress
        toRecipient.emailAddress = msEmailAddress
        let toRecipientList = [toRecipient]
        message.toRecipients = toRecipientList
        message.subject = NSLocalizedString("MAIL_SUBJECT", comment: "")
        let messageBody = MSGraphItemBody()
        messageBody.contentType = MSGraphBodyType.html()
        guard let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html") else {return nil}
        messageBody.content = try! String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
        messageBody.content = messageBody.content.replacingOccurrences(of: "a href=%s", with: ("a href=" + pictureUrl))
        message.body = messageBody

        if let unwrappedImage = self.userPicture {
            let fileAttachment = MSGraphFileAttachment()
            let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
            fileAttachment.contentType = "image/png"
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment"
            fileAttachment.contentBytes = data?.base64EncodedString()
            fileAttachment.name = "me.png"
            message.attachments.append(fileAttachment)
        }
        return message
    }

  ```
2. <span data-ttu-id="1fd00-172">查找以下 Helper 方法，以获取用户信息、获取个人资料照片并将照片上传到 OneDrive：</span><span class="sxs-lookup"><span data-stu-id="1fd00-172">find the following helper methods for getting user information, getting a profile photograph, and uploading the photograph to OneDrive:</span></span>

  ```swift
      /**
     Fetches user information such as mail and display name
     */
    func getUserInfo() {
        self.sendButton.isEnabled = false
        self.statusTextView.text = NSLocalizedString("LOADING_USER_INFO", comment: "")
        
        self.graphClient.me().request().getWithCompletion {
            (user: MSGraphUser?, error: Error?) in
            if let graphError = error {
                print(NSLocalizedString("ERROR", comment: ""), graphError)
                DispatchQueue.main.async(execute: {
                    self.statusTextView.text = NSLocalizedString("GRAPH_ERROR", comment: "")
                })
            }
            else {
                guard let userInfo = user else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_FAILURE", comment: "")
                    })
                    return
                }
                DispatchQueue.main.async(execute: {
                    self.emailTextField.text = userInfo.mail
                    
                    if let displayName = userInfo.displayName {
                        self.headerLabel.text = "Hi " + displayName
                    }
                    else {
                        self.headerLabel.text = NSString(format: NSLocalizedString("HI_USER", comment: "") as NSString, "") as String
                    }
                    
                    self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_SUCCESS", comment: "")
                    self.sendButton.isEnabled = true
                })
            }
        }
    }
    
    /**
     Uploads the user's profile picture (obtained via the Graph API) to the user's OneDrive drive. The OneDrive sharing url is
     returned in the completion handler.
    */
    func uploadPictureToOneDrive(uploadFile image: UIImage?, with completion: @escaping (_ result: GraphResult<String, NSError>) ->Void) {
        
        var webUrl: String = ""
        guard let unwrappedImage = image else {
            return
        }
        let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
        self.graphClient
            .me()
            .drive()
            .root()
            .children()
            .driveItem("me.png")
            .contentRequest()
            .upload(from: data, completion: {
                (driveItem: MSGraphDriveItem?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("UPLOAD_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return

                } else {
                    webUrl = (driveItem?.webUrl)!
                    completion(.success(webUrl))
                }
            })
    }


    /**
     Gets the user's profile picture. Returns the picture as a UIImage via completion handler
    */
    func getUserPicture(forUser upn: String, with completion: @escaping (_ result: GraphResult<UIImage, NSError>) -> Void) {
        
        //Asynchronous Graph call. Closure is invoked after getUserPicture completes. Requires @escaping attribute
        self.graphClient.me().photoValue().download {
            (url: URL?, response: URLResponse?, error: Error?) in
            
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return
                }
                guard let picUrl = url else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "User profile picture is nil")
                    })
                    return
                }
                print(picUrl)
            
                let picData = NSData(contentsOf: picUrl)
                let picImage = UIImage(data: picData! as Data)
            
                if let validPic = picImage {
                    completion(.success(validPic))
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "Picture data is invalid")
                    })
                }
            }
    }

  ```

3. <span data-ttu-id="1fd00-173">在类中查找以下发送邮件方法。</span><span class="sxs-lookup"><span data-stu-id="1fd00-173">Find the following send mail method in the class.</span></span>  

  ```swift
    @IBAction func sendMail(_ sender: AnyObject) {
        guard let toEmail = self.emailTextField.text else {return}
        guard let picUrl = self.userPictureUrl else {return}
        if let message = self.createSampleMessage(to: toEmail, picLink: picUrl) {
            
            let requestBuilder = graphClient.me().sendMail(with: message, saveToSentItems: false)
            let mailRequest = requestBuilder?.request()
            
            _ = mailRequest?.execute(completion: {
                (response: [AnyHashable: Any]?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("SEND_FAILURE", comment: "")
                    })
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.descriptionLabel.text = "Check your inbox. You have a new message :)"
                        self.statusTextView.text = NSLocalizedString("SEND_SUCCESS", comment: "")
                    })
                }
            })
        }
    }

  ```


## <a name="run-the-app"></a><span data-ttu-id="1fd00-174">运行应用</span><span class="sxs-lookup"><span data-stu-id="1fd00-174">Run the app</span></span>
1. <span data-ttu-id="1fd00-175">运行示例前需要提供在“**注册应用**”部分的注册过程中收到的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="1fd00-175">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="1fd00-176">打开 **ApplicationConstants.swift**。</span><span class="sxs-lookup"><span data-stu-id="1fd00-176">Open **ApplicationConstants.swift** .</span></span> <span data-ttu-id="1fd00-177">你会发现，注册过程中的 ClientID 可以被添加到文件顶部：</span><span class="sxs-lookup"><span data-stu-id="1fd00-177">You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  

  ```swift
struct ApplicationConstants {
    static let clientId = "Enter_Client_Id_Here"
    static let scopes   = ["openid", "profile", "Mail.ReadWrite","mail.send","Files.ReadWrite","User.ReadBasic.All"]
}


  ```

> <span data-ttu-id="1fd00-p117">注意：你会注意到为该项目配置了以下权限范围：**https://graph.microsoft.com/Mail.Send”、 “https://graph.microsoft.com/User.Read”、 “offline_access”**。该项目中所使用的服务调用，向你的邮件帐户发送邮件并检索一些个人资料信息（显示名称、电子邮件地址）需要这些应用的权限以正常运行。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p117">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="1fd00-180">运行示例，点击“**连接**”，使用你的个人帐户、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="1fd00-180">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="1fd00-p118">选择“**发送电子邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="1fd00-p118">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1fd00-183">后续步骤</span><span class="sxs-lookup"><span data-stu-id="1fd00-183">Next steps</span></span>
- <span data-ttu-id="1fd00-184">使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="1fd00-184">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="1fd00-185">可在 [Microsoft Graph iOS Objective C 代码段示例](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample) 中找到 REST 和 SDK 操作的常见操作示例。</span><span class="sxs-lookup"><span data-stu-id="1fd00-185">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="1fd00-186">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1fd00-186">See also</span></span>
- [<span data-ttu-id="1fd00-187">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="1fd00-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="1fd00-188">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="1fd00-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-tokens/)
