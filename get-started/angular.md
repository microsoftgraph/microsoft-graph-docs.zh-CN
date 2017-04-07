# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a>在 AngularJS 应用中使用 Microsoft Graph 入门

本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成[适用于 AngularJS 的 Microsoft Connect 示例](https://github.com/microsoftgraph/angular-connect-rest-sample)的步骤，并说明使用 Microsoft Graph 要实施的主要概念。本文还介绍如何通过使用 [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) 或原始 REST 调用来访问 Microsoft Graph。

下图显示了将要创建的应用。 

![登录后 Web 应用显示“发送邮件”按钮](./images/angular-connect-sample.png)


**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/en-us/getting-started) 快速准备就绪并开始运行。

若要下载使用 Azure AD 终结点的 Connect 示例版本，请参阅 [适用于 AngularJS 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth)。


## <a name="prerequisites"></a>先决条件

若要开始，将需要以下各项： 

- 一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)
- [Node.js with npm](https://nodejs.org/en/download/)
- [Bower](https://bower.io)
- [适用于 AngularJS 的 Microsoft Connect 示例](https://github.com/microsoftgraph/angular-connect-rest-sample)。将使用此次演练示例文件中的 **starter-project** 文件夹。

## <a name="register-the-application"></a>注册应用程序
在 Microsoft 应用注册门户上注册一个应用。这会生成在 Visual Studio 中配置此应用要使用的应用程序 ID 和密码。

1. 使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。

2. 选择“**添加应用**”。

3. 输入应用的名称，并选择“**创建应用程序**”。 
    
    将显示注册页，其中列出应用的属性。

4. 复制应用程序 ID。这是配置该应用要使用的应用唯一标识符。

5. 在“**平台**”下，选择“**添加平台**” > “**Web**”。

6. 请确保已选中“**允许隐式流**”复选框，输入 *http://localhost:8080* 作为重定向 URI。 

7. 选择“**保存**”。


## <a name="configure-the-project"></a>配置项目
1. 打开示例文件中的 **starter-project** 文件夹。
2. 在命令提示符中，运行初学者项目的根目录中的以下命令。这将安装项目依赖项。

        npm install  
        bower install
    
3. 在初学者项目文件的“**public/scripts**”文件夹中，打开 config.js。
4. 在“**clientId**”字段，将 **ENTER_YOUR_CLIENT_ID** 占位符值替换为刚复制的应用程序 ID。
5. **如果使用的是 Microsoft Graph SDK**，则安装并引用 SDK。  
   a.在命令提示符中，运行以下命令以安装 SDK。
        
        bower install https://github.com/microsoftgraph/msgraph-sdk-javascript.git
         
   b.在“**public/index.html**”文件中，将以下代码添加到 `<!-- App code. -->` 部分上方的“**head**”元素：
   
        <!--Include Graph SDK -->
        <script src="./bower_components/msgraph-sdk-javascript/lib/graph-js-sdk-web.js"></script>

  
## <a name="authenticate-the-user-and-get-an-access-token"></a>对用户进行身份验证并获取一个访问令牌
在此步骤中，将添加登录和令牌检索代码。但是首先，让我们进一步了解一下身份验证流。

该单页应用程序使用非常基本的隐式授予流实施方法，该过程需要提供已注册应用的应用程序 ID 和重定向 URL。 

身份验证流可以划分为以下几个基本步骤：

1. 重定向用户以进行身份验证并获得许可。
2. 获取访问令牌。

应用使用 [HelloJS](https://adodson.com/hello.js) 客户端库进行身份验证并获取令牌。应用将访问令牌存储在本地存储中。
    
   >**重要说明** 本项目中的简单身份验证和令牌处理操作仅用于演示目的。在生产应用中，应该构建更为可靠的方法来处理身份验证，其中包括验证和安全令牌处理。

现在回到生成应用中。

1. 打开 aad.js 然后添加下列代码。这将配置与 Azure AD 身份验证提供程序的通信，并添加存储包含访问令牌的身份验证响应的侦听程序。（已将对 HelloJS 的脚本引用添加到 index.html 视图。）

        hello.init({

          aad: {
            name: 'Azure Active Directory',    
            oauth: {
              version: 2,
              auth: 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize',
              grant: 'https://login.microsoftonline.com/common/oauth2/v2.0/token'
            },
            scope_delim: ' ',

            // Don't even try submitting via form.
            // This means no POST operations in <=IE9
            form: false
          }
        });

        hello.on('auth.login', function (auth) {

          // save the auth info into localStorage
          localStorage.auth = angular.toJson(auth.authResponse);
        });

2. 在 graphHelper.js 中，将“*// Initialize the auth request*”替换为以下代码。这将设置身份验证请求的参数。

        // Initialize the auth request.
        hello.init( {
          aad: clientId // from public/scripts/config.js
          }, {
          redirect_uri: redirectUrl,
          scope: graphScopes
        });

3. 将“*// Sign in and sign out the user*”替换为以下代码。**login** 函数使用 HelloJS 获取令牌信息。aad.js 中的侦听程序将包含访问令牌的此信息存储在本地存储中。

        // Sign in and sign out the user.
        login: function login() {
          hello('aad').login({
            display: 'page',
            state: 'abcd'
          });
        },
        logout: function logout() {
          hello('aad').logout();
          delete localStorage.auth;
          delete localStorage.user;
        },

4. **如果使用的是 Microsoft Graph SDK，**则打开 app.js 并将以下代码添加到文件的末尾。此操作将初始化 SDK。

        var authToken;
        var graphClient = MicrosoftGraph.init({
            authProvider: function(done) {
                if (typeof authToken === "undefined") {
                  done({err: "No auth token"})
                } else {
                  done(null, authToken); //first parameter takes an error if you can't get an access token
                }
            }
        });

现在可以添加代码调用 Microsoft Graph。 

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph
应用调用 Microsoft Graph 以获取用户信息并代表用户发送电子邮件。这些调用从 MainController 中启动用于响应 UI 事件。

如果使用的是 Microsoft Graph SDK，请继续阅读。如果使用的是 REST，请参阅[使用 REST API](#using-the-rest-api) 部分。

### <a name="using-the-sdk"></a>使用 SDK
1. 在 graphHelper.js 中，将“*//获取当前用户的个人资料*”替换为以下代码。这将配置 GET 请求并将其发送至 */me* 终结点，然后处理该响应。

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. 将“*//代表当前用户发送电子邮件*”替换为以下代码。这将配置 POST 请求并将其发送至 */me/sendMail* 终结点，然后处理该响应。

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. 在“**public/controllers**”文件夹中，打开 mainController.js。

4. 将“*//设置默认标题和用户属性*”替换为以下代码。这将向 HTTP 请求添加访问令牌，调用 **GraphHelper.me** 获取当前用户的个人资料并处理该响应。

        // Set the default headers and user properties.
        function processAuth() {
            let auth = angular.fromJson(localStorage.auth); 

            // Check token expiry. If the token is valid for another 5 minutes, we'll use it.       
            let expiration = new Date();
            expiration.setTime((auth.expires - 300) * 1000); 
            if (expiration > new Date()) {

              // let the authProvider access the access token
              authToken = auth.access_token;

              // This header has been added to identify our sample in the Microsoft Graph service. If extracting this code for your project please remove.
              $http.defaults.headers.common.SampleID = 'angular-connect-starter';

              if (localStorage.getItem('user') === null) {

                // Get the profile of the current user.
                GraphHelper.me().then(function(user) {

                  // Save the user to localStorage.
                  localStorage.setItem('user', angular.toJson(user));

                  vm.displayName = user.displayName;
                  vm.emailAddress = user.mail || user.userPrincipalName;
                });
              } else {
                let user = angular.fromJson(localStorage.user);

                vm.displayName = user.displayName;
                vm.emailAddress = user.mail || user.userPrincipalName;
              }
           }
        }

5. 将“*//代表当前用户发送电子邮件*”替换为以下代码。这将生成电子邮件、调用 **GraphHelper.sendMail** 并处理该响应。

        // Send an email on behalf of the current user.
        function sendMail() {

          // Check token expiry. If the token is valid for another 5 minutes, we'll use it.
          let auth = angular.fromJson(localStorage.auth);       
          let expiration = new Date();
          expiration.setTime((auth.expires - 300) * 1000); 
          if (expiration > new Date()) {

            // Build the HTTP request payload (the Message object).
            var email = {
                Subject: 'Welcome to Microsoft Graph development with Angular and the Microsoft Graph Connect sample',
                Body: {
                  ContentType: 'HTML',
                  Content: getEmailContent()
                },
                ToRecipients: [
                  {
                    EmailAddress: {
                      Address: vm.emailAddress
                    }
                  }
                ]
            };

            // Save email address so it doesn't get lost with two way data binding.
            vm.emailAddressSent = vm.emailAddress;

            GraphHelper.sendMail(email)
              .then(function (response) {
                $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
                vm.requestSuccess = true;
                vm.requestFinished = true;
              }, function (error) {
                $log.error('HTTP request to the Microsoft Graph API failed.');
                vm.requestSuccess = false;
                vm.requestFinished = true;
              });
           } else {

             // If the token is expired, this sample just redirects the user to sign in.
             GraphHelper.login();
           }
        };

        // Get the HTMl for the email to send.
        function getEmailContent() {
          return "<html><head> <meta http-equiv=\'Content-Type\' content=\'text/html; charset=us-ascii\'> <title></title> </head><body style=\'font-family:calibri\'> <p>Congratulations " + vm.displayName + ",</p> <p>This is a message from the Microsoft Graph Connect sample. You are well on your way to incorporating Microsoft Graph endpoints in your apps. </p> <h3>What&#8217;s next?</h3><ul><li>Check out <a href='https://graph.microsoft.io' target='_blank'>graph.microsoft.io</a> to start building Microsoft Graph apps today with all the latest tools, templates, and guidance to get started quickly.</li><li>Use the <a href='https://graph.microsoft.io/graph-explorer' target='_blank'>Graph explorer</a> to explore the rest of the APIs and start your testing.</li><li>Browse other <a href='https://github.com/microsoftgraph/' target='_blank'>samples on GitHub</a> to see more of the APIs in action.</li></ul> <h3>Give us feedback</h3> <ul><li>If you have any trouble running this sample, please <a href='https://github.com/microsoftgraph/angular-connect-sample/issues' target='_blank'>log an issue</a>.</li><li>For general questions about the Microsoft Graph API, post to <a href='https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest' target='blank'>Stack Overflow</a>. Make sure that your questions or comments are tagged with [microsoftgraph].</li></ul><p>Thanks and happy coding!<br>Your Microsoft Graph samples development team</p> <div style=\'text-align:center; font-family:calibri\'> <table style=\'width:100%; font-family:calibri\'> <tbody> <tr> <td><a href=\'https://github.com/microsoftgraph/angular-connect-sample\'>See on GitHub</a> </td> <td><a href=\'https://officespdev.uservoice.com/\'>Suggest on UserVoice</a> </td> <td><a href=\'https://twitter.com/share?text=I%20just%20started%20developing%20%23Angular%20apps%20using%20the%20%23MicrosoftGraph%20Connect%20sample!%20&url=https://github.com/microsoftgraph/angular-connect-sample\'>Share on Twitter</a> </td> </tr> </tbody> </table> </div>  </body> </html>";
        };
    
6. 保存所有更改。现在可以[运行应用](#run-the-app)。
    
### <a name="using-the-rest-api"></a>使用 REST API
1. 在 graphHelper.js 中，将“*//获取当前用户的个人资料*”替换为以下代码。这将配置 GET 请求并将其发送至 */me* 终结点，然后处理该响应。

        // Get the profile of the current user.
        me: function me() {
          return $http.get('https://graph.microsoft.com/v1.0/me');
        },
  
2. 将“*//代表当前用户发送电子邮件*”替换为以下代码。这将配置 POST 请求并将其发送至 */me/sendMail* 终结点，然后处理该响应。

        // Send an email.n sendMail(email) {
          return $http.post('https://graph.microsoft.com/v1.0/me/sendMail', { 'message' : email, 'saveToSentItems': true });        
        }

3. 在“**public/controllers**”文件夹中，打开 mainController.js。

4. 将“*//设置默认标题和用户属性*”替换为以下代码。这将向 HTTP 请求添加访问令牌，调用 **GraphHelper.me** 获取当前用户的个人资料并处理该响应。

        // Set the default headers and user properties.
        function processAuth() {
          let auth = angular.fromJson(localStorage.auth); 

          // Check token expiry. If the token is valid for another 5 minutes, we'll use it.       
          let expiration = new Date();
          expiration.setTime((auth.expires - 300) * 1000); 
          if (expiration > new Date()) {

            // Add the required Authorization header with bearer token.
            $http.defaults.headers.common.Authorization = 'Bearer ' + auth.access_token;

            // This header has been added to identify our sample in the Microsoft Graph service. If extracting this code for your project please remove.
            $http.defaults.headers.common.SampleID = 'angular-connect-rest-starter';

            if (localStorage.getItem('user') === null) {

              // Get the profile of the current user.
              GraphHelper.me().then(function(response) {

                // Save the user to localStorage.
                let user =response.data;
                localStorage.setItem('user', angular.toJson(user));

                vm.displayName = user.displayName;
                vm.emailAddress = user.mail || user.userPrincipalName;
              });
           } else {
             let user = angular.fromJson(localStorage.user);

             vm.displayName = user.displayName;
             vm.emailAddress = user.mail || user.userPrincipalName;
            }
          }
        } 

5. 将“*//代表当前用户发送电子邮件*”替换为以下代码。这将生成电子邮件、调用 **GraphHelper.sendMail** 并处理该响应。

        // Send an email on behalf of the current user.
        function sendMail() {

          // Check token expiry. If the token is valid for another 5 minutes, we'll use it.
          let auth = angular.fromJson(localStorage.auth);
          let expiration = new Date();
          expiration.setTime((auth.expires - 300) * 1000);
          if (expiration > new Date()) {

            // Build the HTTP request payload (the Message object).
            var email = {
                Subject: 'Welcome to Microsoft Graph development with AngularJS and the Microsoft Graph Connect sample',
                Body: {
                    ContentType: 'HTML',
                    Content: getEmailContent()
                },
                ToRecipients: [
                    {
                        EmailAddress: {
                            Address: vm.emailAddress
                        }
                    }
                ]
            };

            // Save email address so it doesn't get lost with two way data binding.
            vm.emailAddressSent = vm.emailAddress;

            GraphHelper.sendMail(email)
                .then(function (response) {
                    $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
                    response.status === 202 ? vm.requestSuccess = true : vm.requestSuccess = false;
                    vm.requestFinished = true;
                }, function (error) {
                    $log.error('HTTP request to the Microsoft Graph API failed.');
                    vm.requestSuccess = false;
                    vm.requestFinished = true;
                });
            } else {

            // If the token is expired, this sample just redirects the user to sign in.
            GraphHelper.login();
            }
        };

        // Get the HTMl for the email to send.
        function getEmailContent() {
          return "<html><head> <meta http-equiv=\'Content-Type\' content=\'text/html; charset=us-ascii\'> <title></title> </head><body style=\'font-family:calibri\'> <p>Congratulations " + vm.displayName + ",</p> <p>This is a message from the Microsoft Graph Connect sample. You are well on your way to incorporating Microsoft Graph endpoints in your apps. </p> <h3>What&#8217;s next?</h3><ul><li>Check out <a href='https://graph.microsoft.io' target='_blank'>graph.microsoft.io</a> to start building Microsoft Graph apps today with all the latest tools, templates, and guidance to get started quickly.</li><li>Use the <a href='https://graph.microsoft.io/graph-explorer' target='_blank'>Graph explorer</a> to explore the rest of the APIs and start your testing.</li><li>Browse other <a href='https://github.com/microsoftgraph/' target='_blank'>samples on GitHub</a> to see more of the APIs in action.</li></ul> <h3>Give us feedback</h3> <ul><li>If you have any trouble running this sample, please <a href='https://github.com/microsoftgraph/angular-connect-rest-sample/issues' target='_blank'>log an issue</a>.</li><li>For general questions about the Microsoft Graph API, post to <a href='https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest' target='blank'>Stack Overflow</a>. Make sure that your questions or comments are tagged with [microsoftgraph].</li></ul><p>Thanks and happy coding!<br>Your Microsoft Graph samples development team</p> <div style=\'text-align:center; font-family:calibri\'> <table style=\'width:100%; font-family:calibri\'> <tbody> <tr> <td><a href=\'https://github.com/microsoftgraph/angular-connect-rest-sample\'>See on GitHub</a> </td> <td><a href=\'https://officespdev.uservoice.com/\'>Suggest on UserVoice</a> </td> <td><a href=\'https://twitter.com/share?text=I%20just%20started%20developing%20%23Angular%20apps%20using%20the%20%23MicrosoftGraph%20Connect%20sample!%20&url=https://github.com/microsoftgraph/angular-connect-rest-sample\'>Share on Twitter</a> </td> </tr> </tbody> </table> </div>  </body> </html>";
        };

6. 保存所有更改。

## <a name="run-the-app"></a>运行应用

1. 在命令提示符中，运行初学者项目的根目录中的以下命令。

        npm start

2. 在浏览器中，导航至 *http://localhost:8080* 然后选择“**连接**”按钮。

3. 登录并授予所请求的权限。 

4. 还可以编辑收件人的电子邮件地址，然后选择“**发送邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。 

## <a name="next-steps"></a>后续步骤
- 使用 [Graph 浏览器](https://graph.microsoft.io/graph-explorer) 试用 REST API。
- 在 GitHub 上了解我们的其他 [AngularJS 示例](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)。


## <a name="see-also"></a>另请参阅
- [Azure AD v2.0 协议](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 令牌](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)