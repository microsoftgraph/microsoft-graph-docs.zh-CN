# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph 快速入门常见问题解答

本常见问题解答可解决在完成每个 [Microsoft Graph 快速入门](https://developer.microsoft.com/en-us/graph/quick-start)时可能遇到的疑问和问题。

## <a name="what-do-the-quick-starts-do"></a>快速入门有何功能？

无论你选择什么平台，每个快速入门都执行以下任务：

- 在[应用程序注册门户](https://apps.dev.microsoft.com)中为你注册新应用程序。 这就是为什么在你**获取应用程序 ID** 时，我们要求你使用 Microsoft 帐户登录。 如果应用程序需要应用程序密码，快速入门将为你创建一个密码。 
- 下载存储在 GitHub 存储库中的示例代码副本。 可以在 GitHub 上的 [MicrosoftGraph 组织](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect)中看到这些存储库。
- 将新的应用程序 ID 和应用程序密码（如有必要）插入存储在 GitHub 存储库的示例代码中的配置文件。 我们不想在 HTTP 请求中发送敏感信息，因此要求你在我们创建新应用程序后复制应用程序密码，然后在下载示例副本之前将它复制到快速入门窗体中。
- 系统将提示你下载完全配置的示例。 下载并解压缩示例代码之后，你就拥有了应能运行的客户端或 Web 应用程序，前提是你已在开发环境中安装了指定的系统必备组件（IDE、Web 框架等）。


## <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>为什么不会生成 ASP.NET、UWP 或 Xamarin 项目？

如果未能在 Visual Studio 中生成使用 .NET 库的示例，那么一个或多个项目运行可能会受到 260 个字符的 Windows 路径长度限制。 Xamarin 解决方案尤其容易受此影响，特别是 Xamarin 解决方案中的 Android 项目。 尝试将解决方案移动到根目录或接近根目录的位置。 

## <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>如果 Web 平台快速入门提供 REST 和 SDK 示例，是否可以同时运行它们？

是的，可以同时运行这两个示例。 只需确保其中一个示例没有在默认端口运行。 这意味着，在启动测试 Web 服务器时，需要指定至少一个版本示例的端口号。

## <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>我没有收到电子邮件且没有看到任何错误或异常。 为什么无法正常工作？

如果示例看起来要发送一封电子邮件，但你并未在收件箱中看到邮件，请检查垃圾邮件或垃圾邮件文件夹。 如果要从测试租户发送邮件，该邮件可能会被标记为垃圾邮件。

## <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>当我尝试登录和授权示例应用程序时遇到一个错误。 我可以采取哪些步骤来解决此问题？ 

首先尝试在 InPrivate 或 Incognito 窗口中运行示例应用程序。 有时 Web 浏览器缓存设置会导致授权步骤失败，尤其是在你使用多个 Microsoft 帐户登录的情况下。 如果这样做不起作用，请在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph) 上向我们提问。 请务必使用 microsoft-graph 标记问题，并将错误信息复制到问题中。

## <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>为什么一些快速入门包括应用程序密码而其他并不包括？

需要安全调用 Microsoft Graph API 的服务器端 Web 应用程序需要应用程序密码。 这就是为什么 ASP.NET MVC、Node.js、PHP 和 Ruby 的快速入门提供应用程序密码。

## <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>为什么 Angular 快速入门不会像所有其他 Web 平台快速入门一样为我提供应用程序密码？

只有服务器端 Web 应用程序需要应用程序密码。

## <a name="why-does-my-quick-start-contain-a-readme-file"></a>为什么我的快速入门包含自述文件？

每个快速入门都注册新应用，并创建一个包含 GitHub 存储库内容的 zip 文件。 它会更新存储库中的文件，使你不必在存储库中配置示例应用程序。 你会在 GitHub 上的 [MicrosoftGraph 组织](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect)中发现这些存储库。

可以随时查看与每个快速入门相关联的存储库、提交问题，和/或按照自述文件中的说明注册你自己的应用程序。 请访问每个快速入门步骤 2 下的**仅为我提供示例代码**链接，转到相关联的存储库。

## <a name="why-did-the-sample-give-me-an-image-containing-a-thought-bubble"></a>为什么示例图像显示一个思想气泡？

快速入门提供的大部分示例都会获取个人资料图片，并将其上传到你的 OneDrive 帐户的根目录。 如果你使用 Microsoft 帐户（live.com、hotmail.com）登录，则 Microsoft Graph 当前将无法获取你的个人资料图片，因此我们会使用思想气泡图像代替。 如果你的帐户没有个人资料图片，示例也会使用此图像。

## <a name="why-do-you-provide-a-manage-your-apphttpsappsdevmicrosoftcom-link-after-i-get-an-app-id"></a>为什么在我获取应用程序 ID 后，你们会提供**[管理应用程序](https://apps.dev.microsoft.com)**链接？

我们提供此链接是因为应用程序 ID 步骤会在[应用程序注册门户](https://apps.dev.microsoft.com)中为你注册新应用程序。 通过此链接可以查看此应用程序的设置，删除应用程序，或者甚至在运行示例之后更新应用程序设置。 

## <a name="didnt-find-what-you-need"></a>无法找到所需的内容？

如果此常见问题解答未能解决你对一个或多个快速入门的疑问或遇到的问题，请在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph) 上报告你的疑问或问题。 

如果你的问题与快速入门提供的代码示例相关，也可以在 GitHub 示例存储库中提交问题。 可以访问每个快速入门步骤 2 下的**仅为我提供示例代码**链接找到存储库。
