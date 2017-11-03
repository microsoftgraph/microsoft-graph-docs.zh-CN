# <a name="ios-samples-for-the-microsoft-graph-api"></a>Microsoft Graph API 的 iOS 示例
本文介绍了两个通过 Office 365 或托管服务帐户 (MSA)（如 Outlook 使用者用户）对用户进行身份验证的 iOS 示例。 两个示例均通过 Outlook 服务发送电子邮件，但其中一个示例获取并在电子邮件正文中发送用户配置文件照片，扩展了此功能

## <a name="ios-objective-c-connect-rest-sample"></a>iOS Objective-C 连接 REST 示例
此示例使用标准 iOS HTTPS 库向 Microsoft Graph 发出 REST 调用。 它使用 Microsoft 身份验证库 (MSAL) 对用户进行身份验证。 使用 MSAL 库，应用可以从 Office 365 或 MSA 帐户对用户进行身份验证。 但是无法从本地 Azure Active Directory 实例对用户进行身份验证。

可以使用此示例发送电子邮件，但无法检索已验证用户的照片，也无法在电子邮件中嵌入照片。

- [开始在 Objective-C iOS 应用中使用 Microsoft Graph](ios_objectivec.md)

## <a name="ios-swift-connect-sample"></a>iOS Swift Connect 示例
此示例对 Objective C 使用 Microsoft Graph 客户端库，以访问 Microsoft Graph 终结点。 用户身份验证由第三方 [NXOAuth2Client](https://github.com/nxtbgthng/OAuth2Client) 库处理。 此库允许应用从本地 Azure Active Directory 实例对用户进行身份验证，但是不会对 MSA 用户进行身份验证。

本示例演示了如何通过 Graph 访问用户的 Azure 个人资料。 另外，还会介绍如何获取用户的个人资料照片、将照片上传到用户的 OneDrive 存储以及在 Outlook 电子邮件正文中嵌入照片。

- [在 iOS 应用中开始使用 Microsoft Graph](ios_swift.md)
