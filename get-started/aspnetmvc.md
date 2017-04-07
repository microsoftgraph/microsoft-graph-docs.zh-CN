# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a>在 ASP.NET 4.6 MVC 应用中使用 Microsoft Graph 入门

本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成[适用于 ASP.NET 4.6 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/aspnet-connect-sample)的步骤，并说明使用 Microsoft Graph 要实施的主要概念。本文还介绍如何通过使用 [Microsoft Graph .NET 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)或原始 REST 调用来访问 Microsoft Graph。

下图显示了将要创建的应用。 

![具备"获取电子邮件地址"和"发送电子邮件"按钮的 Web 应用](images/aspnet-connect-sample.png "具备‘获取电子邮件地址’和‘发送电子邮件’按钮的 Web 应用")

[Azure AD v2.0 终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview) 允许用户使用 Microsoft 帐户 (MSA) 或工作或学校帐户进行登录。应用使用 [ASP.Net OpenID Connect OWIN 中间件](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/)和 [适用于 .Net 的 Microsoft Authentication Library (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client) 进行登录和令牌管理。

>MSAL 目前处于预发布状态，因此，不应该在生产代码中使用。在此处仅用于说明目的。 

**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/en-us/getting-started) 快速准备就绪并开始运行。

若要下载使用 Azure AD 终结点的 Connect 示例版本并使用 REST 调用访问 Microsoft Graph，请参阅 [Office 365 Connect ASP.NET MVC 示例](https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth)。


## <a name="prerequisites"></a>先决条件

若要开始，将需要以下各项： 

- 一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)
- Visual Studio 2015 
- [ASP.NET 4.6 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/aspnet-connect-sample)。将使用示例文件中的 **starter-project** 文件夹。


## <a name="register-the-application"></a>注册应用程序

本步骤中，将会在 Microsoft 应用注册门户上注册一个应用。这会生成在 Visual Studio 中配置此应用时要使用的应用程序 ID 和密码。

1. 使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。

2. 选择“**添加应用**”。

3. 输入应用的名称，并选择“**创建应用程序**”。 
    
    将显示注册页，其中列出应用的属性。

4. 复制应用程序 ID。这是应用的唯一标识符。 

5. 在“**应用程序密码**”下，选择“**生成新密码**”。从“**生成的新密码**”对话框复制密码。

    将使用此应用程序 ID 和密码来配置应用。 

6. 在“**平台**”下，选择“**添加平台**” > “**Web**”。

7. 请确保已选中“**允许隐式流**”复选框，输入 *http://localhost:55065/* 作为重定向 URI。 

    “**允许隐式流**”选项可启用 OpenID Connect 混合流。在身份验证过程中，这可使应用同时接收登录信息 (**id_token**) 以及应用用来获取访问令牌的项目（在这种情况下，项目为授权代码）。

8. 选择“**保存**”。

### <a name="configure-the-project"></a>配置项目

1. 在 Visual Studio 中打开初学者项目的解决方案文件。

2. 打开项目的 Web.config 文件。

3. 在 **appSettings** 元素中找到应用配置密钥。将 ENTER_YOUR_CLIENT_ID 和 ENTER_YOUR_SECRET 占位符值替换为刚复制的值。

重定向 URI 是已注册项目的 URL。已请求的[权限范围](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes)允许应用获取用户配置文件信息并发送电子邮件。


## <a name="authenticate-the-user-and-get-an-access-token"></a>对用户进行身份验证并获取一个访问令牌

在此步骤中，你将添加登录和令牌管理代码。但是首先，让我们来进一步了解一下身份验证流。

此应用使用具有委派用户身份的授权代码授予流。对于 Web 应用程序，该流需要已注册应用的应用程序 ID、密码和重定向 URL。 

身份验证流可以划分为以下几个基本步骤：

1. 重定向用户以进行身份验证并获得许可
2. 获取授权代码
3. 兑换访问令牌的授权代码
4. 如果访问令牌过期，则可以使用刷新令牌获取新的访问令牌

应用使用 [ASP.Net OpenID Connect OWIN 中间件](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/)和[适用于 .Net 的 Microsoft Authentication Library (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client) 进行登录和令牌管理。这些将为你处理大多数身份验证任务。
    
初学者项目已声明以下中间件和 MSAL NuGet 依赖项：

  - Microsoft.Owin.Security.OpenIdConnect
  - Microsoft.Owin.Security.Cookies
  - Microsoft.Owin.Host.SystemWeb
  - Microsoft.Identity.Client -Pre

现在回到生成应用的操作中。

1. 在 **App_Start** 文件夹中，打开 Startup.Auth.cs。 

1. 用以下代码替换 **ConfigureAuth** 方法。这会设置与 Azure AD 进行通信的坐标，并设置 OpenID Connect 中间件所使用的 Cookie 身份验证。

        public void ConfigureAuth(IAppBuilder app)
        {
            app.SetDefaultSignInAsAuthenticationType(CookieAuthenticationDefaults.AuthenticationType);

            app.UseCookieAuthentication(new CookieAuthenticationOptions());

            app.UseOpenIdConnectAuthentication(
                new OpenIdConnectAuthenticationOptions
                {

                    // The `Authority` represents the Microsoft v2.0 authentication and authorization service.
                    // The `Scope` describes the permissions that your app will need. See https://azure.microsoft.com/documentation/articles/active-directory-v2-scopes/                    
                    ClientId = appId,
                    Authority = "https://login.microsoftonline.com/common/v2.0",
                    PostLogoutRedirectUri = redirectUri,
                    RedirectUri = redirectUri,
                    Scope = "openid email profile offline_access " + graphScopes,
                    TokenValidationParameters = new TokenValidationParameters
                    {
                        ValidateIssuer = false,
                        // In a real application you would use IssuerValidator for additional checks, 
                        // like making sure the user's organization has signed up for your app.
                        //     IssuerValidator = (issuer, token, tvp) =>
                        //     {
                        //         if (MyCustomTenantValidation(issuer)) 
                        //             return issuer;
                        //         else
                        //             throw new SecurityTokenInvalidIssuerException("Invalid issuer");
                        //     },
                    },
                    Notifications = new OpenIdConnectAuthenticationNotifications
                    {
                        AuthorizationCodeReceived = async (context) =>
                        {
                            var code = context.Code;
                            string signedInUserID = context.AuthenticationTicket.Identity.FindFirst(ClaimTypes.NameIdentifier).Value;
                            ConfidentialClientApplication cca = new ConfidentialClientApplication(
                                appId, 
                                redirectUri,
                                new ClientCredential(appSecret),
                                new SessionTokenCache(signedInUserID, context.OwinContext.Environment["System.Web.HttpContextBase"] as HttpContextBase));
                                string[] scopes = graphScopes.Split(new char[] { ' ' });

                            AuthenticationResult result = await cca.AcquireTokenByAuthorizationCodeAsync(scopes, code);
                        },
                        AuthenticationFailed = (context) =>
                        {
                            context.HandleResponse();
                            context.Response.Redirect("/Error?message=" + context.Exception.Message);
                            return Task.FromResult(0);
                        }
                    }
                });
        }
  
  应用启动时，OWIN Startup 类（在 Startup.cs 中定义）调用 **ConfigureAuth** 方法，该方法又调用 **app.UseOpenIdConnectAuthentication** 以初始化用于登录和初始化令牌请求的中间件。应用请求以下权限范围：

  - 用于登录的 **openid**、**电子邮件** 和 **配置文件**
  - 用于获取令牌的**offline\_access**（获取刷新令牌所需的）、**User.Read**、**Mail.Send**
  
  MSAL **ConfidentialClientApplication** 对象代表应用，并处理令牌管理任务。使用在其中存储令牌信息的 **SessionTokenCache**（在 TokenStorage/SessionTokenCache.cs 中定义的示例令牌缓存实现）进行初始化。缓存根据用户 ID 保存当前 HTTP 会话中的令牌，但生产应用程序可能会使用更为持久的存储。

现在将代码添加到示例身份验证提供程序，旨在轻松地替换为你自己的自定义身份验证提供程序。接口和提供程序类已添加到该项目。

1. 在“**帮助程序**”文件夹中，打开 SampleAuthProvider.cs。

1. 将 **GetUserAccessTokenAsync** 方法替代为以下使用 MSAL 的实现，以获取访问令牌。

        // Get an access token. First tries to get the token from the token cache.
        public async Task<string> GetUserAccessTokenAsync()
        {
            string signedInUserID = ClaimsPrincipal.Current.FindFirst(ClaimTypes.NameIdentifier).Value;
            tokenCache = new SessionTokenCache(
                signedInUserID, 
                HttpContext.Current.GetOwinContext().Environment["System.Web.HttpContextBase"] as HttpContextBase);
            //var cachedItems = tokenCache.ReadItems(appId); // see what's in the cache

            ConfidentialClientApplication cca = new ConfidentialClientApplication(
                appId, 
                redirectUri,
                new ClientCredential(appSecret), 
                tokenCache);

            try
            {
                AuthenticationResult result = await cca.AcquireTokenSilentAsync(scopes.Split(new char[] { ' ' }));
                return result.Token;
            }

            // Unable to retrieve the access token silently.
            catch (MsalSilentTokenAcquisitionException)
            {
                HttpContext.Current.Request.GetOwinContext().Authentication.Challenge(
                    new AuthenticationProperties() { RedirectUri = "/" },
                    OpenIdConnectAuthenticationDefaults.AuthenticationType);

                throw new Exception(Resource.Error_AuthChallengeNeeded);
            }
        }

  MSAL 检查匹配未过期或将要过期的访问令牌的缓存。如果找不到有效的令牌，将会使用刷新令牌（如果存在有效的刷新令牌）获取新的访问令牌。如果无法自动获得一个新的访问令牌，MSAL 会引发 **MsalSilentTokenAcquisitionException** 来指示需要用户提示。 

接下来，将添加代码来处理从 UI 进行登录和注销。

1. 在“**控制器**”文件夹中，打开 AccountController.cs。  

1. 将以下方法添加到 **AccountController** 类。**SignIn** 方法通知中间件将授权请求发送到 Azure AD。

        public void SignIn()
        {
            if (!Request.IsAuthenticated)
            {
                // Signal OWIN to send an authorization request to Azure.
                HttpContext.GetOwinContext().Authentication.Challenge(
                    new AuthenticationProperties { RedirectUri = "/" },
                    OpenIdConnectAuthenticationDefaults.AuthenticationType);
            }
        }

        // Here we just clear the token cache, sign out the GraphServiceClient, and end the session with the web app.  
        public void SignOut()
        {
            if (Request.IsAuthenticated)
            {
                // Get the user's token cache and clear it.
                string userObjectId = ClaimsPrincipal.Current.FindFirst(ClaimTypes.NameIdentifier).Value;

                SessionTokenCache tokenCache = new SessionTokenCache(userObjectId, HttpContext);
                tokenCache.Clear(userObjectId);
            }

            //SDKHelper.SignOutClient();

            // Send an OpenID Connect sign-out request. 
            HttpContext.GetOwinContext().Authentication.SignOut(
            CookieAuthenticationDefaults.AuthenticationType);
            Response.Redirect("/");
        }

现在可以添加代码调用 Microsoft Graph。 

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph

如果使用的是 Microsoft Graph 库，请继续阅读。如果使用的是 REST，请参阅[使用 REST API](#using-the-rest-api) 部分。

### <a name="using-the-library"></a>使用库
在此步骤中，将会关注 **SDKHelper****GraphService** 和 **HomeController** 类。 

 - 每次调用 Microsoft Graph 之前，**SDKHelper** 会初始化库的 **GraphServiceClient** 实例。在将访问令牌添加到该请求时执行此操作。 
 - **GraphService** 使用库生成请求并将其发送到 Microsoft Graph，然后处理响应。
 - **HomeController** 包含初始化库调用以响应 UI 事件的操作。

初学者项目已为 Microsoft Graph .NET Client Library NuGet 程序包声明依赖项：*Microsoft.Graph*。

1. 右键单击“**帮助程序**”文件夹并选择“**添加**” > “**类**”。 

1. 命名新类 *SDKHelper* 并选择“**添加**”。

1. 用以下代码替换内容。

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

  请注意，初始化客户端时，调用 **SampleAuthProvider** 以获取令牌。

1. 在“**模型**”文件夹中，打开 GraphService.cs。该服务使用库与 Microsoft Graph 进行交互。

1. 添加以下 **using** 语句。

        using Microsoft.Graph;

1. 用以下方法替换 *// GetMyEmailAddress*。可获取当前用户的电子邮件地址。 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  请注意，**Select** 段只能请求要返回的 **mail** 和 **userPrinicipalName**。可以使用 **Select** 和 **Filter** 减少响应数据有效负载的大小。

1. 用以下方法替换 *// SendEmail* 以生成和发送电子邮件。

        // Send an email message from the current user.
        public async Task SendEmail(GraphServiceClient graphClient, Message message)
        {
            await graphClient.Me.SendMail(message, true).Request().PostAsync();
        }

        // Create the email message.
        public Message BuildEmailMessage(string recipients, string subject)
        {

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
                    Content = Resource.Graph_SendMail_Body_Content,
                    ContentType = BodyType.Html,
                },
                Subject = subject,
                ToRecipients = recipientList
            };
            return email;
        }

1. 在“**控制器**”文件夹中，打开 HomeController.cs。

1. 添加以下 **using** 语句。

        using Microsoft.Graph;
  
1. 用以下操作替换 *// Controller actions*。

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

            // Build the email message.
            Message message = graphService.BuildEmailMessage(Request.Form["recipients"], Request.Form["subject"]);
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
           }
        }

接下来，将更改在需要用户提示时身份验证提供程序引发的异常。

1. 在“**帮助程序**”文件夹中，打开 SampleAuthProvider.cs。

1. 添加以下 **using** 语句。

        using Microsoft.Graph;
  
1. 在 **GetUserAccessTokenAsync** 方法的**捕获**块更改所引发的异常，如下所示：

        throw new ServiceException(
            new Error
            {
                Code = GraphErrorCode.AuthenticationFailure.ToString(),
                Message = Resource.Error_AuthChallengeNeeded,
            });

最后，将添加调用来注销客户端。 

1. 在“**控制器**”文件夹中，打开 AccountController.cs。 

1. 取消评论下列行：

        SDKHelper.SignOutClient();

现在可以[运行应用](#run-the-app)。

### <a name="using-the-rest-api"></a>使用 REST API
在此步骤中，将使用 **GraphService**、**GraphResources** 和 **HomeController** 类进行操作。 

 - **GraphService** 生成 HTTP 请求并将其发送到 Microsoft Graph，然后处理响应。 
 - **GraphResources** 代表该应用发送到 Microsoft Graph 的数据和从 Microsoft Graph 接收的数据。 
 - **HomeController** 包含初始化 Microsoft Graph 调用以响应 UI 事件的操作。

首先定义数据访问层。

1. 在“**模型**”文件夹中，打开 GraphService.cs。

1. 添加以下 **using** 语句。

        using Newtonsoft.Json;
        using Newtonsoft.Json.Linq;
        using System.Net;
        using System.Net.Http;
        using System.Net.Http.Headers;
        using System.Text;

1. 用以下方法替换 *// GetMyEmailAddress*。可获取当前用户的电子邮件地址。 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(string accessToken)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            string endpoint = "https://graph.microsoft.com/v1.0/me";
            string queryParameter = "?$select=mail,userPrincipalName";
            UserInfo me = new UserInfo();

            using (var client = new HttpClient())
            {
                using (var request = new HttpRequestMessage(HttpMethod.Get, endpoint + queryParameter))
                {
                    request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
                    request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
                    using (HttpResponseMessage response = await client.SendAsync(request))
                    {
                        if (response.StatusCode == HttpStatusCode.OK)
                        {
                            var json = JObject.Parse(await response.Content.ReadAsStringAsync());
                            me.Address = !string.IsNullOrEmpty(json.GetValue("mail").ToString())?json.GetValue("mail").ToString():json.GetValue("userPrincipalName").ToString();
                        }
                        return me.Address?.Trim();
                    }
                }
            }
        }

1. 用以下方法替换 *// SendEmail* 以生成和发送电子邮件。

        // Send an email message from the current user.
        public async Task<string> SendEmail(string accessToken, MessageRequest email)
        {
            string endpoint = "https://graph.microsoft.com/v1.0/me/sendMail";
            using (var client = new HttpClient())
            {
                using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
                {
                    request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
                    request.Content = new StringContent(JsonConvert.SerializeObject(email), Encoding.UTF8, "application/json");
                    using (HttpResponseMessage response = await client.SendAsync(request))
                    {
                        if (response.IsSuccessStatusCode)
                        {
                            return Resource.Graph_SendMail_Success_Result;
                        }
                        return response.ReasonPhrase;
                    }
                }
            }
        }

        // Create the email message.
        public MessageRequest BuildEmailMessage(string recipients, string subject)
        {

            // Prepare the recipient list.
            string[] splitter = { ";" };
            string[] splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();
            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient
                {
                    EmailAddress = new UserInfo
                    {
                        Address = recipient.Trim()
                    }
                });
            }

            // Build the email message.
            Message message = new Message
            {
                Body = new ItemBody
                {
                    Content = Resource.Graph_SendMail_Body_Content,
                    ContentType = "HTML"
                },
                Subject = subject,
                ToRecipients = recipientList
            };

            return new MessageRequest
            {
                Message = message,
                SaveToSentItems = true
            };
        }

1. 右键单击“**模型**”文件夹并选择“**添加**” > “**类**”。

1. 命名类 *GraphResources*，然后选择“**确定**”。

1. 用以下代码替换内容。
 
        using System;
        using System.Collections.Generic;

        namespace Microsoft_Graph_SDK_ASPNET_Connect.Models
        {
            public class UserInfo
            {
                public string Address { get; set; }
            }

            public class Message
            {
                public string Subject { get; set; }
                public ItemBody Body { get; set; }
                public List<Recipient> ToRecipients { get; set; }
            }

          public class Recipient
            {
                public UserInfo EmailAddress { get; set; }
            }

            public class ItemBody
            {
                public string ContentType { get; set; }
                public string Content { get; set; }
            }

            public class MessageRequest
            {
                public Message Message { get; set; }
                public bool SaveToSentItems { get; set; }
            }
        }

1. 在“**控制器**”文件夹中，打开 HomeController.cs。
  
1. 用以下操作替换 *// Controller actions*。

        [Authorize]
        // Get the current user's email address from their profile.
        public async Task<ActionResult> GetMyEmailAddress()
        {
            try
            {

                // Get an access token.
                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                // Get the current user's email address. 
                ViewBag.Email = await graphService.GetMyEmailAddress(accessToken);
                return View("Graph");
            }
            catch (Exception e)
            {
                if (e.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + e.Message });
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

            // Build the email message.
            MessageRequest email = graphService.BuildEmailMessage(Request.Form["recipients"], Request.Form["subject"]);
            try
            {

                // Get an access token.
                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                // Send the email.
                ViewBag.Message = await graphService.SendEmail(accessToken, email);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                return View("Graph");
            }
            catch (Exception e)
            {
                if (e.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + e.Message });
            }
        }

## <a name="run-the-app"></a>运行应用
1. 按 F5 生成和运行此应用。 

2. 使用个人、工作或学校帐户登录，并授予所请求的权限。

3. 选择“**获取电子邮件地址**”按钮。在操作完成后，已登录用户的电子邮件地址会在此页上显示。

4. 还可以编辑收件人列表和电子邮件主题，然后选择“**发送电子邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。


## <a name="next-steps"></a>后续步骤
- 使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer)试用 REST API。
- 在 [ASP.NET 4.6 的 Microsoft Graph 代码段示例](https://github.com/microsoftgraph/aspnet-snippets-sample)中查找常见操作的示例，或浏览 GitHub 上的其他 [ASP.NET 示例](http://aka.ms/aspnetgraphsamples)。

## <a name="see-also"></a>另请参阅
- [Microsoft Graph.NET 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [用于 web API 身份验证方案的 Web 应用程序](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [使用 OpenID Connect 将 Microsoft 标识和 Microsoft Graph 集成到 Web 应用程序中](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [Azure AD v2.0 协议](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 令牌](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
