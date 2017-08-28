# <a name="get-started-with-microsoft-graph-in-a-ruby-on-rails-app"></a><span data-ttu-id="3c0cb-101">在 Ruby on Rails 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3c0cb-101">Get started with Microsoft Graph in a Ruby on Rails app</span></span>

<span data-ttu-id="3c0cb-p101">本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成 [Microsoft Graph Ruby on Rails Connect 示例](https://github.com/microsoftgraph/ruby-connect-rest-sample) 的步骤，并说明使用 Microsoft Graph 要实现的主要概念。本文还介绍了如何使用 REST 直接调用来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample) and explains the main concepts that you implement to use the Microsoft Graph. The article also describes how to access Microsoft Graph by using direct REST calls.</span></span>

<span data-ttu-id="3c0cb-105">若要下载使用 Azure AD 终结点的 Connect 示例版本，请参阅 [Microsoft Graph Ruby on Rails Connect 示例](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth)。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-105">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).</span></span>

<span data-ttu-id="3c0cb-106">下图显示了将要创建的应用。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-106">The following image shows the app you'll create.</span></span> 

![Microsoft Ruby on Rails Connect 示例屏幕截图](./images/Microsoft-Graph-Ruby-Connect-UI.png)

<span data-ttu-id="3c0cb-p102">**不想生成一个应用吗？**使用 [Microsoft Graph 快速入门](https://graph.microsoft.io/en-us/getting-started) 快速准备就绪并开始运行，或者下载本文基于的 [Ruby REST Connect 示例](https://github.com/microsoftgraph/ruby-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast, or download the [Ruby REST Connect sample](https://github.com/microsoftgraph/ruby-connect-rest-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="3c0cb-110">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c0cb-110">Prerequisites</span></span>

<span data-ttu-id="3c0cb-111">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="3c0cb-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="3c0cb-112">Ruby 2.1，用于在开发服务器上运行该示例。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-112">Ruby 2.1 to run the sample on a development server.</span></span>
- <span data-ttu-id="3c0cb-113">Rails 框架（该示例已经过 Rails 4.2 测试）。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-113">Rails framework (the sample has been tested on Rails 4.2).</span></span>
- <span data-ttu-id="3c0cb-114">捆绑程序依存关系管理器</span><span class="sxs-lookup"><span data-stu-id="3c0cb-114">Bundler dependency manager.</span></span>
- <span data-ttu-id="3c0cb-115">用于 Ruby 的 Rack Web 服务器界面。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-115">Rack web server interface for Ruby.</span></span>
- <span data-ttu-id="3c0cb-116">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="3c0cb-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="3c0cb-p103">适用于 Ruby on Rails 的 Microsoft Graph Connect 初学者项目。下载 [Microsoft Graph Ruby on Rails Connect 示例](https://github.com/microsoftgraph/ruby-connect-rest-sample)。初学者项目位于“初学者”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p103">The Microsoft Graph Connect Starter Project for Ruby on Rails. Download the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample). The starter project is located in the _starter_ folder.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="3c0cb-120">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="3c0cb-120">Register the application</span></span>

<span data-ttu-id="3c0cb-p104">在 Microsoft 应用注册门户上注册一个应用。这将生成应用程序 ID 和机密，然后你将用它们配置要进行身份验证的应用。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and secret that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="3c0cb-123">使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-123">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="3c0cb-124">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-124">Choose **Add an app**.</span></span>

3. <span data-ttu-id="3c0cb-125">输入应用的名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-125">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="3c0cb-126">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-126">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="3c0cb-p105">复制应用程序 ID。这是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p105">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="3c0cb-p106">在“**应用程序机密**”下，选择“**生成新密码**”。从“**生成的新密码**”对话中复制应用机密。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog.</span></span>

    <span data-ttu-id="3c0cb-131">将使用此应用程序 ID 和应用机密配置应用。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-131">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="3c0cb-132">在“**平台**”下，选择“**添加平台**” > “**Web**”。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-132">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="3c0cb-133">请确保已选中“**允许隐式流**”复选框，输入 *http://localhost:3000/auth/microsoft_v2_auth/callback* 作为重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-133">Make sure the **Allow Implicit Flow** check box is selected, and enter *http://localhost:3000/auth/microsoft_v2_auth/callback* as the Redirect URI.</span></span>

    <span data-ttu-id="3c0cb-p107">“允许隐式流”选项启用 OpenID Connect 混合流。在身份验证过程中，这可使应用同时接收登录信息 (id_token) 以及应用用来获取访问令牌的项目（在这种情况下，项目为授权代码）。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p107">The Allow Implicit Flow option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

    <span data-ttu-id="3c0cb-136">重定向 URL *http://localhost:3000/auth/microsoft_v2_auth/callback* 是 OmniAuth 中间件处理身份验证请求后进行配置所要使用的值。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-136">The redirect URI *http://localhost:3000/auth/microsoft_v2_auth/callback* is the value that the OmniAuth middleware is configured to use once it has processed the authentication request.</span></span>

8. <span data-ttu-id="3c0cb-137">选择“**保存**”。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-137">Choose **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="3c0cb-138">配置项目</span><span class="sxs-lookup"><span data-stu-id="3c0cb-138">Configure the project</span></span>

1. <span data-ttu-id="3c0cb-p108">下载或克隆 [Microsoft Graph Ruby on Rails Connect 示例](https://github.com/microsoftgraph/ruby-connect-rest-sample)。在自己选择的编辑器中打开“_初学者_”文件夹。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p108">Download or clone the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample). Open the _starter_ folder in the editor of your choice.</span></span>
1. <span data-ttu-id="3c0cb-141">如果你还没有捆绑程序和机架，请使用以下命令进行安装。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-141">If you don't already have bundler and rack, you can install them with the following command.</span></span>

    ```
    gem install bundler rack
    ```
2. <span data-ttu-id="3c0cb-142">在 config/environment.rb 文件中执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3c0cb-142">In the config/environment.rb file, do the following:</span></span>
    - <span data-ttu-id="3c0cb-143">用所注册应用程序的客户端 ID 替换 *ENTER_YOUR_CLIENT_ID*。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-143">Replace *ENTER_YOUR_CLIENT_ID* with the client ID of your registered  application.</span></span>
    - <span data-ttu-id="3c0cb-144">用所注册的应用程序的密钥替换 *ENTER_YOUR_SECRET*。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-144">Replace *ENTER_YOUR_SECRET* with the key of your registered application.</span></span>

3. <span data-ttu-id="3c0cb-145">使用以下命令安装 Rails 应用程序和依存关系。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-145">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="3c0cb-146">对用户进行身份验证并获取一个访问令牌</span><span class="sxs-lookup"><span data-stu-id="3c0cb-146">Authenticate the user and get an access token</span></span>

<span data-ttu-id="3c0cb-p109">此应用使用授权代码授予流和委派用户身份。对于 Web 应用程序，该流需要已注册应用的应用程序 ID、机密和重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="3c0cb-149">身份验证流可以划分为以下几个基本步骤：</span><span class="sxs-lookup"><span data-stu-id="3c0cb-149">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="3c0cb-150">重定向用户以进行身份验证并获得许可</span><span class="sxs-lookup"><span data-stu-id="3c0cb-150">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="3c0cb-151">获取授权代码</span><span class="sxs-lookup"><span data-stu-id="3c0cb-151">Get an authorization code</span></span>
3. <span data-ttu-id="3c0cb-152">兑换访问令牌的授权代码</span><span class="sxs-lookup"><span data-stu-id="3c0cb-152">Redeem the authorization code for an access token</span></span>

><span data-ttu-id="3c0cb-153">有关该身份验证流的详细信息，请参阅 Azure AD 文档中的 [Web 应用程序到 Web API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) 和 [使用 OpenID Connect 将 Microsoft 身份和 Microsoft Graph 集成到 Web 应用程序中](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-153">For more information about this auth flow, see [Web application to web API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) and  [Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) in the Azure AD documentation.</span></span>

<span data-ttu-id="3c0cb-154">我们将使用具有三个 [Rack](http://rack.github.io/) 中间件的堆栈来使应用对 Microsoft Graph 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-154">We'll be using a stack of three pieces of [Rack](http://rack.github.io/) middleware to enable the app to authenticate against the Microsoft Graph:</span></span>

- <span data-ttu-id="3c0cb-155">[OmniAuth](https://rubygems.org/gems/omniauth) 用于进行多个提供程序身份验证的通用 Rack 框架。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-155">[OmniAuth](https://rubygems.org/gems/omniauth), a generalized Rack framework for multiple-provider authentication.</span></span>
- <span data-ttu-id="3c0cb-156">[Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2) 用于 OmniAuth 的抽象 OAuth2 策略。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-156">[Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), an abstract OAuth2 strategy for OmniAuth.</span></span> 
- <span data-ttu-id="3c0cb-p110">omniauth-microsoft_v2_auth，一种 OmniAuth 策略，可自定义 Omniauth-oauth2 以专门对 Azure AD v2.0 终结点提供身份验证。此项目包含在代码示例中。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p110">omniauth-microsoft_v2_auth, an OmniAuth strategy that customizes Omniauth-oauth2 to specifically provide authentication against the Azure AD v2.0 endpoint. This project is included in the code sample.</span></span>

### <a name="specify-gem-dependencies-for-authentication"></a><span data-ttu-id="3c0cb-159">指定用于身份验证的 gem 依赖项</span><span class="sxs-lookup"><span data-stu-id="3c0cb-159">Specify gem dependencies for authentication</span></span>

<span data-ttu-id="3c0cb-160">在 Gemfile 中，取消评论以下 gem 以将其添加为依赖项。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-160">In Gemfile, uncomment the following gems to add them as dependencies.</span></span>

    ```
    gem 'omniauth'
    gem 'omniauth-oauth2'
    gem 'omniauth-microsoft_v2_auth', path: './omniauth-microsoft_v2_auth'
    ```

<span data-ttu-id="3c0cb-161">注意 `omniauth-microsoft_v2_auth` 包含在应用项目中，并且会通过指定的路径进行安装。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-161">Note that `omniauth-microsoft_v2_auth` is included in the app project, and will be installed from the path specified.</span></span> 

### <a name="configure-the-authentication-middleware"></a><span data-ttu-id="3c0cb-162">配置身份验证中间件</span><span class="sxs-lookup"><span data-stu-id="3c0cb-162">Configure the authentication middleware</span></span>

<span data-ttu-id="3c0cb-163">在 `config/initializers/omniauth-microsoft_v2_auth.rb` 中，取消评论下列行。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-163">In `config/initializers/omniauth-microsoft_v2_auth.rb`, uncomment the following lines.</span></span>

    ```
    Rails.application.config.middleware.use OmniAuth::Builder do
      provider :microsoft_v2_auth,
      ENV['CLIENT_ID'],
      ENV['CLIENT_SECRET'],
      :scope => ENV['SCOPE']
    end
    ```
<span data-ttu-id="3c0cb-p111">这将配置 OmniAuth 中间件，其中包括指定要使用的应用程序 ID 和应用机密及用户要请求的范围。以下是之前在 `config/environment.rb` 指定的值。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p111">This configures the OmniAuth middleware, including specifying the app ID and app secret to use, as well as the scopes to request for the user. These are the values you specified earlier in `config/environment.rb`.</span></span>

### <a name="specify-routes-for-authentication"></a><span data-ttu-id="3c0cb-166">指定身份验证的路由</span><span class="sxs-lookup"><span data-stu-id="3c0cb-166">Specify routes for authentication</span></span>

<span data-ttu-id="3c0cb-p112">现在我们需要指定身份验证流必需的两个路由。第一个路由将身份验证请求转发至 OmniAuth 中间件，第二个路由指定发生身份验证后 OmniAuth 应在应用中重定向到的位置。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p112">Now we need to specify two routes necessary for the authentication flow. The first route forwards the authentication request to the OmniAuth middleware, and the second specifies the location in the app to which OmniAuth should redirect once authentication has occurred.</span></span>

<span data-ttu-id="3c0cb-169">在 `config/routes.rb` 中，取消评论以下理由指令。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-169">In `config/routes.rb`, uncomment the following route directive.</span></span>

    get '/login', to: 'pages#login'

<span data-ttu-id="3c0cb-170">这会将登录请求定向到页面控制器的 `login` 方法，该方法会将请求重定向至 omniauth-microsoft_v2_auth 中间件。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-170">This directs login requests to the pages controller's `login` method, which in turn redirects the request to the omniauth-microsoft_v2_auth middleware.</span></span>

    def login
        redirect_to '/auth/microsoft_v2_auth'
    end

<span data-ttu-id="3c0cb-p113">接下来，我们需要指定发生身份验证后 OmniAuth 应在应用中重定向到的位置。取消评论以下路由。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p113">Next, we need to specify where in the app OmniAuth should redirect once authentication has occurred. Uncomment the following route.</span></span>

    match '/auth/:provider/callback', to: 'pages#callback', via: [:get, :post]

<span data-ttu-id="3c0cb-p114">OmniAuth 完成对用户的身份验证后，会调用应用注册中指定的重定向 URL；在此示例中为 *http://localhost:3000/auth/microsoft_v2_auth/callback*。上述路由模式与该 URL 匹配，因此会将请求路由至页面控制器的 `callback` 方法。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p114">When OmniAuth has finished authenticating the user, it calls the redirect URL specified in the app registration; in this case, *http://localhost:3000/auth/microsoft_v2_auth/callback*. The route pattern above matches that URL and so routes the request to the page controller's `callback` method.</span></span>

### <a name="get-an-access-token"></a><span data-ttu-id="3c0cb-175">获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="3c0cb-175">Get an access token</span></span>

<span data-ttu-id="3c0cb-176">接下来，我们将添加在用户成功登录后实际启动身份验证进程和检索访问令牌的代码。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-176">Next, we'll add the code that actually starts the authentication process, and retrieves the access token once the user has successfully signed in.</span></span>

<span data-ttu-id="3c0cb-p115">请查看 `app/views/pages/index.html.erb`，网站根目录视图。视图包括可允许用户登录的单个按钮。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p115">Take a look at `app/views/pages/index.html.erb`, the view for the site root. The view includes a single button, which enables users to sign in.</span></span>

    <button class="ms-Button" onclick="window.location.href = '/login'">
        <span class="ms-Button-label"><%= t('connect_button') %></span>
    </button>

<span data-ttu-id="3c0cb-p116">如上所示，登录方法重定向至已配置应用程序 ID 和应用机密及用户要请求的范围的 OmniAuth 中间件。用户成功完成身份验证后，OmniAuth 将带有访问令牌和其他用户信息的哈希返回至应用。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p116">As shown earlier, the login method redirects to the OmniAuth middleware, which has been configured with the app ID and app secret, as well as the scopes to request for the user. Once the user is successfully authenticated, OmniAuth returns a hash with the access token and other user information to the app.</span></span>

<span data-ttu-id="3c0cb-181">现在可以添加代码来处理 OmniAuth 回叫，并通过该哈希检索信息。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-181">Now let's add code to handle the OmniAuth callback, and retrieve information from that hash.</span></span> 

<span data-ttu-id="3c0cb-182">在 `app/controllers/pages_controller.rb` 中，用以下代码替换空的 `callback` 方法。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-182">In `app/controllers/pages_controller.rb`, replace the empty `callback` method with the following code.</span></span>

    ```
    def callback
        # Access the authentication hash for omniauth
        # and extract the auth token, user name, and email
        data = request.env['omniauth.auth']
    
        @email = data[:extra][:raw_info][:userPrincipalName]
        @name = data[:extra][:raw_info][:displayName]

        # Associate token/user values to the session
        session[:access_token] = data['credentials']['token']
        session[:name] = @name
        session[:email] = @email
        
        # Debug logging
        logger.info "Name: #{@name}"
        logger.info "Email: #{@email}"
        logger.info "[callback] - Access token: #{session[:access_token]}"
    end

    ```

<span data-ttu-id="3c0cb-183">该方法会检索身份验证哈希，然后存储当前会话中的访问令牌、用户名和电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-183">This method retrieves the authentication hash, and then stores the access token, user name, and email in the current session.</span></span>

> <span data-ttu-id="3c0cb-p117">**注意：**本项目中的简单身份验证和令牌处理操作仅用于说明目的。在生产应用中，可能会构建更为可靠的方法来处理身份验证，其中包括安全令牌处理和令牌刷新。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p117">**Note:** The simple authentication  and token handling in this project is presented for illustrative purposes only. In a production app, you would likely construct a more robust way of handling authentication, including secure token handling and token refresh.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="3c0cb-186">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3c0cb-186">Call Microsoft Graph</span></span>

<span data-ttu-id="3c0cb-187">现在可以添加代码调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-187">Now you're ready to add code to call Microsoft Graph.</span></span> 

<span data-ttu-id="3c0cb-p118">由 `callback` 方法 (`app/views/pages/callback.html.erb`) 呈现的视图包含带有单一按钮的简单窗体。该窗体会发布到 `send_mail`，并且其中包含单一参数、预设收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p118">The view rendered by the `callback` method (`app/views/pages/callback.html.erb`) includes a simple form with a single button. The form posts to  `send_mail`, and includes a single parameter, the email address of the intended recipient.</span></span>
    
    ``` 
    <form action="../../send_mail" method="post">
      <div class="ms-Grid-col ms-u-mdPush1 ms-u-md9 ms-u-lgPush1 ms-u-lg6">
        ...
            <div class="ms-TextField">
               <input class="ms-TextField-field" name="specified_email" value="<%= @email %>">
            </div>
            <button class="ms-Button">
            <span class="ms-Button-label"><i class="ms-Icon ms-Icon--mail" aria-hidden="true"></i><%= t('send_mail_button') %></span>
            </button> 
        ...
    ```

<span data-ttu-id="3c0cb-190">在 `app/controllers/pages_controller.rb` 中，用以下代码替换空的 `send_mail` 方法。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-190">In `app/controllers/pages_controller.rb`, replace the empty `send_mail` method with the following code.</span></span>

    ```
    def send_mail
        logger.debug "[send_mail] - Access token: #{session[:access_token]}"
        
        # Used in the template
        @name = session[:name]
        @email = params[:specified_email]
        @recipient = params[:specified_email]
        @mail_sent = false
        
        send_mail_endpoint = URI("#{GRAPH_RESOURCE}#{SENDMAIL_ENDPOINT}")
        content_type = CONTENT_TYPE
        http = Net::HTTP.new(send_mail_endpoint.host, send_mail_endpoint.port)
        http.use_ssl = true
        
        # If you want to use a sniffer tool, like Fiddler, to see the request
        # you might need to add this line to tell the engine not to verify the
        # certificate or you might see a "certificate verify failed" error
        # http.verify_mode = OpenSSL::SSL::VERIFY_NONE
        
        email_body = File.read('app/assets/MailTemplate.html')
        email_body.sub! '{given_name}', @name
        email_subject = t('email_subject')
        
        logger.debug email_body
    
        email_message = "{
            Message: {
            Subject: '#{email_subject}',
            Body: {
                ContentType: 'HTML',
                Content: '#{email_body}'
            },
            ToRecipients: [
                {
                    EmailAddress: {
                        Address: '#{@recipient}'
                    }
                }
            ]
            },
            SaveToSentItems: true
            }"
            
        response = http.post(
            SENDMAIL_ENDPOINT,
            email_message,
            'Authorization' => "Bearer #{session[:access_token]}",
            'Content-Type' => content_type
        )
        
        logger.debug "Code: #{response.code}"
        logger.debug "Message: #{response.message}"
        
        # The send mail endpoint returns a 202 - Accepted code on success
        if response.code == '202'
            @mail_sent = true
        else
            @mail_sent = false
            flash[:httpError] = "#{response.code} - #{response.message}"
        end
        
        render 'callback'
    end
    ```

<span data-ttu-id="3c0cb-191">该代码会构建 HTTP 请求，设置电子邮件的格式，然后调用 Microsoft Graph 发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-191">This code constructs the HTTP request, formats the email, and then calls Microsoft Graph to send the email.</span></span>

<span data-ttu-id="3c0cb-p119">若要创建电子邮件，代码会通过窗体传递的参数中的会话令牌和收件人电子邮件地址拉取用户名。然后代码会在项目所包含的模板中读取电子邮件正文，插入用户名和电子邮件地址，并将电子邮件文本附加为 HTTP 请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

<span data-ttu-id="3c0cb-194">若要发送电子邮件，代码会构建 HTTP 请求，将访问令牌附加为授权标头，然后将请求发布至发送电子邮件终结点。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="3c0cb-195">最后，代码会使用返回的 HTTP 响应代码来通知用户电子邮件是否发送成功。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="3c0cb-196">运行应用</span><span class="sxs-lookup"><span data-stu-id="3c0cb-196">Run the app</span></span>

1. <span data-ttu-id="3c0cb-197">使用以下命令安装 Rails 应用程序和依存关系。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="3c0cb-198">要启动 Rails 应用程序，请键入以下命令。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="3c0cb-199">转到 Web 浏览器中的 `http://localhost:3000`。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="3c0cb-200">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3c0cb-200">See also</span></span>
- <span data-ttu-id="3c0cb-201">使用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 试用 REST API。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-201">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="3c0cb-202">在 GitHub 上了解我们的其他 [Microsoft Graph 示例](https://github.com/microsoftgraph)。</span><span class="sxs-lookup"><span data-stu-id="3c0cb-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>


