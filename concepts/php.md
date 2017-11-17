# <a name="get-started-with-microsoft-graph-in-a-php-app"></a><span data-ttu-id="b33fd-101">在 PHP 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b33fd-101">Get started with Microsoft Graph in a PHP app</span></span>

<span data-ttu-id="b33fd-p101">本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成[适用于 PHP 的 Connect 示例 (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) 的步骤，并说明实现使用 Microsoft Graph 的主要概念。本文还介绍如何使用 REST 调用来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call  Microsoft Graph. It walks you through building the [Connect Sample for PHP (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using REST calls.</span></span>

<span data-ttu-id="b33fd-p102">若要在 PHP 应用中使用 Microsoft Graph，则需要向用户显示 Microsoft 登录页。以下屏幕截图显示了 Microsoft 帐户的登录页。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p102">To use Microsoft Graph in your PHP app, you need to show the Microsoft sign in page to your users. The following screenshot shows a sign in page for Microsoft accounts.</span></span>

![Microsoft 帐户的登录页](images/MicrosoftSignIn.png)

<span data-ttu-id="b33fd-p103">**不想生成一个应用吗？**通过下载本文所基于的[适用于 PHP 的 Connect 示例 (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) 快速准备就绪并开始运行。或尝试使用[适用于 PHP 的 Connect 示例 (SDK) ](https://github.com/microsoftgraph/php-connect-sample)版本，该版本使用[适用于 PHP 的 Microsoft Graph 库](https://github.com/microsoftgraph/msgraph-sdk-php)（预览）。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p103">**Don't feel like building an app?** Get up and running fast by downloading the [Connect Sample for PHP (REST)](https://github.com/microsoftgraph/php-connect-rest-sample) that this article is based on. Or try out the [Connect Sample for PHP (SDK)](https://github.com/microsoftgraph/php-connect-sample) version that uses the [Microsoft Graph Library for PHP](https://github.com/microsoftgraph/msgraph-sdk-php) (Preview).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="b33fd-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="b33fd-111">Prerequisites</span></span>

<span data-ttu-id="b33fd-112">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="b33fd-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="b33fd-113">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="b33fd-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="b33fd-114">PHP 版本 5.5.9 或更高版本</span><span class="sxs-lookup"><span data-stu-id="b33fd-114">PHP version 5.5.9 or greater</span></span>
- [<span data-ttu-id="b33fd-115">编辑器</span><span class="sxs-lookup"><span data-stu-id="b33fd-115">Composer</span></span>](https://getcomposer.org/)


## <a name="register-the-application"></a><span data-ttu-id="b33fd-116">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="b33fd-116">Register the application</span></span>
<span data-ttu-id="b33fd-p104">在 Microsoft 应用注册门户上注册一个应用。这会生成用于配置此应用的应用程序 ID 和密码。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app.</span></span>

1. <span data-ttu-id="b33fd-119">使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="b33fd-119">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="b33fd-120">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="b33fd-120">Choose **Add an app**.</span></span>

3. <span data-ttu-id="b33fd-121">输入应用的名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="b33fd-121">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="b33fd-122">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="b33fd-122">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="b33fd-123">选择“**生成新密码**”。</span><span class="sxs-lookup"><span data-stu-id="b33fd-123">Choose **Generate New Password**.</span></span>

5. <span data-ttu-id="b33fd-124">复制应用程序 ID 和密码。</span><span class="sxs-lookup"><span data-stu-id="b33fd-124">Copy the application ID and password.</span></span>

6. <span data-ttu-id="b33fd-125">选择“**添加平台**”和“**网页**”。</span><span class="sxs-lookup"><span data-stu-id="b33fd-125">Choose **Add Platform** and **Web**.</span></span>

7. <span data-ttu-id="b33fd-126">在“**重定向 URI**”字段中，键入 `http://localhost:8000/oauth`。</span><span class="sxs-lookup"><span data-stu-id="b33fd-126">In the **Redirect URI** field, type `http://localhost:8000/oauth`.</span></span>

8. <span data-ttu-id="b33fd-127">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="b33fd-127">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="b33fd-128">配置项目</span><span class="sxs-lookup"><span data-stu-id="b33fd-128">Configure the project</span></span>

<span data-ttu-id="b33fd-p105">使用编辑器启动一个新项目。若要使用 Laravel 框架创建新的 PHP 项目，请使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="b33fd-p105">Start a new project using composer. To create a new PHP project using the Laravel framework, use the following command:</span></span>

```bash
composer create-project --prefer-dist laravel/laravel getstarted
```
 
<span data-ttu-id="b33fd-131">这将创建一个可用于此项目的 **getstarted** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="b33fd-131">This creates a **getstarted** folder that you can use for this project.</span></span>

> <span data-ttu-id="b33fd-132">注意：还可以使用 [初学者项目](https://github.com/microsoftgraph/php-connect-rest-sample/tree/master/starter-project) 进行项目配置，这样就可以专注于此次演练的编码部分。</span><span class="sxs-lookup"><span data-stu-id="b33fd-132">Note: You can also use the [Starter project](https://github.com/microsoftgraph/php-connect-rest-sample/tree/master/starter-project) that takes care of the project configuration so you can focus on the coding sections of this walkthrough.</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="b33fd-133">对用户进行身份验证并获取一个访问令牌</span><span class="sxs-lookup"><span data-stu-id="b33fd-133">Authenticate the user and get an access token</span></span>
<span data-ttu-id="b33fd-p106">使用 OAuth 库来简化身份验证流程。[PHP 联盟](http://thephpleague.com/) 提供了可用于此项目的 [OAuth 客户端库](https://github.com/thephpleague/oauth2-client)。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p106">Use an OAuth library to simplify the authentication process. [The PHP League](http://thephpleague.com/) provides an [OAuth client library](https://github.com/thephpleague/oauth2-client) that you can use in this project.</span></span>

### <a name="add-the-dependency-to-composer"></a><span data-ttu-id="b33fd-136">将依赖项添加到编辑器</span><span class="sxs-lookup"><span data-stu-id="b33fd-136">Add the dependency to composer</span></span>

<span data-ttu-id="b33fd-137">打开 `composer.json` 文件，并在**请求**部分中包括以下依赖项：</span><span class="sxs-lookup"><span data-stu-id="b33fd-137">Open the `composer.json` file and include the following dependency in the **require** section:</span></span>

```json
"league/oauth2-client": "^1.4"
```

<span data-ttu-id="b33fd-138">通过运行以下命令更新这些依赖项：</span><span class="sxs-lookup"><span data-stu-id="b33fd-138">Update the dependencies by running the following command:</span></span>

```bash
composer update
```

### <a name="start-the-authentication-flow"></a><span data-ttu-id="b33fd-139">开始身份验证流</span><span class="sxs-lookup"><span data-stu-id="b33fd-139">Start the authentication flow</span></span>

1. <span data-ttu-id="b33fd-p107">打开**资源** > **视图** >  **welcome.blade.php** 文件。用以下代码替换 **title** div 元素。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p107">Open the **resources** > **views** > **welcome.blade.php** file. Replace the **title** div element with the following code.</span></span>
    ```html
    <div class="title" onClick="window.location='/oauth'">Sign in to Microsoft</div>
    ```
    
2. <span data-ttu-id="b33fd-p108">在 **app** > **Http** > **routes.php** 文件上键入提示 `Illuminate\Http\Request` 类。在任何路由声明前面添加以下行。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p108">Type-hint the `Illuminate\Http\Request` class on the **app** > **Http** > **routes.php** file. Add the following line before any route declaration.</span></span>
    ```php
    use Illuminate\Http\Request;
    ```
    
3. <span data-ttu-id="b33fd-p109">将 */oauth* 路由添加到 **app** > **Http** > **routes.php** 文件。若要添加路由，请在默认路由声明后复制以下代码。将应用的**应用程序 ID** 和**密码**插入到分别标记为 **\<YOUR_APPLICATION_ID\>** 和 **\<YOUR_PASSWORD\>** 的占位符中。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p109">Add an */oauth* route to the **app** > **Http** > **routes.php** file. To add the route, copy the following code after the default route declaration. Insert the **application ID** and **password** of your app in the placeholder marked with **\<YOUR_APPLICATION_ID\>** and **\<YOUR_PASSWORD\>** respectively.</span></span>
    ```php
    Route::get('/oauth', function () {
        $provider = new \League\OAuth2\Client\Provider\GenericProvider([
            'clientId'                => '<YOUR_APPLICATION_ID>',
            'clientSecret'            => '<YOUR_PASSWORD>',
            'redirectUri'             => 'http://localhost:8000/oauth',
            'urlAuthorize'            => 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize',
            'urlAccessToken'          => 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
            'urlResourceOwnerDetails' => '',
            'scopes'                  => 'openid mail.send'
        ]);

        if (!$request->has('code')) {
            return redirect($provider->getAuthorizationUrl());
        }
    });
    ```
    
<span data-ttu-id="b33fd-p110">此时，应该会有一个显示*登录到 Microsoft* 的 PHP 应用。如果单击文本，该应用会显示 Microsoft 登录页。下一步是处理授权服务器发送到重定向 URI 的代码，并用它来交换访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p110">At this point, you should have a PHP app that displays *Sign in to Microsoft*. If you click the text, the app presents the Microsoft sign-in page. The next step is to handle the code that the authorization server sends to the redirect URI and exchange it for an access token.</span></span>

### <a name="exchange-the-authorization-code-for-an-access-token"></a><span data-ttu-id="b33fd-150">用授权代码交换访问令牌</span><span class="sxs-lookup"><span data-stu-id="b33fd-150">Exchange the authorization code for an access token</span></span>

<span data-ttu-id="b33fd-151">需要处理授权服务器的响应，其中包含可交换访问令牌的代码。</span><span class="sxs-lookup"><span data-stu-id="b33fd-151">You need to handle the authorization server response, which contains a code that you can exchange for an access token.</span></span>

<span data-ttu-id="b33fd-p111">更新 */oauth* 路由，以便它可以使用授权代码获取访问令牌。若要执行此操作，请打开 **app** > **Http** > **routes.php** 文件并将以下 *else* 条件子句添加到现有的 *if* 语句。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p111">Update the */oauth* route so it can get an access token with the authorization code. To do this, open the **app** > **Http** > **routes.php** file and add the following *else* conditional clause to the existing *if* statement.</span></span>

```php
if (!$request->has('code')) {
    ...
    // add the following lines
} else {
    $accessToken = $provider->getAccessToken('authorization_code', [
        'code'     => $request->input('code')
    ]);
    exit($accessToken->getToken());
}
```
    
<span data-ttu-id="b33fd-p112">请注意，在行 `exit($accessToken->getToken());` 中有一个访问令牌。现在可以添加代码调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p112">Note that you have an access token in this line: `exit($accessToken->getToken());`. Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph-using-rest"></a><span data-ttu-id="b33fd-156">使用 REST 调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b33fd-156">Call Microsoft Graph using REST</span></span>
<span data-ttu-id="b33fd-p113">可以使用 REST 调用 Microsoft Graph。用以下代码替换行 `exit($accessToken->getToken());`。将电子邮件地址插入标记为 **\<YOUR_EMAIL_ADDRESS\>** 的占位符中。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p113">You can call Microsoft Graph using REST. Replace the line `exit($accessToken->getToken());` with the following code. Insert your email address in the placeholder marked with **\<YOUR_EMAIL_ADDRESS\>**.</span></span>

```php
$client = new \GuzzleHttp\Client();

$email = "{
    Message: {
    Subject: 'Sent using the Microsoft Graph REST API',
    Body: {
        ContentType: 'text',
        Content: 'This is the email body'
    },
    ToRecipients: [
        {
            EmailAddress: {
            Address: '<YOUR_EMAIL_ADDRESS>'
            }
        }
    ]
    }}";

$response = $client->request('POST', 'https://graph.microsoft.com/v1.0/me/sendmail', [
    'headers' => [
        'Authorization' => 'Bearer ' . $accessToken->getToken(),
        'Content-Type' => 'application/json;odata.metadata=minimal;odata.streaming=true'
    ],
    'body' => $email
]);
if($response.getStatusCode() === 201) {
    exit('Email sent, check your inbox');
} else {
    exit('There was an error sending the email. Status code: ' . $response.getStatusCode());
}
```

## <a name="run-the-app"></a><span data-ttu-id="b33fd-160">运行应用</span><span class="sxs-lookup"><span data-stu-id="b33fd-160">Run the app</span></span>
<span data-ttu-id="b33fd-161">现在可以尝试运行 PHP 应用。</span><span class="sxs-lookup"><span data-stu-id="b33fd-161">You're ready to try your PHP app.</span></span>

1. <span data-ttu-id="b33fd-162">在 shell 中，键入以下命令：</span><span class="sxs-lookup"><span data-stu-id="b33fd-162">In your shell, type the following command:</span></span>
    ```bash
    php artisan serve
    ```
    
2. <span data-ttu-id="b33fd-163">转到 Web 浏览器中的 `http://localhost:8000`。</span><span class="sxs-lookup"><span data-stu-id="b33fd-163">Go to `http://localhost:8000` in your web browser.</span></span>
3. <span data-ttu-id="b33fd-164">选择“**登录到 Microsoft**”。</span><span class="sxs-lookup"><span data-stu-id="b33fd-164">Choose **Sign in to Microsoft**.</span></span>
4. <span data-ttu-id="b33fd-165">使用你的个人、工作或学校帐户登录，并授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="b33fd-165">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

<span data-ttu-id="b33fd-p114">检查在 [使用 REST 调用 Microsoft Graph](#call-microsoft-graph-using-rest) 部分中配置的电子邮件地址的收件箱。你应该会收到一封用于登录该应用的帐户所发送的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b33fd-p114">Check the inbox of the email address that you configured in [Call the Microsoft Graph using REST](#call-microsoft-graph-using-rest) section. You should have an email from the account that you used to sign in to the app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b33fd-168">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b33fd-168">Next steps</span></span>
- <span data-ttu-id="b33fd-169">试用 [Microsoft Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="b33fd-169">Try out the [Microsoft Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


## <a name="see-also"></a><span data-ttu-id="b33fd-170">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b33fd-170">See also</span></span>
* [<span data-ttu-id="b33fd-171">Azure AD v2.0 协议</span><span class="sxs-lookup"><span data-stu-id="b33fd-171">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
* [<span data-ttu-id="b33fd-172">Azure AD v2.0 令牌</span><span class="sxs-lookup"><span data-stu-id="b33fd-172">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
