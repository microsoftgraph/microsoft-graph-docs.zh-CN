# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a><span data-ttu-id="92b34-101">在 Node.js 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92b34-101">Get started with Microsoft Graph in a Node.js app</span></span>

<span data-ttu-id="92b34-102">本文介绍了通过 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需执行的任务。</span><span class="sxs-lookup"><span data-stu-id="92b34-102">This article describes the tasks required to get an access token from the v2.0 authentication endpoint and call  Microsoft Graph.</span></span> <span data-ttu-id="92b34-103">它逐步介绍了如何生成 [Microsoft Connect Node.js 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)，并说明了使用 Microsoft Graph 所要实现的主要概念。</span><span class="sxs-lookup"><span data-stu-id="92b34-103">It walks you through building the [Connect Sample for PHP](https://github.com/microsoftgraph/nodejs-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span> <span data-ttu-id="92b34-104">本文介绍了如何使用原始 REST 调用来访问 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="92b34-104">The article describes how to access Microsoft Graph by using direct REST calls.</span></span> <span data-ttu-id="92b34-105">若要了解如何生成使用 JavaScript SDK 连接到 Microsoft Graph 的 Node.js 应用，请参阅[基于 Microsoft Graph SDK 的 Node.js Connect 示例](https://github.com/microsoftgraph/nodejs-connect-sample)。</span><span class="sxs-lookup"><span data-stu-id="92b34-105">If you're interested in building a Node.js app that connects to Microsoft Graph with the JavaScript SDK, see our [Microsoft Graph SDK-based Node.js Connect sample](https://github.com/microsoftgraph/nodejs-connect-sample).</span></span>

<span data-ttu-id="92b34-106">下图展示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="92b34-106">The following image shows is the app you'll create.</span></span> 

![登录后 Web 应用显示“发送邮件”按钮](./images/web-screenshot.png)


<span data-ttu-id="92b34-p102">**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/zh-CN/getting-started) 快速准备就绪并开始运行。</span><span class="sxs-lookup"><span data-stu-id="92b34-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/zh-CN/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="92b34-110">若要下载使用 Azure AD 终结点的 Connect 示例版本，请参阅 [适用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth)。</span><span class="sxs-lookup"><span data-stu-id="92b34-110">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="92b34-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="92b34-111">Prerequisites</span></span>

<span data-ttu-id="92b34-112">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="92b34-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="92b34-113">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="92b34-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- [<span data-ttu-id="92b34-114">含 npm 的 Node.js</span><span class="sxs-lookup"><span data-stu-id="92b34-114">Node.js with npm</span></span>](https://nodejs.org/en/download/) 
- <span data-ttu-id="92b34-115">[Microsoft Connect Node.js 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="92b34-115">The [Microsoft Connect sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span></span> <span data-ttu-id="92b34-116">将在本次演练中使用示例文件中的 **starter-project** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="92b34-116">The Microsoft Connect Sample for AngularJS. You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="92b34-117">注册应用</span><span class="sxs-lookup"><span data-stu-id="92b34-117">Register the application</span></span>
<span data-ttu-id="92b34-p104">在 Microsoft 应用注册门户上注册一个应用。这会生成在 Visual Studio 中配置此应用要使用的应用程序 ID 和密码。</span><span class="sxs-lookup"><span data-stu-id="92b34-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="92b34-120">使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="92b34-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="92b34-121">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="92b34-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="92b34-122">输入应用的名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="92b34-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="92b34-123">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="92b34-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="92b34-p105">复制应用程序 ID。这是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="92b34-p105">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="92b34-p106">在“**应用程序密码**”下，选择“**生成新密码**”。从“**生成的新密码**”对话框复制密码。</span><span class="sxs-lookup"><span data-stu-id="92b34-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="92b34-128">将使用此应用程序 ID 和应用程序密码（机密）配置应用。</span><span class="sxs-lookup"><span data-stu-id="92b34-128">You'll use the application ID and application password (secret) to configure the app.</span></span> 

6. <span data-ttu-id="92b34-129">在“平台”****下，依次选择“添加平台”**** > “Web”****。</span><span class="sxs-lookup"><span data-stu-id="92b34-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="92b34-130">输入“http://localhost:3000/token”**作为重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="92b34-130">Enter *http://localhost:3000/token* as the Redirect URI.</span></span> 

8. <span data-ttu-id="92b34-131">选择“保存”****。</span><span class="sxs-lookup"><span data-stu-id="92b34-131">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="92b34-132">配置项目</span><span class="sxs-lookup"><span data-stu-id="92b34-132">Configure the project</span></span>
1. <span data-ttu-id="92b34-133">打开示例文件中的 **starter-project** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="92b34-133">Open the **starter-project** folder in the sample files.</span></span>

1. <span data-ttu-id="92b34-p107">在命令提示符中，运行初学者项目的根目录中的以下命令。这将安装项目依赖项。</span><span class="sxs-lookup"><span data-stu-id="92b34-p107">In a command prompt, run the following command in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install

1. <span data-ttu-id="92b34-136">在初学者项目文件中，打开 utils\config.js。</span><span class="sxs-lookup"><span data-stu-id="92b34-136">In the starter project files, open utils\config.js.</span></span>


1. <span data-ttu-id="92b34-137">在“**凭据**”字段中，将“**ENTER\_YOUR\_CLIENT\_ID**”和“**ENTER\_YOUR\_SECRET**”占位符值替换为刚复制的值。</span><span class="sxs-lookup"><span data-stu-id="92b34-137">In the **credentials** field, replace the **ENTER\_YOUR\_CLIENT\_ID** and **ENTER\_YOUR\_SECRET** placeholder values with the values you just copied.</span></span>

  
## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="92b34-138">对用户进行身份验证并获取一个访问令牌</span><span class="sxs-lookup"><span data-stu-id="92b34-138">Authenticate the user and get an access token</span></span>
<span data-ttu-id="92b34-p108">在此步骤中，你将添加登录和令牌管理代码。但是首先，让我们来进一步了解一下身份验证流。</span><span class="sxs-lookup"><span data-stu-id="92b34-p108">In this step, you'll add sign-in and token management code. But first, let's take a closer look at the auth flow.</span></span>

<span data-ttu-id="92b34-p109">此应用使用授权代码授予流和委派用户身份。对于 Web 应用程序，该流需要已注册应用的应用程序 ID、机密和重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="92b34-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="92b34-143">身份验证流可以划分为以下几个基本步骤：</span><span class="sxs-lookup"><span data-stu-id="92b34-143">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="92b34-144">重定向用户以进行身份验证并获得许可</span><span class="sxs-lookup"><span data-stu-id="92b34-144">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="92b34-145">获取授权代码</span><span class="sxs-lookup"><span data-stu-id="92b34-145">Get an authorization code</span></span>
3. <span data-ttu-id="92b34-146">兑换访问令牌的授权代码</span><span class="sxs-lookup"><span data-stu-id="92b34-146">Redeem the authorization code for an access token</span></span>
4. <span data-ttu-id="92b34-147">如果访问令牌过期，则可以使用刷新令牌获取新的访问令牌</span><span class="sxs-lookup"><span data-stu-id="92b34-147">Use the refresh token to get a new access token when the access token expires</span></span>

<span data-ttu-id="92b34-p110">应用使用 [oauth](https://www.npmjs.com/package/oauth) 中间件进行身份验证并获取令牌。它使用 [cookie-parser](https://www.npmjs.com/package/cookie-parser) 中间件在 cookie 中缓存令牌信息。用于存储和访问令牌信息的代码可以在 index.js 控制器中找到。</span><span class="sxs-lookup"><span data-stu-id="92b34-p110">The app uses the [oauth](https://www.npmjs.com/package/oauth) middleware to authenticate and obtain tokens. It uses the [cookie-parser](https://www.npmjs.com/package/cookie-parser) middleware to cache token information in cookies. The code used to store and access token information is found in the index.js controller.</span></span>
    
   ><span data-ttu-id="92b34-p111">**重要说明** 本项目中的简单身份验证和令牌处理操作仅用于演示目的。在生产应用中，应该构建更为可靠的方法来处理身份验证，其中包括验证和安全令牌处理。</span><span class="sxs-lookup"><span data-stu-id="92b34-p111">**Important** The simple authentication and token handling in this project is for sample purposes only. In a production app, you should construct a more robust way of handling authentication, including validation and secure token handling.</span></span>

<span data-ttu-id="92b34-153">现在可以添加代码调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="92b34-153">Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph"></a><span data-ttu-id="92b34-154">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92b34-154">Call Microsoft Graph</span></span>
<span data-ttu-id="92b34-p112">应用调用 Microsoft Graph 以获取用户信息并代表用户发送电子邮件。这些调用从 index.js 控制器中启动用于响应 UI 事件。</span><span class="sxs-lookup"><span data-stu-id="92b34-p112">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the index.js controller in response to UI events.</span></span>

1. <span data-ttu-id="92b34-157">打开 utils\graphHelper.js。</span><span class="sxs-lookup"><span data-stu-id="92b34-157">Open utils\graphHelper.js.</span></span>

1. <span data-ttu-id="92b34-p113">将 **getUserData** 函数替换为以下代码。这将配置 GET 请求并将其发送至 */me* 终结点，然后处理该响应。</span><span class="sxs-lookup"><span data-stu-id="92b34-p113">Replace the **getUserData** function with the following code. This configures and sends the GET request to the */me* endpoint and processes the response.</span></span>

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. <span data-ttu-id="92b34-p114">将 **getProfilePhoto** 函数替换为以下代码。这将配置 GET 请求并将其发送至 */me/photo/$value* 终结点，然后处理响应。注意个人资料照片当前不适用于 MSA 帐户。</span><span class="sxs-lookup"><span data-stu-id="92b34-p114">Replace the **getProfilePhoto** function with the following code. This configures and sends the GET request to the */me/photo/$value* endpoint and processes the response. Note that profile photos aren't currently available for MSA accounts.</span></span>
    
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

1. <span data-ttu-id="92b34-p115">将 **uploadFile** 函数替换为以下代码。这将配置 PUT 请求并将其发送至 */me/drive/root/children/mypic.jpg/content* 终结点。如果该文件存在，此请求将更新其内容。如果该文件不存在，此请求将创建此文件并上载个人资料照片的内容。</span><span class="sxs-lookup"><span data-stu-id="92b34-p115">Replace the **uploadFile** function with the following code. This configures and sends the PUT request to the */me/drive/root/children/mypic.jpg/content* endpoint. If the file exists, this requests updates the content. If it doesn't exist, it creates the file and uploads the contents of the profile photo.</span></span> 

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

1. <span data-ttu-id="92b34-p116">将 **getSharingLink** 函数替换为以下代码。这将配置 GET 请求并将其发送至 */me/drive/items/{file id}/createLink* 终结点，然后处理结果。结果是消息中将包含的文件共享链接。</span><span class="sxs-lookup"><span data-stu-id="92b34-p116">Replace the **getSharingLink** function with the following code. This configures and sends the GET request to the */me/drive/items/{file id}/createLink* endpoint and processes the result. The result is a sharing link to the file that will be included in the message.</span></span>

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

1. <span data-ttu-id="92b34-p117">将 **postSendMail** 函数替换为以下代码。这将配置 POST 请求并将其发送至 */me/sendMail* 终结点，然后处理该响应。</span><span class="sxs-lookup"><span data-stu-id="92b34-p117">Replace the **postSendMail** function with the following code. This configures and sends the POST request to the */me/sendMail* endpoint and processes the response.</span></span>

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

1. <span data-ttu-id="92b34-172">打开 utils\emailer.js。</span><span class="sxs-lookup"><span data-stu-id="92b34-172">Open utils\emailer.js.</span></span>

1. <span data-ttu-id="92b34-p118">将 **wrapEmail** 函数替换为以下代码。这将生成表示要发送的电子邮件的有效负载。</span><span class="sxs-lookup"><span data-stu-id="92b34-p118">Replace the **wrapEmail** function with the following code. This builds the payload that represents the email message to send.</span></span>

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

## <a name="run-the-app"></a><span data-ttu-id="92b34-175">运行应用</span><span class="sxs-lookup"><span data-stu-id="92b34-175">Run the app</span></span>

1. <span data-ttu-id="92b34-176">在命令提示符中，运行初学者项目的根目录中的以下命令。</span><span class="sxs-lookup"><span data-stu-id="92b34-176">In a command prompt, run the following command in the root directory of the starter project.</span></span>


        npm start

1. <span data-ttu-id="92b34-177">在浏览器中，导航至 *http://localhost:3000* 然后选择“**连接到 Office 365**”按钮。</span><span class="sxs-lookup"><span data-stu-id="92b34-177">In a browser, navigate to *http://localhost:3000* and choose the **Connect to Office 365** button.</span></span>

1. <span data-ttu-id="92b34-178">登录并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="92b34-178">Sign in and grant the requested permissions.</span></span> 

1. <span data-ttu-id="92b34-p119">还可以编辑收件人的电子邮件地址，然后选择“**发送邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="92b34-p119">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="92b34-181">后续步骤</span><span class="sxs-lookup"><span data-stu-id="92b34-181">Next steps</span></span>
- <span data-ttu-id="92b34-182">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="92b34-182">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="92b34-183">探索我们在 GitHub 上的其他 [Node.js 示例](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)。</span><span class="sxs-lookup"><span data-stu-id="92b34-183">Explore our other [Node.js samples](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>
- <span data-ttu-id="92b34-184">使用 [Microsoft Graph TypeScript 类型](https://github.com/microsoftgraph/msgraph-typescript-typings)</span><span class="sxs-lookup"><span data-stu-id="92b34-184">Use the [Microsoft Graph TypeScript types](https://github.com/microsoftgraph/msgraph-typescript-typings)</span></span>
- <span data-ttu-id="92b34-185">尝试 [Microsoft Graph TypeScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)</span><span class="sxs-lookup"><span data-stu-id="92b34-185">Try the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)</span></span>

## <a name="see-also"></a><span data-ttu-id="92b34-186">另请参阅</span><span class="sxs-lookup"><span data-stu-id="92b34-186">See also</span></span>
- [<span data-ttu-id="92b34-187">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="92b34-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="92b34-188">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="92b34-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-v2-tokens/)
- [<span data-ttu-id="92b34-189">Microsoft Graph JavaScript SDK Node.js Connect 示例</span><span class="sxs-lookup"><span data-stu-id="92b34-189">Microsoft Graph JavaScript SDK Node.js Connect sample</span></span>](https://github.com/microsoftgraph/nodejs-connect-sample)
