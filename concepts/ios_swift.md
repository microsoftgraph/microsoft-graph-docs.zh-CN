# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="bdd58-101">在 Swift iOS 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bdd58-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="bdd58-p101">**为企业客户生成应用？** 如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。</span><span class="sxs-lookup"><span data-stu-id="bdd58-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="bdd58-p102">若要跨**所有企业方案**支持**全部企业客户**，必须使用 Azure AD 终结点，并使用 [Azure 门户](https://aka.ms/aadapplist)管理应用。有关详细信息，请参阅[在 Azure AD 和 Azure AD v2.0 终结点之间进行选择](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="bdd58-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="bdd58-p103">本文介绍了从 [Azure AD v2.0 终结点](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth)获取访问令牌和调用 Microsoft Graph 所需的任务。本文通过演示[适用于 iOS 的 Office 365 Connect 示例 (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) 中的代码，以说明你在使用 Microsoft Graph 的应用中实现的主要概念。本文介绍了如何通过使用异步 **Promise chain** 模式来访问 Microsoft Graph。示例中的 Promises 是通过使用 [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPod 来实现的。</span><span class="sxs-lookup"><span data-stu-id="bdd58-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) to explain the main concepts that you implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using REST operations in an asynchronous **Promise chain** pattern.  Promises in the sample are implemented by using the [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPod.</span></span> 

<span data-ttu-id="bdd58-111">示例是使用 **XCode 9.2** 和 **Swift 3.2** 创建的。</span><span class="sxs-lookup"><span data-stu-id="bdd58-111">The sample was created using **XCode 9.2** and **Swift 3.2**.</span></span>

<span data-ttu-id="bdd58-112">你可以在以下 GitHub 存储库中下载要创建的应用版本：</span><span class="sxs-lookup"><span data-stu-id="bdd58-112">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="bdd58-113">使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例</span><span class="sxs-lookup"><span data-stu-id="bdd58-113">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

<span data-ttu-id="bdd58-114">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="bdd58-114">The following image shows the app you'll create.</span></span>

![通过 Connect 示例演练，说明如何在应用中进行连接和发送邮件](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="bdd58-116">工作流对访问 Microsoft Graph 资源的示例进行身份验证和授权，使用工作或个人帐户登录，最后向收件人发送邮件。</span><span class="sxs-lookup"><span data-stu-id="bdd58-116">The workflow authenticates and authorizes the sample to access  Microsoft Graph resources, signs in with your work or personal account, and finally sends a mail to a recipient.</span></span>

<span data-ttu-id="bdd58-p104">**不想生成一个应用？那就使用 [Microsoft Graph 快速入门](https://developer.microsoft.com/en-us/graph/quick-start)快速准备就绪并开始运行吧。**</span><span class="sxs-lookup"><span data-stu-id="bdd58-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/en-us/graph/quick-start) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdd58-119">先决条件</span><span class="sxs-lookup"><span data-stu-id="bdd58-119">Prerequisites</span></span>

<span data-ttu-id="bdd58-120">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="bdd58-120">To get started, you'll need:</span></span> 

* <span data-ttu-id="bdd58-121">Apple 的 [Xcode](https://developer.apple.com/xcode/downloads/)</span><span class="sxs-lookup"><span data-stu-id="bdd58-121">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="bdd58-122">安装 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) 作为依赖关系管理器。</span><span class="sxs-lookup"><span data-stu-id="bdd58-122">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="bdd58-123">安装 [Carthage](https://github.com/Carthage/Carthage) 以导入和生成 **MSAL** 库。</span><span class="sxs-lookup"><span data-stu-id="bdd58-123">Installation of [Carthage](https://github.com/Carthage/Carthage) to import and build the **MSAL** library.</span></span>
* <span data-ttu-id="bdd58-124">安装 [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod。</span><span class="sxs-lookup"><span data-stu-id="bdd58-124">Installation of the [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod.</span></span> 
* <span data-ttu-id="bdd58-125">一个 [Microsoft 帐户](https://www.outlook.com/)或者一个[工作或学校帐户](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="bdd58-125">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>

## <a name="register-the-app"></a><span data-ttu-id="bdd58-126">注册应用</span><span class="sxs-lookup"><span data-stu-id="bdd58-126">Register the app</span></span>
 
1. <span data-ttu-id="bdd58-127">使用个人或工作或学校帐户登录到[应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="bdd58-127">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="bdd58-128">选择“添加应用”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="bdd58-128">Select **Add an app**.</span></span>
3. <span data-ttu-id="bdd58-129">为应用输入名称，并选择“创建应用程序”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="bdd58-129">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="bdd58-130">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="bdd58-130">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="bdd58-131">在“平台”\*\*\*\* 下，选择“添加平台”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="bdd58-131">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="bdd58-132">选择“本机平台”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="bdd58-132">Select **Native platform**.</span></span>
6. <span data-ttu-id="bdd58-p105">将客户端 ID 复制到剪贴板。将需要在示例应用中输入该值。</span><span class="sxs-lookup"><span data-stu-id="bdd58-p105">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="bdd58-135">应用 ID 是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bdd58-135">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="bdd58-136">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="bdd58-136">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="bdd58-137">导入项目依赖项</span><span class="sxs-lookup"><span data-stu-id="bdd58-137">Importing the project dependencies</span></span>

1. <span data-ttu-id="bdd58-138">克隆该存储库，[使用 Microsoft Graph SDK 的适用于 iOS 的 Office 365 Connect 示例](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="bdd58-138">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span></span> 


2. <span data-ttu-id="bdd58-139">使用 CocoaPods 导入 PromiseKit 依赖项。</span><span class="sxs-lookup"><span data-stu-id="bdd58-139">Use CocoaPods to import the PromiseKit dependencies.</span></span> <span data-ttu-id="bdd58-140">该示例应用已包含可将 pod 导入项目中的 Podfile。</span><span class="sxs-lookup"><span data-stu-id="bdd58-140">This sample app already contains a podfile that will get the pods into the project.</span></span> <span data-ttu-id="bdd58-141">导航至“终端”\*\*\*\* 应用中项目的根文件夹，然后从“终端”\*\*\*\* 中运行：</span><span class="sxs-lookup"><span data-stu-id="bdd58-141">Navigate to the root folder of the project in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="bdd58-p107">你会收到已将 Pod 导入到项目的确认消息。有关详细信息，请参阅 [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span><span class="sxs-lookup"><span data-stu-id="bdd58-p107">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>

## <a name="install-the-msal-authentication-framework"></a><span data-ttu-id="bdd58-144">安装 MSAL 身份验证框架</span><span class="sxs-lookup"><span data-stu-id="bdd58-144">Install the MSAL authentication framework</span></span>

<span data-ttu-id="bdd58-145">MSAL 预览版将作为使用 Carthage 的头文件和符号文件进行分发。</span><span class="sxs-lookup"><span data-stu-id="bdd58-145">The preview version of MSAL is distributed as header and symbol files using Carthage.</span></span> <span data-ttu-id="bdd58-146">若要在项目中安装 MSAL，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="bdd58-146">To install MSAL in the project, do these steps:</span></span>

1. <span data-ttu-id="bdd58-147">打开 Bash 终端并转到应用根文件夹。</span><span class="sxs-lookup"><span data-stu-id="bdd58-147">Open the Bash terminal and go to the app root folder.</span></span>
2. <span data-ttu-id="bdd58-148">创建 **cartfile**：将 `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` 复制到终端，并运行命令。</span><span class="sxs-lookup"><span data-stu-id="bdd58-148">Create a **cartfile**: Copy `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile`  into the terminal and run the command.</span></span>
3. <span data-ttu-id="bdd58-149">生成 MSAL 库：将 `carthage update` 复制到终端，并运行命令。</span><span class="sxs-lookup"><span data-stu-id="bdd58-149">Build the MSAL library: Copy `carthage update` into the terminal and run the command.</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="bdd58-150">启用密钥链共享</span><span class="sxs-lookup"><span data-stu-id="bdd58-150">Enable keychain sharing</span></span>
 
<span data-ttu-id="bdd58-p109">对于 Xcode 8，你需要添加密钥链组，否则应用将无法访问密钥链。如需添加密钥链组：</span><span class="sxs-lookup"><span data-stu-id="bdd58-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="bdd58-153">在 XCode 项目管理器面板上选择项目。</span><span class="sxs-lookup"><span data-stu-id="bdd58-153">Select the project on the project manager panel in XCode.</span></span> <span data-ttu-id="bdd58-154">(⌘ + 1)。</span><span class="sxs-lookup"><span data-stu-id="bdd58-154">(⌘ + 1).</span></span>
 
2. <span data-ttu-id="bdd58-155">选择 **O365-iOS-Microsoft-Graph-Connect-swift** 目标。</span><span class="sxs-lookup"><span data-stu-id="bdd58-155">Select the **O365-iOS-Microsoft-Graph-Connect-swift** target.</span></span>

3. <span data-ttu-id="bdd58-156">在“常规”\*\*\*\* 选项卡和“签名”\*\*\*\* 部分，验证已选中“自动管理签名”\*\*\*\* 并具有有效的签名证书。</span><span class="sxs-lookup"><span data-stu-id="bdd58-156">On the **General** tab and **Signing** section, verify that **Automatically manage signing** is checked and you have a valid signing certificate.</span></span>
 
3. <span data-ttu-id="bdd58-157">在“功能”\*\*\*\* 选项卡上启用“钥匙链共享”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="bdd58-157">On the **Capabilities** tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="bdd58-158">如果 **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** 未在钥匙链组的列表中，请添加它。</span><span class="sxs-lookup"><span data-stu-id="bdd58-158">If **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** is not in the list of Keychain Groups, add it.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="bdd58-159">使用 Microsoft Graph 进行身份验证</span><span class="sxs-lookup"><span data-stu-id="bdd58-159">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="bdd58-160">UI 工作流如下：应用要求用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="bdd58-160">The UI workflow is as follows: The app asks the user to authenticate.</span></span> <span data-ttu-id="bdd58-161">进行身份验证后，用户可以向其他用户发送邮件。</span><span class="sxs-lookup"><span data-stu-id="bdd58-161">After authentication, the user can send a mail to another user.</span></span> <span data-ttu-id="bdd58-162">若要向 Microsoft Graph 发出请求，该示例将使用 **MSAL** 身份验证库对含有相应 OAuth 2.0 持有者令牌的 HTTPS 请求进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="bdd58-162">To make requests against Microsoft Graph, the sample uses the **MSAL** authentication library to authenticate HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="bdd58-163">在示例项目 **AuthenticationClass.swift** 中，</span><span class="sxs-lookup"><span data-stu-id="bdd58-163">In the sample project the **AuthenticationClass.swift.**</span></span> <span data-ttu-id="bdd58-164">类导入 **MSAL** 库并获取 Microsoft Graph REST 操作所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="bdd58-164">class imports the **MSAL** library and acquires the access token needed for Microsoft Graph REST operations.</span></span>

1. <span data-ttu-id="bdd58-165">打开 **XCode** 项目工作区 (**Graph-iOS-Swift-Connect.xcworkspace**)，然后打开类文件 **AuthenticationClass.swift**。在该类中查找以下代码。</span><span class="sxs-lookup"><span data-stu-id="bdd58-165">Open the **XCode** project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the class file **AuthenticationClass.swift** Find the following code in that class.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph.
     If a user has previously signed in before and not disconnected, silent log in
     will take place.
     If not, authentication will ask for credentials
     */
    func connectToGraph(scopes: [String],
                        completion:@escaping (_ error: ApplicationConstants.MSGraphError?, _ accessToken: String) -> Bool)  {
        do {
            if let initError = self.lastInitError {
                if initError.lengthOfBytes(using: String.Encoding.ascii) > 1 {
                    throw NSError.init(domain: initError, code: 0, userInfo: nil)
                }
            }
            // We check to see if we have a current logged in user. If we don't, then we need to sign someone in.
            // We throw an interactionRequired so that we trigger the interactive signin.
            if  try authenticationProvider.users().isEmpty {
                throw NSError.init(domain: "MSALErrorDomain", code: MSALErrorCode.interactionRequired.rawValue, userInfo: nil)
            } else {
                // Acquire a token for an existing user silently
                try authenticationProvider.acquireTokenSilent(forScopes: scopes, user: authenticationProvider.users().first) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        _ = completion(nil, self.accessToken);
                    } else {
                        //"Could not acquire token silently: \(error ?? "No error information" as! Error )"
                       var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            }
        }  catch let error as NSError {
            // interactionRequired means we need to ask the user to sign-in. This usually happens
            // when the user's Refresh Token is expired or if the user has changed their password
            // among other possible reasons.
            if error.code == MSALErrorCode.interactionRequired.rawValue {
                authenticationProvider.acquireToken(forScopes: scopes) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        var _ = completion(nil, self.accessToken);
                    } else  {
                        var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            } else {
                var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);

            }
        } catch {
            // This is the catch all error.
            var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);
        }
    }

  ```


2. <span data-ttu-id="bdd58-166">我们将从 **ConnectViewController.swift** 中调用 **connectToGraph** 函数。</span><span class="sxs-lookup"><span data-stu-id="bdd58-166">We'll call the **connectToGraph** function from **ConnectViewController.swift**.</span></span> <span data-ttu-id="bdd58-167">此控制器是应用加载的默认视图，其中包含名称为“连接”\*\*\*\* 的单个按钮，用户点击此按钮即可启动身份验证过程。</span><span class="sxs-lookup"><span data-stu-id="bdd58-167">This controller is the default view that the app loads with a single button named **Connect** that the user taps to start authenticating.</span></span> 

  ```swift
// MARK: Authentication
private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        let scopes = ApplicationConstants.kScopes
        AuthenticationClass.sharedInstance?.connectToGraph( scopes: scopes) {
            (result: ApplicationConstants.MSGraphError?, accessToken: String) -> Bool  in
            defer {self.loadingUI(show: false)}
            if let graphError = result {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.userInfo)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
                return false
            }
            else {
                // run on main thread!!
                DispatchQueue.main.async {
                    self.performSegue(withIdentifier: "sendMail", sender: nil)
                }
                return true
            }
        }
    }
}

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="bdd58-168">使用 Microsoft Graph 发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="bdd58-168">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="bdd58-169">将用户连接到 Microsoft Graph 后，示例将获取经过身份验证的用户的电子邮件地址、显示名称和个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="bdd58-169">After connecting the user to Microsoft Graph, the sample gets the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="bdd58-170">示例将个人资料照片上传到用户的 OneDrive 根文件夹，并要求 OneDrive 共享照片的 URL。</span><span class="sxs-lookup"><span data-stu-id="bdd58-170">The sample uploads the profile photo to the user's OneDrive root folder and asks OneDrive for the sharing Url of the picture.</span></span> <span data-ttu-id="bdd58-171">最后，示例向 Microsoft Graph 发送 REST 请求，以向提供的电子邮件地址发送邮件消息。</span><span class="sxs-lookup"><span data-stu-id="bdd58-171">Finally, the sample posts a REST request to Microsoft Graph to send a mail message to the provided email address.</span></span> 

<span data-ttu-id="bdd58-172">邮件正文包含图片共享链接，图片本身作为附加的图像文件。</span><span class="sxs-lookup"><span data-stu-id="bdd58-172">The message body contains the picture sharing link and the picture itself as an attached image file.</span></span> <span data-ttu-id="bdd58-173">默认收件人是经过身份验证的用户，但该示例允许用户提供任何其他用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="bdd58-173">The default recipient is the authenticated user, but the sample allows the user to provide the email address of any other user.</span></span> 

<span data-ttu-id="bdd58-174">我们将在此处使用的代码位于 **SendMailViewController_WithPromise.swift** 类中。</span><span class="sxs-lookup"><span data-stu-id="bdd58-174">The code we'll work with here is in the class **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="bdd58-175">函数读取 `self.emailTextField.text` 值，以获取邮件收件人的电子邮件地址，然后启动 **promise chain**，以获取经过身份验证的用户个人资料照片。`viewDidLoad()`</span><span class="sxs-lookup"><span data-stu-id="bdd58-175">The `viewDidLoad()` function reads the `self.emailTextField.text` value to get the mail recipient's email address and then starts a **promise chain** to get the authenticated user's profile picture.</span></span> <span data-ttu-id="bdd58-176">如果 promise 被拒绝，则不会启用 `sendMailButton`。</span><span class="sxs-lookup"><span data-stu-id="bdd58-176">If the promise is rejected, the `sendMailButton` is not enabled.</span></span>

1. <span data-ttu-id="bdd58-177">打开 **SendMailViewController_WithPromise.swift**，</span><span class="sxs-lookup"><span data-stu-id="bdd58-177">Open **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="bdd58-178">然后查找 `viewDidLoad` 函数。</span><span class="sxs-lookup"><span data-stu-id="bdd58-178">and find the `viewDidLoad` function.</span></span> <span data-ttu-id="bdd58-179">将调用 `self.userPictureWork` 函数，以启动 promise chain。</span><span class="sxs-lookup"><span data-stu-id="bdd58-179">The `self.userPictureWork` function is called to start the promise chain.</span></span>

   ```swift
    override func viewDidLoad() {
        super.viewDidLoad()
        //Get user state values before creating mail message to be sent
        do
        {
            try self.userName = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].name!
            try self.emailTextField.text = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].displayableId
            self.userEmailAddress = self.emailTextField.text
            self.headerLabel.text = "Hi, \(self.userName! )"
            
            updateUI(showActivityIndicator: true, statusText: "Getting picture", sendMail: true)

            //Important: Break out of async promise chain by declaring result returns Void
            _ = self.userPictureWork().then{
                result -> Void in
                    self.userPictureUrl = (result[1] as! String)
                    self.userProfilePicture = (result[0] as! UIImage)
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)

            }.catch{err -> Void  in
                self.updateUI(showActivityIndicator: false, statusText: "", sendMail: false)

            }
        } catch _ as NSError{
            self.updateUI(showActivityIndicator: false,
                          statusText: "Error getting user profile picture.", sendMail: false)
        }
    }
  
   ```

   

1. <span data-ttu-id="bdd58-180">在类中查找邮件请求创建帮助程序函数：</span><span class="sxs-lookup"><span data-stu-id="bdd58-180">Find the mail request creation helper function in the class:</span></span>

   ```swift
    /**
     Prepare mail content by loading the JSON request payload template and HTML message body template from resources and replacing placeholders in the templates with appropriate values.
     */
    func mailContent() -> Data? {
        if let emailFilePath = Bundle.main.path(forResource: "EmailPostContent", ofType: "json"),
            let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html")
        {
            do {
                // Prepare upload content
                let emailContent = try String(contentsOfFile: emailFilePath, encoding: String.Encoding.utf8)
                let emailBodyRaw = try String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
                // Request doesn't accept a single quotation mark("), so change it to the acceptable form (\")
                var emailValidBody: String;
                emailValidBody = emailBodyRaw.replacingOccurrences(of: "\"", with: "\\\"")
                emailValidBody = emailValidBody.replacingOccurrences(of: "a href=%s", with: ("a href=" + self.userPictureUrl!))
                let imageData: NSData = UIImagePNGRepresentation(self.userProfilePicture!)! as NSData;
                let emailPostContent = emailContent.replacingOccurrences(of: "<EMAIL>", with: self.emailTextField.text!)
                    .replacingOccurrences(of: "<CONTENTTYPE>", with: "HTML")
                    .replacingOccurrences(of: "<CONTENT>", with: emailValidBody)
                    .replacingOccurrences(of: "<ODATA.TYPE>", with: "#microsoft.graph.fileAttachment")
                    .replacingOccurrences(of: "<IMAGE.TYPE>", with: "image\\/png")
                    .replacingOccurrences(of: "<CONTENTBYTES>", with: imageData.base64EncodedString())
                    .replacingOccurrences(of: "<NAME>", with: "me.png")
                // Return JSON payload with mail body as HTML string and attached picture as a file attachment of type NSData
                return emailPostContent.data(using: String.Encoding.utf8)
            }
            catch {
                // Error handling in case file loading fails.
                return nil
            }
        }
        // Error handling in case files aren't present.
        return nil
    }

   ```
2. <span data-ttu-id="bdd58-181">找到以下帮助程序函数，以获取用户的个人资料照片，将照片上传到 OneDrive，并请求照片的共享链接：</span><span class="sxs-lookup"><span data-stu-id="bdd58-181">Find the following helper functions for getting the user's profile picture,  uploading the photograph to OneDrive, and requesting a sharing link for the picture:</span></span>

   ```swift
    /**
      Async func. Get user's profile photo, upload photo to OneDrive, and get sharing link
     - returns:
        Promise<UIImage>. The user's profile picture
     */
    func getUserPicture()->Promise<UIImage?>{
        return Promise{ fulfill, reject in
            let urlRequest = self.buildRequest(operation: "GET", resource: "photo/$value") as URLRequest
            let task = URLSession.shared.dataTask(with:urlRequest){ data , res , err in
                if let err:Error = err {
                    print(err.localizedDescription)
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return fulfill(self.getDefaultPicture())
                }
                if let data = data {
                    if let userImage: UIImage = UIImage(data:data) {
                        self.userProfilePicture = userImage
                        return fulfill(userImage)
                    } else {
                        return reject("no image" as! Error)
                    }
                } else {
                    return fulfill(self.getDefaultPicture())
                }
            }
            task.resume()
        }
    }
    
    /**
     Async func. Uploads a UIImage object to the signed in user's OneDrive root folder
     - Returns:
        A Promise encapsulating an array of AnyObject. Element 0 contains the user profile photo obtained in the previous chained async call
        Element 1 contains the web sharing URL of the photo in OneDrive as a String
     - Parameters:
     - UIImage: The image to upload to OneDrive
     */
    func uploadPicture(photo: UIImage) -> Promise<[AnyObject]> {
        return Promise<[AnyObject]>{ fulfill, reject in
            let uploadRequestUrl = self.buildRequest(operation: "PUT", resource: "drive/root:/me.jpg:/content", content: UIImageJPEGRepresentation(photo, 1.0)!) as URLRequest
            let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                if let err = err{
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return reject(HTTPError.InvalidRequest)
                }
                //data can be serialized to a DriveItem object
                //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                var itemId: String = "";
                if let responseContent = data {
                    itemId = self.getValueFromResponse(json: responseContent, key: "id" )
                    var returnValues = [AnyObject]();
                    returnValues.append(photo as AnyObject)
                    returnValues.append(itemId as AnyObject)
                    return fulfill(returnValues)
                }
            }
            task.resume()
        }
    }

    /**
     Async func. Requests a new sharing link for the OneDrive item specified by the item id.
     - returns:
     - Promise<String: AnyObject>. The new sharing link and the image wrapped in a Promise
     */
    func createSharingLink(itemId: String, image: UIImage) ->Promise<[AnyObject]>{
        return Promise<[AnyObject]>{ fulfill, reject in
            //Create Data object for the JSON payload
            if let sharingLinkFilePath = Bundle.main.path(forResource: "CreateSharingLink", ofType: "json")
            {
                do {
                    let sharingLinkcontent = try String(contentsOfFile: sharingLinkFilePath, encoding: String.Encoding.utf8)
                    let jsonPayload: Data = sharingLinkcontent.data(using: String.Encoding.utf8)!
                    let uploadRequestUrl = self.buildRequest(
                        operation: "POST", resource: "drive/items/"+itemId+"/createLink", content: jsonPayload) as URLRequest
                    let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                        if let err = err{
                            return reject(err)
                        }
                        if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                            return reject(HTTPError.InvalidRequest)
                        }
                        //data can be serialized to a DriveItem object
                        //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                        var sharingLink: String = "";
                        if let responseContent = data {
                            do {
                                let resultJson = try JSONSerialization.jsonObject(
                                    with: responseContent, options: []) as? [String:AnyObject]
                                sharingLink = (OneDriveFileLink.init(json:resultJson!)?.webUrl)!

                            } catch let error as NSError {
                                print(error)
                            }
                            var returnValues = [AnyObject]();
                            returnValues.append(image as AnyObject)
                            returnValues.append(sharingLink as AnyObject)
                            return fulfill(returnValues)
                        }
                    }
                    task.resume()

                }
            }
        }
   ```

3. <span data-ttu-id="bdd58-182">在类中查找以下发送邮件函数。</span><span class="sxs-lookup"><span data-stu-id="bdd58-182">Find the following send mail function in the class.</span></span>  
 
   ```swift
    /**
     POSTS a new message to the sendmail resource
     - parameters:
        - Data: The body of the message
     */
    func sendMailRESTWithContent(_ content: Data) {
        let _ = self.sendCRUDMessage(resource: "microsoft.graph.sendmail",
                                     operation: "POST",
                                     content: content)
    }
    
    /**
     Send a create, read, update, delete (CRUD) message.
     Create= POST, Update= PUT, Delete= DELETE.
     Read= GET. Use sendGETMessage(resource: String) to read Graph contents
     - returns:
     JSON response as Data
     - parameters:
        - String: The REST resource receiving the CRUD request
        - String: the REST operation requested
        - Data: The json (as Data) representing the values to update
     */
    func sendCRUDMessage(resource: String, operation:String, content: Data)->Data  {
        var returnData: Data;
        returnData = Data.init();
        if  (self.connectToGraph()){
            if (operation == "GET") {
                return self.sendGETMessage(resource: resource)
            }
            let request = self.buildRequest(operation: operation, resource: resource, content:content);
            let task = URLSession.shared.dataTask(with:request as URLRequest, completionHandler:{ data, res, err in
                if let err = err{
                    self.updateUI(showActivityIndicator: false,
                             statusText: "Error assembling the mail content." + err.localizedDescription, sendMail: false)
                }
                let nttpError = self.checkResult(result: res!)
                if (nttpError != HTTPError.NoError) {
                    self.updateUI(showActivityIndicator: false,
                                  statusText: "Error sending the mail.", sendMail: false)
                }
                else {
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)
                }
            }) // let task
             task.resume()
        }
        return returnData;
    }

   ```


## <a name="run-the-app"></a><span data-ttu-id="bdd58-183">运行应用</span><span class="sxs-lookup"><span data-stu-id="bdd58-183">Run the app</span></span>
1. <span data-ttu-id="bdd58-184">运行示例前需要提供在“注册应用”\*\*\*\* 部分的注册过程中收到的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="bdd58-184">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="bdd58-185">打开 **Info.plist** 作为源代码。</span><span class="sxs-lookup"><span data-stu-id="bdd58-185">Open **Info.plist** as source code.</span></span> 

   - <span data-ttu-id="bdd58-186">将 `ENTER_CLIENT_ID_HERE` 替换为注册过程中收到的 **ClientID**。</span><span class="sxs-lookup"><span data-stu-id="bdd58-186">Replace  `ENTER_CLIENT_ID_HERE` with the **ClientID** from the registration process.</span></span> <span data-ttu-id="bdd58-187">请确保 `msal` 未被替换。</span><span class="sxs-lookup"><span data-stu-id="bdd58-187">Be sure that `msal` is not replaced.</span></span> <span data-ttu-id="bdd58-188">替换字符串后，数组字符串值应类似于 `msal48d31887-5fad-4d73-a9f5-3c356e68a038`，其中 GUID 部分是\*\*\*\* 你的客户端 ID：</span><span class="sxs-lookup"><span data-stu-id="bdd58-188">After you replace the string, the array string value looks like `msal48d31887-5fad-4d73-a9f5-3c356e68a038` where the GUID portion is **your** client Id:</span></span>  

   <span data-ttu-id="bdd58-189">例如，</span><span class="sxs-lookup"><span data-stu-id="bdd58-189">For example,</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msalENTER_CLIENT_ID_HERE</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

     <span data-ttu-id="bdd58-190">变为...</span><span class="sxs-lookup"><span data-stu-id="bdd58-190">becomes...</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msal48d31887-5fad-4d73-a9f5-3c356e68a038</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

> <span data-ttu-id="bdd58-191">**注意：** 你会看到已为此项目配置了以下权限范围：`["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]`。</span><span class="sxs-lookup"><span data-stu-id="bdd58-191">**Note:** You'll notice that the following permission scopes have been configured for this project: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` .</span></span> <span data-ttu-id="bdd58-192">在该项目中使用的服务调用，向你的邮件帐户发送邮件并检索一些个人资料信息（显示名称、电子邮件地址），以及写入到用户的 OneDrive 根目录都需要具有这些权限，以使应用在没有权限错误的情况下运行。</span><span class="sxs-lookup"><span data-stu-id="bdd58-192">The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address), and writing to the user's OneDrive root require these permissions for the app to run without a permissions error.</span></span>

2. <span data-ttu-id="bdd58-193">运行示例，点击“连接”\*\*\*\*，使用你的个人帐户、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="bdd58-193">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="bdd58-p120">选择“**发送电子邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="bdd58-p120">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bdd58-196">后续步骤</span><span class="sxs-lookup"><span data-stu-id="bdd58-196">Next steps</span></span>
- <span data-ttu-id="bdd58-197">使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer)试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="bdd58-197">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="bdd58-198">可在 [Microsoft Graph iOS Objective C 代码段示例](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample)中找到 SDK 操作的常见操作示例。</span><span class="sxs-lookup"><span data-stu-id="bdd58-198">Find examples of common operations for SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="bdd58-199">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bdd58-199">See also</span></span>
- [<span data-ttu-id="bdd58-200">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="bdd58-200">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="bdd58-201">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="bdd58-201">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
