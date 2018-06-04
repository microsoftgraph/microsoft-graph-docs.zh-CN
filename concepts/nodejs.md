# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a>在 Node.js 应用中开始使用 Microsoft Graph

本文介绍了通过 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需执行的任务。 它逐步介绍了如何生成 [Microsoft Connect Node.js 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)，并说明了使用 Microsoft Graph 所要实现的主要概念。 本文介绍了如何使用原始 REST 调用来访问 Microsoft Graph API。 若要了解如何生成使用 JavaScript SDK 连接到 Microsoft Graph 的 Node.js 应用，请参阅[基于 Microsoft Graph SDK 的 Node.js Connect 示例](https://github.com/microsoftgraph/nodejs-connect-sample)。

下图展示了将要创建的应用。 

![登录后 Web 应用显示“发送邮件”按钮](./images/web-screenshot.png)


**** 不想生成一个应用？那就使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/zh-CN/getting-started)快速准备就绪并开始运行吧。

若要下载使用 Azure AD 终结点的 Connect 示例版本，请参阅 [适用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth)。


## <a name="prerequisites"></a>先决条件

若要开始，将需要以下各项： 

- 一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](https://docs.microsoft.com/zh-CN/office/developer-program/office-365-developer-program-faq#account-types)
- [含 npm 的 Node.js](https://nodejs.org/en/download/) 
- [Microsoft Connect Node.js 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。 将在本次演练中使用示例文件中的 **starter-project** 文件夹。

## <a name="register-the-application"></a>注册应用程序
在 Microsoft 应用注册门户上注册一个应用。这会生成在 Visual Studio 中配置此应用要使用的应用程序 ID 和密码。

1. 使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。

2. 选择“**添加应用**”。

3. 输入应用的名称，并选择“**创建应用程序**”。 
    
    将显示注册页，其中列出应用的属性。

4. 复制应用程序 ID。这是应用的唯一标识符。 

5. 在“**应用程序密码**”下，选择“**生成新密码**”。从“**生成的新密码**”对话框复制密码。

    将使用此应用程序 ID 和应用程序密码（机密）配置应用。 

6. 在“平台”**** 下，依次选择“添加平台”**** > “Web”****。

7. 输入 *http://localhost:3000/token* 作为重定向 URI。 

8. 选择“保存”****。


## <a name="configure-the-project"></a>配置项目
1. 打开示例文件中的 **starter-project** 文件夹。

1. 在命令提示符中，运行初学者项目的根目录中的以下命令。这将安装项目依赖项。

        npm install

1. 在初学者项目文件中，打开 utils\config.js。


1. 在“**凭据**”字段中，将“**ENTER\_YOUR\_CLIENT\_ID**”和“**ENTER\_YOUR\_SECRET**”占位符值替换为刚复制的值。

  
## <a name="authenticate-the-user-and-get-an-access-token"></a>对用户进行身份验证并获取一个访问令牌
在此步骤中，你将添加登录和令牌管理代码。但是首先，让我们来进一步了解一下身份验证流。

此应用使用授权代码授予流和委派用户身份。对于 Web 应用程序，该流需要已注册应用的应用程序 ID、机密和重定向 URL。 

身份验证流可以划分为以下几个基本步骤：

1. 重定向用户以进行身份验证并获得许可
2. 获取授权代码
3. 兑换访问令牌的授权代码
4. 如果访问令牌过期，则可以使用刷新令牌获取新的访问令牌

应用使用 [oauth](https://www.npmjs.com/package/oauth) 中间件进行身份验证并获取令牌。它使用 [cookie-parser](https://www.npmjs.com/package/cookie-parser) 中间件在 cookie 中缓存令牌信息。用于存储和访问令牌信息的代码可以在 index.js 控制器中找到。
    
   >**重要说明** 本项目中的简单身份验证和令牌处理操作仅用于演示目的。在生产应用中，应该构建更为可靠的方法来处理身份验证，其中包括验证和安全令牌处理。

现在可以添加代码调用 Microsoft Graph。 

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph
应用调用 Microsoft Graph 以获取用户信息并代表用户发送电子邮件。这些调用从 index.js 控制器中启动用于响应 UI 事件。

1. 打开 utils\graphHelper.js。

1. 将 **getUserData** 函数替换为以下代码。这将配置 GET 请求并将其发送至 */me* 终结点，然后处理该响应。

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. 将 **getProfilePhoto** 函数替换为以下代码。这将配置 GET 请求并将其发送至 */me/photo/$value* 终结点，然后处理响应。注意个人资料照片当前不适用于 MSA 帐户。
    
        function getProfilePhoto(accessToken, callback) {
          // Get the profile photo of the current user (from the user's mailbox on Exchange Online).
          // This operation in version 1.0 supports only work or school mailboxes, not personal mailboxes.
          request
           .get('https://graph.microsoft.com/v1.0/me/photo/$value')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             // Returns 200 OK and the photo in the body. If no photo exists, returns 404 Not Found.
             callback(err, res.body);
           });
        }

1. 将 **uploadFile** 函数替换为以下代码。这将配置 PUT 请求并将其发送至 */me/drive/root/children/mypic.jpg/content* 终结点。如果该文件存在，此请求将更新其内容。如果该文件不存在，此请求将创建此文件并上载个人资料照片的内容。 

        function uploadFile(accessToken, file, callback) {
          // This operation only supports files up to 4MB in size.
          // To upload larger files, see `https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/item_createUploadSession`.
          request
           .put('https://graph.microsoft.com/v1.0/me/drive/root/children/mypic.jpg/content')
           .send(file)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'image/jpg')
           .end((err, res) => {
             // Returns 200 OK and the file metadata in the body.
             callback(err, res.body);
           });
        }

1. 将 **getSharingLink** 函数替换为以下代码。这将配置 GET 请求并将其发送至 */me/drive/items/{file id}/createLink* 终结点，然后处理结果。结果是消息中将包含的文件共享链接。

        function getSharingLink(accessToken, id, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/drive/items/' + id + '/createLink')
           .send({ type: 'view' })
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .end((err, res) => {
             // Returns 200 OK and the permission with the link in the body.
             callback(err, res.body.link);
           });
        }

1. 将 **postSendMail** 函数替换为以下代码。这将配置 POST 请求并将其发送至 */me/sendMail* 终结点，然后处理该响应。

        function postSendMail(accessToken, message, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/sendMail')
           .send(message)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .set('Content-Length', message.length)
           .end((err, res) => {
             // Returns 202 if successful.
             // Note: If you receive a 500 - Internal Server Error
             // while using a Microsoft account (outlook.com, hotmail.com or live.com),
             // it's possible that your account has not been migrated to support this flow.
             // Check the inner error object for code 'ErrorInternalServerTransientError'.
             // You can try using a newly created Microsoft account or contact support.
             callback(err, res);
           });
        }

1. 打开 utils\emailer.js。

1. 将 **wrapEmail** 函数替换为以下代码。这将生成表示要发送的电子邮件的有效负载。

        function wrapEmail(content, recipient, file) {
          const attachments = [{
            '@odata.type': '#microsoft.graph.fileAttachment',
            ContentBytes: file,
            Name: 'mypic.jpg'
          }];
          const emailAsPayload = {
            Message: {
              Subject: 'Welcome to Microsoft Graph development with Node.js and the Microsoft Graph Connect sample',
              Body: {
                ContentType: 'HTML',
                Content: content
              },
              ToRecipients: [
                {
                  EmailAddress: {
                    Address: recipient
                  }
                }
              ]
            },
            SaveToSentItems: true,
            Attachments: attachments
          };
          return emailAsPayload;
        }

## <a name="run-the-app"></a>运行应用

1. 在命令提示符中，运行初学者项目的根目录中的以下命令。


        npm start

1. 在浏览器中，导航至 *http://localhost:3000* 然后选择“连接到 Office 365”**** 按钮。

1. 登录并授予所请求的权限。 

1. 还可以编辑收件人的电子邮件地址，然后选择“**发送邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。 

## <a name="next-steps"></a>后续步骤
- 使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)试用 REST API。
- 探索我们在 GitHub 上的其他 [Node.js 示例](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)。
- 使用 [Microsoft Graph TypeScript 类型](https://github.com/microsoftgraph/msgraph-typescript-typings)
- 尝试 [Microsoft Graph TypeScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)

## <a name="see-also"></a>另请参阅
- [Azure AD v2.0 协议](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-protocols/)
- [Azure AD v2.0 令牌](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-tokens/)
- [Microsoft Graph JavaScript SDK Node.js Connect 示例](https://github.com/microsoftgraph/nodejs-connect-sample)
