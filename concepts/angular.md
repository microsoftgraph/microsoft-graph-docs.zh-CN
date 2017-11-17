# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a><span data-ttu-id="75bf8-101">在 AngularJS 应用中使用 Microsoft Graph 入门</span><span class="sxs-lookup"><span data-stu-id="75bf8-101">Get started with Microsoft Graph in an AngularJS app</span></span>

<span data-ttu-id="75bf8-p101">本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成[适用于 AngularJS 的 Microsoft Connect 示例](https://github.com/microsoftgraph/angular-connect-rest-sample)的步骤，并说明使用 Microsoft Graph 要实施的主要概念。本文还介绍如何通过使用 [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) 或原始 REST 调用来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) or raw REST calls.</span></span>

<span data-ttu-id="75bf8-105">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="75bf8-105">The following image shows the app you'll create.</span></span> 

![登录后 Web 应用显示“发送邮件”按钮](./images/angular-connect-sample.png)


<span data-ttu-id="75bf8-p102">**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/en-us/getting-started) 快速准备就绪并开始运行。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="75bf8-109">若要下载使用 Azure AD 终结点的 Connect 示例版本，请参阅 [适用于 AngularJS 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth)。</span><span class="sxs-lookup"><span data-stu-id="75bf8-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="75bf8-110">先决条件</span><span class="sxs-lookup"><span data-stu-id="75bf8-110">Prerequisites</span></span>

<span data-ttu-id="75bf8-111">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="75bf8-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="75bf8-112">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="75bf8-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- [<span data-ttu-id="75bf8-113">Node.js with npm</span><span class="sxs-lookup"><span data-stu-id="75bf8-113">Node.js with npm</span></span>](https://nodejs.org/en/download/)
- [<span data-ttu-id="75bf8-114">Bower</span><span class="sxs-lookup"><span data-stu-id="75bf8-114">Bower</span></span>](https://bower.io)
- <span data-ttu-id="75bf8-p103">[适用于 AngularJS 的 Microsoft Connect 示例](https://github.com/microsoftgraph/angular-connect-sample)。将使用此次演练示例文件中的 **starter-project** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p103">The [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="75bf8-117">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="75bf8-117">Register the application</span></span>
<span data-ttu-id="75bf8-p104">在 Microsoft 应用注册门户上注册一个应用。这会生成在 Visual Studio 中配置此应用要使用的应用程序 ID 和密码。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="75bf8-120">使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="75bf8-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="75bf8-121">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="75bf8-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="75bf8-122">输入应用的名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="75bf8-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="75bf8-123">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="75bf8-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="75bf8-p105">复制应用程序 ID。这是配置该应用要使用的应用唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p105">Copy the application ID. This is the unique identifier for your app that you'll use to configure the app.</span></span>

5. <span data-ttu-id="75bf8-126">在“**平台**”下，选择“**添加平台**” > “**Web**”。</span><span class="sxs-lookup"><span data-stu-id="75bf8-126">Under **Platforms**, choose **Add Platform** > **Web**.</span></span>

6. <span data-ttu-id="75bf8-127">请确保已选中“**允许隐式流**”复选框，输入 *http://localhost:8080* 作为重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="75bf8-127">Make sure the **Allow Implicit Flow** check box is selected, and enter *http://localhost:8080* as the Redirect URI.</span></span> 

7. <span data-ttu-id="75bf8-128">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="75bf8-128">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="75bf8-129">配置项目</span><span class="sxs-lookup"><span data-stu-id="75bf8-129">Configure the project</span></span>
1. <span data-ttu-id="75bf8-130">打开示例文件中的 **starter-project** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="75bf8-130">Open the **starter-project** folder in the sample files.</span></span>
2. <span data-ttu-id="75bf8-p106">在命令提示符中，运行初学者项目的根目录中的以下命令。这将安装项目依赖项。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p106">In a command prompt, run the following commands in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install  
        bower install
    
3. <span data-ttu-id="75bf8-133">在初学者项目文件的“public/scripts”****文件夹中，打开 config.js。</span><span class="sxs-lookup"><span data-stu-id="75bf8-133">In the starter project files, in the **public/scripts** folder, open config.js.</span></span>
4. <span data-ttu-id="75bf8-134">在“clientID”****字段中，将 **ENTER_YOUR_CLIENT_ID** 占位符值替换为刚复制的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="75bf8-134">In the **clientID** field, replace the **ENTER_YOUR_CLIENT_ID** placeholder value with the application ID you just copied.</span></span>

## <a name="call-microsoft-graph-with-the-sdk"></a><span data-ttu-id="75bf8-135">使用 SDK 调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75bf8-135">Call Microsoft Graph with the SDK</span></span>
<span data-ttu-id="75bf8-p107">应用调用 Microsoft Graph 以获取用户信息并代表用户发送电子邮件。这些调用从 MainController 中启动用于响应 UI 事件。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p107">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the MainController in response to UI events.</span></span>

<span data-ttu-id="75bf8-p108">打开 app.js 并将以下代码添加到文件底部。此操作将初始化 SDK。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p108">Open app.js and add the following code to the bottom of the file. This initializes the SDK.</span></span>

    var authToken;
    var graphClient = MicrosoftGraph.Client.init({
        authProvider: function(done) {
        if (typeof authToken === "undefined") {
          done({err: "No auth token"})
        } else {
          done(null, authToken); //first parameter takes an error if you can't get an access token
        }
        }
    });

### <a name="using-the-sdk"></a><span data-ttu-id="75bf8-140">使用 SDK</span><span class="sxs-lookup"><span data-stu-id="75bf8-140">Using the SDK</span></span>
1. <span data-ttu-id="75bf8-p109">在 graphHelper.js 中，将“*//获取当前用户的个人资料*”替换为以下代码。这将配置 GET 请求并将其发送至 */me* 终结点，然后处理该响应。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p109">In graphHelper.js, replace *// Get the profile of the current user* with the following code. This configures and sends the GET request to the */me* endpoint, and processes the response.</span></span>

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. <span data-ttu-id="75bf8-p110">将“*//代表当前用户发送电子邮件*”替换为以下代码。这将配置 POST 请求并将其发送至 */me/sendMail* 终结点，然后处理该响应。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p110">Replace *// Send an email on behalf of the current user* with the following code. This configures and sends the POST request to the */me/sendMail* endpoint, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. <span data-ttu-id="75bf8-145">在“**public/controllers**”文件夹中，打开 mainController.js。</span><span class="sxs-lookup"><span data-stu-id="75bf8-145">In the **public/controllers** folder, open mainController.js.</span></span>

4. <span data-ttu-id="75bf8-p111">将“*//设置默认标题和用户属性*”替换为以下代码。这将向 HTTP 请求添加访问令牌，调用 **GraphHelper.me** 获取当前用户的个人资料并处理该响应。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p111">Replace *// Set the default headers and user properties* with the following code. This adds the access token to the HTTP request, calls **GraphHelper.me** to get the current user's profile, and processes the response.</span></span>

        // Set the default headers and user properties.
        function processAuth() {

        // let the authProvider access the access token
        authToken = localStorage.token;

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

5. <span data-ttu-id="75bf8-p112">将“*//代表当前用户发送电子邮件*”替换为以下代码。这将生成电子邮件、调用 **GraphHelper.sendMail** 并处理该响应。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p112">Replace *// Send an email on behalf of the current user* with the following code. This builds the email message, calls **GraphHelper.sendMail**, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        function sendMail() {

          authToken = localStorage.token;       

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
          $scope.$apply();
        }, function (error) {
          $log.error('HTTP request to the Microsoft Graph API failed.');
          vm.requestSuccess = false;
          vm.requestFinished = true;
          $scope.$apply();
        });

        };

6. <span data-ttu-id="75bf8-150">保存所有更改。</span><span class="sxs-lookup"><span data-stu-id="75bf8-150">Save all your changes.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="75bf8-151">运行应用</span><span class="sxs-lookup"><span data-stu-id="75bf8-151">Run the app</span></span>

1. <span data-ttu-id="75bf8-152">在命令提示符中，运行初学者项目的根目录中的以下命令。</span><span class="sxs-lookup"><span data-stu-id="75bf8-152">In a command prompt, run the following command in the root directory of the starter project.</span></span>

        npm start

2. <span data-ttu-id="75bf8-153">在浏览器中，导航至 *http://localhost:8080* 然后选择“**连接**”按钮。</span><span class="sxs-lookup"><span data-stu-id="75bf8-153">In a browser, navigate to *http://localhost:8080* and choose the **Connect** button.</span></span>

3. <span data-ttu-id="75bf8-154">登录并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="75bf8-154">Sign in and grant the requested permissions.</span></span> 

4. <span data-ttu-id="75bf8-p113">还可以编辑收件人的电子邮件地址，然后选择“**发送邮件**”按钮。在邮件发送后，按钮下方将显示成功消息。</span><span class="sxs-lookup"><span data-stu-id="75bf8-p113">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="75bf8-157">后续步骤</span><span class="sxs-lookup"><span data-stu-id="75bf8-157">Next steps</span></span>
- <span data-ttu-id="75bf8-158">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="75bf8-158">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="75bf8-159">在 GitHub 上了解我们的其他 [AngularJS 示例](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults)。</span><span class="sxs-lookup"><span data-stu-id="75bf8-159">Explore our other [AngularJS samples](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="75bf8-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="75bf8-160">See also</span></span>
- [<span data-ttu-id="75bf8-161">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="75bf8-161">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="75bf8-162">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="75bf8-162">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
