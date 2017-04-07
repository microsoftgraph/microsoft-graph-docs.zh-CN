# <a name="register-your-microsoft-graph-application-with-the-azure-ad-v20-endpoint"></a>使用 Azure AD v2.0 终结点注册 Microsoft Graph 应用程序

若要使用 Azure AD v2.0 终结点，则需要在 [Microsoft 应用注册门户](https://apps.dev.microsoft.com) (https://apps.dev.microsoft.com) 上注册你的应用。注册应用可以使用该身份验证提供程序创建应用的身份，并且允许应用在提交来自用户的身份验证请求时证明自身身份。注册生成将用于配置应用进行身份验证的应用程序 ID 和应用机密。

> **注意：**本文介绍了如何向 Azure AD v2.0 终结点进行应用注册。若要[向 Azure AD 注册应用](app_authorization.md)，请使用 [Azure 门户](https://aka.ms/aadapplist)。
> 
> 此外，请注意如果已经在 Microsoft Azure 管理门户注册应用，那么这些应用将不会在应用注册门户中列出。在 Azure 管理门户中管理这些应用。 

1. 使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。

2. 选择“**添加应用**”。

3. 输入应用的名称，并选择“**创建应用程序**”。

    将显示注册页，其中列出应用的属性。

4. 复制应用程序 ID。这是应用的唯一标识符。

    你将使用该应用程序 ID 配置应用。

5. 在“**平台**”下，选择“**添加平台**”，然后为应用选择合适的平台：
    
    对于客户端应用：
    1. 选择“**移动平台**”。

    2. 将客户端 ID（应用程序 ID）和重定向 URL 值复制到剪切板。将需要在示例应用中输入这些值。

        应用 ID 是应用的唯一标识符。重定向 URL 是向每个应用程序提供的唯一的 URI，以确保发送到此 URI 的邮件只发送到该应用程序。 

    对于 Web 应用：
    1. 选择“**Web**”。
    2. 如果使用的是隐式授权类型，或者如果使用的是 OpenID Connect 混合流，请确保已选中“允许隐式流”复选框。 
        
        “允许隐式流”选项启用 OpenID Connect 混合流。在身份验证过程中，这可使应用同时接收登录信息 (id_token) 以及应用用来获取访问令牌的项目（在这种情况下，项目为授权代码）。


    3. 指定重定向 URI。
        
        重定向 URI 是 Azure AD v2.0 终结点处理身份验证请求后在应用中调用的位置。
    4. 在“**应用程序机密**”下，选择“**生成新密码**”。从“**生成的新密码**”对话框复制应用机密。
        
        你将使用该应用机密配置应用。
    
6. 选择“**保存**”。

## <a name="see-also"></a>另请参阅

[Microsoft Graph 的应用身份验证](auth_overview.md)
