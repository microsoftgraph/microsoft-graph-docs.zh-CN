# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph 快速入门常见问题解答

本常见问题解答可解决在完成每个 [Microsoft Graph 快速入门](https://developer.microsoft.com/en-us/graph/quick-start)时可能遇到的疑问和问题。

## <a name="what-do-the-quick-starts-do"></a>快速入门有何功能？

快速入门示例演示了如何访问 Microsoft Graph 的功能。 

使用旧版的 Microsoft REST API 时，必须对想要调用的每一个服务进行身份验证。 Microsoft Graph 统一了身份验证并将所有的 API 入口点合并到一个 Graph API 入口点，从而为开发人员消除了这种复杂性。 现在进行一次身份验证，即可访问多个应用程序和服务中的信息。 

为了说明这一点，Microsoft Graph 快速入门示例将通过一次身份验证访问 3 个不同的服务：Microsoft 帐户、OneDrive 和 Outlook。 每个快速入门均从 Microsoft 帐户用户个人资料拉取信息，合并信息并将数据（照片）写入 OneDrive，然后使用 Outlook 生成电子邮件（包含照片的链接）。 

每个获取可供运行的示例应用的快速入门均包含四个步骤：
- 选择平台 
- 获取应用 ID（aka 客户端 ID）
- 生成示例
- 登录并通过电子邮件发送个人资料照片

>注意：这些代码不用于使生产就绪；它们只是对如何在多种不同编程语言和平台中执行同一种方案的简单说明。 若要执行快速入门，建议[全面了解身份验证](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-scenarios)，创建生产就绪应用。


## <a name="general-quick-start-sample-questions"></a>快速入门示例常见问题
关于快速入门示例系列的组织和内容的问题

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>为什么我的快速入门包含自述文件？

每个快速入门都注册新应用程序，并创建一个包含 GitHub 存储库内容的 zip 文件。 它会更新存储库中的文件，使你不必在存储库中配置示例应用程序。 你会在 GitHub 上的 [MicrosoftGraph 组织](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect)中发现这些存储库。

可以随时查看与每个快速入门相关联的存储库、提交问题，和/或按照自述文件中的说明注册你自己的应用程序。 请访问每个快速入门步骤 2 下的**仅为我提供示例代码**链接，转到相关联的存储库。

### <a name="which-microsoft-api-features-do-the-quick-start-samples-show"></a>快速入门示例演示了哪些 Microsoft API 功能？

我们正在持续改进示例系列。 请查看你感兴趣的示例存储库。 我们向你感兴趣的示例添加功能后，会通过该示例的自述文件宣布添加项。 下表说明了各个示例的当前功能

|示例|身份验证|获取个人资料照片|将照片上传到 OneDrive|在电子邮件中共享链接|将照片附加到电子邮件中|发送电子邮件|
|-----:|-----:|-----:|------:|------:|------:|-----:|
|[Android Connect](https://github.com/microsoftgraph/android-java-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Angular 2 Connect](https://github.com/microsoftgraph/angular-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Angular 2 Connect REST](https://github.com/microsoftgraph/angular2-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[ASP.NET Connect](https://github.com/microsoftgraph/aspnet-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect - Swift](https://github.com/microsoftgraph/ios-swift-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect REST - Objective C](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|[](./images/Check.PNG)|
|[Node.js Connect REST](https://github.com/microsoftgraph/nodejs-connect-rest-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)| |![](./images/Check.PNG)|
|[php Connect REST](https://github.com/microsoftgraph/php-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[php Connect](https://github.com/microsoftgraph/php-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Ruby Connect REST](https://github.com/microsoftgraph/ruby-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[UWP Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Xamarin Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|

## <a name="authentication-and-authorization"></a>身份验证和授权
身份验证相关问题和授权问题。 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>为什么快速入门示例没有演示高级身份验证用例？

快速入门示例提供了关于身份验证和 Microsoft Graph API 调用的简介。 向生产应用程序添加身份验证和 Graph API 调用时，需要了解如何针对涉及安全和条件访问问题的高级身份验证方案进行设计。

通过访问身份验证库发布者的页面，可以详细了解你所使用的身份验证库的高级身份验证方案。

- [适用于 Android 和 iOS 的 OAuth2Client](https://github.com/nxtbgthng/OAuth2Client)
- [适用于 Node 的 Passport](http://passportjs.org/)
- [适用于 PHP 的 Illuminate Auth](https://github.com/illuminate/auth)
- [适用于 Python 3 的 Flask](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [适用于 Ruby 的 OmniAuth](https://github.com/omniauth/omniauth)
- [适用于 .NET 的 Microsoft 身份验证库 (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [适用于 Android 的 Microsoft 身份验证库](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [适用于 JavaScript 的 Microsoft 身份验证库](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>Microsoft Graph API
关于 Microsoft Graph API 编码的问题

### <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>我没有收到电子邮件且没有看到任何错误或异常。 为什么无法正常工作？

如果示例看起来要发送一封电子邮件，但你并未在收件箱中看到邮件，请检查垃圾邮件或垃圾邮件文件夹。 如果要从测试租户发送邮件，该邮件可能会被标记为垃圾邮件。

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>为什么示例发送的电子邮件未包含我的个人资料照片？

- 通常情况下，这是因为你的个人资料未设置用户个人资料照片。 使用 Microsoft 服务帐户 (MSA) 登录时，即使你有个人资料照片，它也不会在电子邮件中显示。 Microsoft Graph API 当前不支持 MSA 帐户中的用户个人资料照片。 <br/>快速入门提供的大部分示例都会获取个人资料图片，并将其上传到你的 OneDrive 帐户的根目录。 如果你使用 Microsoft 帐户（live.com、hotmail.com）登录，则 Microsoft Graph 当前将无法获取你的个人资料图片，因此我们会使用思想气泡图像代替。

- Node 示例和 iOS Objective-C 示例无法将用户个人资料照片附加到电子邮件中。 

## <a name="asp-net"></a>ASP .NET
与编码、生成或运行 ASP.NET 快速入门示例有关的问题。

## <a name="universal-windows-platform-uwp"></a>通用 Windows 平台 (UWP)
与编码、生成或运行 UWP 快速入门示例有关的问题。

## <a name="xamarin"></a>Xamarin
与编码、生成或运行 Xamarin 快速入门示例有关的问题。

### <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>为什么不会生成 ASP.NET、UWP 或 Xamarin 项目？

如果未能在 Visual Studio 中生成使用 .NET 库的示例，那么一个或多个项目运行可能会受到 260 个字符的 Windows 路径长度限制。 Xamarin 解决方案尤其容易受此影响，特别是 Xamarin 解决方案中的 Android 项目。 尝试将解决方案移动到根目录或接近根目录的位置。 

## <a name="web-stack-samples"></a>Web 堆栈示例
与编码、生成或运行使用 Web 技术生成的快速入门示例有关的问题。

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>如何知道我的本地计算机是否支持本地 Web 服务器？
基于 Web 技术的快速入门示例提供启动和托管本地 Web 服务器所需的逻辑。 例如，基于 php 5.4.0+ 运行时的 php 示例包含可用于开发的[内置 Web 服务器](http://php.net/manual/en/features.commandline.webserver.php)。 它不适用于生产环境。 

如果下载了 Node.js 示例，请阅读此 [Node.js 入门指南](https://nodejs.org/en/docs/guides/getting-started-guide/)，了解有关启动 Node Web 服务器的信息。 

对于 ASP.NET 示例，Visual Studio 2015 和更高版本包含一个开发 Web 服务器，当你运行该示例时此服务器将自动启动。 无需将示例项目配置为使用该 Web 服务器。 

Ruby Connect 示例[自述文件](https://github.com/microsoftgraph/ruby-connect-rest-sample/blob/master/README.md)提供了启动本地 Ruby Web 服务器所需的说明。 

### <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>如果 Web 平台快速入门提供 REST 和 SDK 示例，是否可以同时运行它们？

是的，可以同时运行这两个示例。 只需确保其中一个示例没有在默认端口运行。 这意味着，在启动测试 Web 服务器时，需要指定至少一个版本示例的端口号。

### <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>为什么一些快速入门包括应用程序密码而其他并不包括？

需要安全调用 Microsoft Graph API 的服务器端 Web 应用程序需要应用程序密码。 这就是为什么 ASP.NET MVC、Node.js、PHP 和 Ruby 的快速入门提供应用程序密码。

### <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>为什么 Angular 快速入门不会像所有其他 Web 平台快速入门一样为我提供应用程序密码？

只有服务器端 Web 应用程序需要应用程序密码。

### <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>当我尝试登录和授权示例应用时遇到一个错误。 我可以采取哪些步骤来解决此问题？ 

首先尝试在 InPrivate 或 Incognito 窗口中运行示例应用程序。 有时 Web 浏览器缓存设置会导致授权步骤失败，尤其是在你使用多个 Microsoft 帐户登录的情况下。 如果这样做不起作用，请在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph) 上向我们提问。 请务必使用 microsoft-graph 标记问题，并将错误信息复制到问题中。

## <a name="didnt-find-what-you-need"></a>无法找到所需的内容？

如果此常见问题解答未能解决你对一个或多个快速入门的疑问或遇到的问题，请在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph) 上报告你的疑问或问题。 

如果你的问题与快速入门提供的代码示例相关，也可以在 GitHub 示例存储库中记录问题。 可以访问每个快速入门步骤 2 下的**仅为我提供示例代码**链接找到存储库。
