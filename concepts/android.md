# <a name="get-started-with-microsoft-graph-in-an-android-app"></a><span data-ttu-id="60856-101">在 Android 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="60856-101">Get started with Microsoft Graph in an Android app</span></span>

> <span data-ttu-id="60856-p101">**为企业客户生成应用？** 如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。</span><span class="sxs-lookup"><span data-stu-id="60856-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="60856-p102">若要跨**所有企业方案**支持**全部企业客户**，必须使用 Azure AD 终结点，并使用 [Azure 门户](https://aka.ms/aadapplist)管理应用。有关详细信息，请参阅[在 Azure AD 和 Azure AD v2.0 终结点之间进行选择](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="60856-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="60856-p103">本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)的步骤，并说明实现在面向 Android 的应用中使用 Microsoft Graph 的主要概念。本文还介绍如何通过使用[用于 Android 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-android) 或原始 REST 调用来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="60856-p103">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and explains the main concepts that you implement to use Microsoft Graph in your app for Android. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) or raw REST calls.</span></span>

<span data-ttu-id="60856-110">若要在 Android 版应用中使用 Microsoft Graph，需要向用户显示 Microsoft 登录页，如以下屏幕截图所示。</span><span class="sxs-lookup"><span data-stu-id="60856-110">To use Microsoft Graph in your app for Android, you need to show the Microsoft sign-in page to your users, as shown in the following screenshot.</span></span>

![Android 上的 Microsoft 帐户登录页](images/AndroidConnect.png)

<br/>

<span data-ttu-id="60856-p104">**不想生成一个应用吗？** 通过下载本文所基于的 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)快速准备就绪并开始运行。</span><span class="sxs-lookup"><span data-stu-id="60856-p104">**Don't feel like building an app?** Get up and running fast by downloading the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="60856-114">先决条件</span><span class="sxs-lookup"><span data-stu-id="60856-114">Prerequisites</span></span>

<span data-ttu-id="60856-115">若要开始，将需要以下各项：</span><span class="sxs-lookup"><span data-stu-id="60856-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="60856-116">一个 [Microsoft 帐户](https://www.outlook.com/) 或者一个[工作或学校帐户](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="60856-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="60856-117">Android Studio 2.0 或更高版本</span><span class="sxs-lookup"><span data-stu-id="60856-117">Android Studio 2.0 or newer version</span></span>


## <a name="configure-a-new-project"></a><span data-ttu-id="60856-118">配置新项目</span><span class="sxs-lookup"><span data-stu-id="60856-118">Configure a new project</span></span>

<span data-ttu-id="60856-119">如果已下载 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)，请跳过这一步。</span><span class="sxs-lookup"><span data-stu-id="60856-119">If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample), skip this step.</span></span> 

<span data-ttu-id="60856-120">在 Android Studio 中，启动一个新项目。</span><span class="sxs-lookup"><span data-stu-id="60856-120">Start a new project in Android Studio.</span></span> <span data-ttu-id="60856-121">可以保留大多数向导的默认值，只要选择下列选项即可：</span><span class="sxs-lookup"><span data-stu-id="60856-121">You can leave the default values for most of the wizard; just make sure to choose the following options:</span></span>

- <span data-ttu-id="60856-122">目标 Android 设备：**手机和平板电脑**</span><span class="sxs-lookup"><span data-stu-id="60856-122">Target Android Devices: **Phone and Tablet**</span></span>
- <span data-ttu-id="60856-123">最低 SDK：**API 16:Android 4.1 (Jelly Bean)**</span><span class="sxs-lookup"><span data-stu-id="60856-123">Minimum SDK: **API 16: Android 4.1 (Jelly Bean)**</span></span>
- <span data-ttu-id="60856-124">将活动添加到移动设备：**基本活动**</span><span class="sxs-lookup"><span data-stu-id="60856-124">Add an Activity to Mobile: **Basic Activity**</span></span>
 
<span data-ttu-id="60856-125">这样，可以创建包含活动和用户身份验证按钮的 Android 项目。</span><span class="sxs-lookup"><span data-stu-id="60856-125">This provides you with an Android project with an activity and a button that you can use to authenticate the user.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="60856-126">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="60856-126">Register the application</span></span>

<span data-ttu-id="60856-127">需要在 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)中注册应用，无论是已下载连接示例还是创建了新项目。</span><span class="sxs-lookup"><span data-stu-id="60856-127">You need to register your app on the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) whether you've downloaded the connect sample or created a new project.</span></span>

<span data-ttu-id="60856-p106">在 Microsoft 应用注册门户上注册一个应用。这会生成用于配置此应用的应用 ID。</span><span class="sxs-lookup"><span data-stu-id="60856-p106">Register an app on the Microsoft App Registration Portal. This generates the app ID that you'll use to configure the app.</span></span>

1. <span data-ttu-id="60856-130">使用个人帐户/工作或学校帐户，登录 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="60856-130">Sign in to the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) by using either your personal or work or school account.</span></span>

2. <span data-ttu-id="60856-131">选择“**添加应用**”。</span><span class="sxs-lookup"><span data-stu-id="60856-131">Select **Add an app**.</span></span>

    > <span data-ttu-id="60856-132">**提示：** 如果已下载 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)并刚为其创建注册，请先取消选中“引导式安装”**** 复选框，再选择“创建”**** 按钮。</span><span class="sxs-lookup"><span data-stu-id="60856-132">**Tip:** If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and are just creating a registration for it, clear the **Guided Setup** check box before selecting the **Create** button.</span></span>

3. <span data-ttu-id="60856-133">输入应用名称，再选择“创建”****。</span><span class="sxs-lookup"><span data-stu-id="60856-133">Enter a name for the app, and then select **Create**.</span></span> 
    
    <span data-ttu-id="60856-134">对于“引导式安装”**** 流：</span><span class="sxs-lookup"><span data-stu-id="60856-134">For the  **Guided Setup** flow:</span></span>
 
    <span data-ttu-id="60856-135">a.</span><span class="sxs-lookup"><span data-stu-id="60856-135">a.</span></span> <span data-ttu-id="60856-136">选择“移动和桌面应用”****，定义要创建的应用类型。</span><span class="sxs-lookup"><span data-stu-id="60856-136">Select **Mobile and Desktop App** to define the kind of app you are creating.</span></span>

    <span data-ttu-id="60856-137">b.</span><span class="sxs-lookup"><span data-stu-id="60856-137">b.</span></span> <span data-ttu-id="60856-138">选择“Android”****，定义要使用的移动技术。</span><span class="sxs-lookup"><span data-stu-id="60856-138">Select **Android** to define the mobile technology you are using.</span></span>

    <span data-ttu-id="60856-139">c.</span><span class="sxs-lookup"><span data-stu-id="60856-139">c.</span></span> <span data-ttu-id="60856-140">查看入门主题。完成后，选择页面底部的“安装”**** 按钮。</span><span class="sxs-lookup"><span data-stu-id="60856-140">Review the introductory topic, and when finished, select the **Setup** button at the end of the page.</span></span>

    <span data-ttu-id="60856-p110">d.根据有关“设置”**** 步骤的说明，将 MSAL 库添加到应用 build.gradle 中。</span><span class="sxs-lookup"><span data-stu-id="60856-p110">d. Follow the instructions on the **Setup** step to add the MSAL library to your app build.gradle.</span></span>

    <span data-ttu-id="60856-143">e.</span><span class="sxs-lookup"><span data-stu-id="60856-143">e.</span></span> <span data-ttu-id="60856-144">按照“使用”**** 步骤中的说明操作，将 MSAL 逻辑添加到新项目中。</span><span class="sxs-lookup"><span data-stu-id="60856-144">Follow the directions on the **Use** step to add MSAL logic to your new project.</span></span>

    <span data-ttu-id="60856-p112">f.在“配置”**** 页上，门户已为你创建唯一的应用程序 ID。使用它来配置应用。</span><span class="sxs-lookup"><span data-stu-id="60856-p112">f. On the **Configure** page, the portal has created a unique application ID for you. Use it to configure your app.</span></span>

    <br/>
    
    <span data-ttu-id="60856-148">对于非引导流：</span><span class="sxs-lookup"><span data-stu-id="60856-148">For the unguided flow:</span></span>

    <span data-ttu-id="60856-149">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="60856-149">The registration page displays, listing the properties of your app.</span></span>

    <span data-ttu-id="60856-p113">a.复制应用程序 ID。这是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="60856-p113">a. Copy the application ID. This is the unique identifier for your app.</span></span> 

    <span data-ttu-id="60856-153">b.</span><span class="sxs-lookup"><span data-stu-id="60856-153">b.</span></span> <span data-ttu-id="60856-154">选择“添加平台”**** 和“原生应用”****。</span><span class="sxs-lookup"><span data-stu-id="60856-154">Select **Add Platform** and **Native Application**.</span></span>

      > <span data-ttu-id="60856-155">**注意：** 应用注册门户提供值为 `msalENTER_YOUR_CLIENT_ID://auth` 的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="60856-155">**Note:** The Application Registration Portal provides a redirect URI with a value of `msalENTER_YOUR_CLIENT_ID://auth`.</span></span> <span data-ttu-id="60856-156">请勿使用内置的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="60856-156">Do not use the built-in redirect URIs.</span></span> <span data-ttu-id="60856-157">[Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)实现的 MSAL 身份验证库需要使用此重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="60856-157">The [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) implements the MSAL authentication library that requires this redirect URI.</span></span> <span data-ttu-id="60856-158">如果使用的是[受支持的第三方库](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries)或 **ADAL** 库，必须使用内置的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="60856-158">If you're using a [supported third-party library](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) or the **ADAL** library, you must use the built-in redirect URIs.</span></span>
      
      <span data-ttu-id="60856-159">c.</span><span class="sxs-lookup"><span data-stu-id="60856-159">c.</span></span> <span data-ttu-id="60856-160">添加委托权限。</span><span class="sxs-lookup"><span data-stu-id="60856-160">Add delegated permissions.</span></span> <span data-ttu-id="60856-161">需要 **profile**、**Mail.ReadWrite**、**Mail.Send**、**Files.ReadWrite** 和 **User.ReadBasic.All**。</span><span class="sxs-lookup"><span data-stu-id="60856-161">You'll need **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite**, and **User.ReadBasic.All**.</span></span> 

      <span data-ttu-id="60856-162">d.</span><span class="sxs-lookup"><span data-stu-id="60856-162">d.</span></span> <span data-ttu-id="60856-163">选择“保存”****。</span><span class="sxs-lookup"><span data-stu-id="60856-163">Select **Save**.</span></span>


## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="60856-164">验证用户并获取访问令牌</span><span class="sxs-lookup"><span data-stu-id="60856-164">Authenticate the user and get an access token</span></span>

> <span data-ttu-id="60856-165">**注意：** 如果已按照应用注册门户中“引导式安装”**** 流内的说明操作来新建应用，可以跳过这些步骤。</span><span class="sxs-lookup"><span data-stu-id="60856-165">**Note:** If you followed the instructions in the **Guided Setup** flow from the application registration portal to create a new application, you can skip these steps.</span></span> <span data-ttu-id="60856-166">若要详细了解 Graph API，请参阅[使用 Microsoft Graph SDK 调用 Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk)。</span><span class="sxs-lookup"><span data-stu-id="60856-166">To learn more about the Graph API, see [Call Microsoft Graph using the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk).</span></span>

<span data-ttu-id="60856-167">接下来，将逐步演示 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)，方便大家了解已添加的 MSAL 和 Microsoft Graph 代码。</span><span class="sxs-lookup"><span data-stu-id="60856-167">Let's walk through the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) to learn about the MSAL and Microsoft Graph code we've added.</span></span>

### <a name="add-the-dependency-to-appbuildgradle"></a><span data-ttu-id="60856-168">向 app/build.gradle 添加依赖项</span><span class="sxs-lookup"><span data-stu-id="60856-168">Add the dependency to app/build.gradle</span></span>

<span data-ttu-id="60856-169">在应用模块中打开 `build.gradle` 文件，并查找以下依赖项：</span><span class="sxs-lookup"><span data-stu-id="60856-169">Open the `build.gradle` file in the app module and find the following dependency:</span></span>

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'
```

<br/>

### <a name="start-the-authentication-flow"></a><span data-ttu-id="60856-170">启动身份验证流</span><span class="sxs-lookup"><span data-stu-id="60856-170">Start the authentication flow</span></span>

1. <span data-ttu-id="60856-171">打开“AuthenticationManager”**** 文件，再依次查找“PublicClientApplication”**** 对象声明和“getInstance”**** 方法中的实例化。</span><span class="sxs-lookup"><span data-stu-id="60856-171">Open the **AuthenticationManager** file and find the **PublicClientApplication** object declaration, and then the instantiation in the **getInstance** method.</span></span>

   ```java
    private static PublicClientApplication mPublicClientApplication;
    ....

    public static synchronized AuthenticationManager getInstance() {
        if (INSTANCE == null) {
            INSTANCE = new AuthenticationManager();
            if (mPublicClientApplication == null) {
                mPublicClientApplication = new PublicClientApplication(Connect.getInstance());
            }
        }
        return INSTANCE;
    }

   ```

<br/>

2. <span data-ttu-id="60856-p119">在 **ConnectActivity** 类中，找到 **mConnectButton** 的 click 事件的事件处理程序。查找 **onClick** 方法并审查相关代码。</span><span class="sxs-lookup"><span data-stu-id="60856-p119">In the **ConnectActivity** class, locate the event handler for the click event of the **mConnectButton**. Find the **onClick** method and review relevant code.</span></span>
  
    <span data-ttu-id="60856-174">**connect** 方法支持记录个人身份信息 (PII)，获取示例帮助程序类 **AuthenticationManager** 的实例，并获取 MSAL 平台对象用户集合。</span><span class="sxs-lookup"><span data-stu-id="60856-174">The **connect** method enables personally identifiable information (PII) logging, gets an instance of the sample helper class **AuthenticationManager**, and gets the MSAL platform object users collection.</span></span> <span data-ttu-id="60856-175">如果没有用户，则会对新用户执行 Azure AD 身份验证和授权流。</span><span class="sxs-lookup"><span data-stu-id="60856-175">If there are no users, the new user is taken to the Azure AD authentication and authorization flow.</span></span> <span data-ttu-id="60856-176">否则，以静默方式获取身份验证令牌。</span><span class="sxs-lookup"><span data-stu-id="60856-176">Otherwise, an authentication token is obtained silently.</span></span>

   ```java
    @Override
    public void onClick(View view) {
        ....
        connect();
    }

        private void connect() {

        if (mEnablePiiLogging) {
            Logger.getInstance().setEnablePII(true);
        } else {
            Logger.getInstance().setEnablePII(false);
        }

        AuthenticationManager mgr = AuthenticationManager.getInstance();

        List<User> users = null;

        try {
            users = mgr.getPublicClient().getUsers();

            if (users != null && users.size() == 1) {
                mUser = users.get(0);
                mgr.callAcquireTokenSilent(mUser, true, this);
            } else {
                mgr.callAcquireToken(
                        this,
                        this);
            }
        } catch (MsalClientException e) {
            Log.d(TAG, "MSAL Exception Generated while getting users: " + e.toString());

        } catch (IndexOutOfBoundsException e) {
            Log.d(TAG, "User at this position does not exist: " + e.toString());
        }
    }

   ```
   
<br/>

3. <span data-ttu-id="60856-177">查找事件处理程序，它负责处理 Azure AD 在用户关闭身份验证对话框时生成的 Azure AD 重定向响应。</span><span class="sxs-lookup"><span data-stu-id="60856-177">Find the event handler that processes the Azure AD redirect response generated by Azure AD when the user closes the authentication dialog.</span></span> <span data-ttu-id="60856-178">此处理程序位于 **ConnectActivity** 类中。</span><span class="sxs-lookup"><span data-stu-id="60856-178">This handler is in the **ConnectActivity** class.</span></span>

   ```java
       /**
     * Handles redirect response from https://login.microsoftonline.com/common and
     * notifies the MSAL library that the user has completed the authentication
     * dialog
     * @param requestCode
     * @param resultCode
     * @param data
     */
    @Override
    protected void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if (AuthenticationManager
                .getInstance()
                .getPublicClient() != null) {
            AuthenticationManager
                    .getInstance()
                    .getPublicClient()
                    .handleInteractiveRequestRedirect(requestCode, resultCode, data);
        }
    }

   ```  
   
   <br/>

4. <span data-ttu-id="60856-179">查找缓存用于 Graph API 调用的身份验证令牌的身份验证回调方法。</span><span class="sxs-lookup"><span data-stu-id="60856-179">Find the authentication callback method that caches the authentication token that is used in Graph API calls.</span></span>


```java
    /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

```

<br/>
   
<span data-ttu-id="60856-180">连接示例应用对主要活动使用“连接”**** 按钮。</span><span class="sxs-lookup"><span data-stu-id="60856-180">The connect sample app has a **Connect** button on the main activity.</span></span> <span data-ttu-id="60856-181">如果选择此按钮，应用会在首次使用时通过设备浏览器显示身份验证页。</span><span class="sxs-lookup"><span data-stu-id="60856-181">If you select the button, on first use, the app presents an authentication page using the device's browser.</span></span> <span data-ttu-id="60856-182">下一步是处理授权服务器发送到重定向 URI 的代码，并用它来交换访问令牌。</span><span class="sxs-lookup"><span data-stu-id="60856-182">The next step is to handle the code that the authorization server sends to the redirect URI and exchange it for an access token.</span></span>

### <a name="exchange-the-authorization-code-for-an-access-token"></a><span data-ttu-id="60856-183">用授权代码交换访问令牌</span><span class="sxs-lookup"><span data-stu-id="60856-183">Exchange the authorization code for an access token</span></span>

<span data-ttu-id="60856-184">需要让应用准备就绪，以处理授权服务器的响应，其中包含用于交换访问令牌的代码。</span><span class="sxs-lookup"><span data-stu-id="60856-184">You need to make your app ready to handle the authorization server response, which contains a code that you can exchange for an access token.</span></span>

1. <span data-ttu-id="60856-p123">需要告诉 Android 系统，Connect 应用可以处理应用程序注册中所配置的重定向 URL 的请求。若要执行此操作，请打开 **strings.xml** 字符串资源文件并将以下子项添加到项目 **\<application/\>** 元素中。</span><span class="sxs-lookup"><span data-stu-id="60856-p123">You need to tell the Android system that Connect app can handle requests to the redirect URL configured in the application registration. To do this, open the **strings.xml** string resource file and add the following children to the projects  **\<application/\>** element.</span></span>

   ```xml
   <!DOCTYPE resources [
       <!ENTITY clientId "ENTER_YOUR_CLIENT_ID">
       ]>

    ...
    <string name="client_Id">&clientId;</string>
    <string name="msalPrefix">msal&clientId;</string>
   ```

   <br/>

   <span data-ttu-id="60856-187">将在 **AndroidManifest.xml** 文件中使用字符串资源。</span><span class="sxs-lookup"><span data-stu-id="60856-187">The string resources are used in the **AndroidManifest.xml** file.</span></span> <span data-ttu-id="60856-188">**MSAL** 库在运行时读取客户端 ID，并返回为 **BrowserTabActivity** 定义的重定向 URL 的 REST 响应。</span><span class="sxs-lookup"><span data-stu-id="60856-188">The **MSAL** library reads the client ID at runtime and returns REST responses to the redirect URL defined for the **BrowserTabActivity**.</span></span>

    ```xml
        <uses-sdk tools:overrideLibrary="com.microsoft.identity.msal" />
        <application ...>
            ...
           <activity
               android:name="com.microsoft.identity.client.BrowserTabActivity">
               <intent-filter>
                   <action android:name="android.intent.action.VIEW" />
                   <category android:name="android.intent.category.DEFAULT" />
                   <category android:name="android.intent.category.BROWSABLE" />
                   <data android:scheme="@string/msalPrefix"
                       android:host="auth" />
               </intent-filter>
           </activity>
           <meta-data
               android:name="https://login.microsoftonline.com/common"
               android:value="authority string"/>
           <meta-data
               android:name="com.microsoft.identity.client.ClientId"
               android:value="@string/client_Id"/>
        </application>
    ```


2. <span data-ttu-id="60856-p125">**MSAL** 库需要访问由注册门户分配的应用程序 ID。**MSAL 库将应用程序 ID 称为“客户端 ID”**。从传入库构造函数的应用程序上下文获取应用程序 ID（客户端 ID）。</span><span class="sxs-lookup"><span data-stu-id="60856-p125">The **MSAL** library needs access to the application Id assigned by the registration portal. **The MSAL library refers to the application Id as the "Client Id"**. It gets the application Id (Client Id) from the application context that you pass in the library constructor.</span></span> 

   > <span data-ttu-id="60856-192">**注意：** 还可以将字符串参数传递给构造函数，从而在运行时提供客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="60856-192">**Note:** You can also provide the client Id at run-time by passing a string parameter to the constructor.</span></span> 

3. <span data-ttu-id="60856-p126">授权服务器发送响应时，将调用活动。使用授权服务器的响应请求一个访问令牌。转到 **AuthenticationManager** 并在类中查找以下代码。</span><span class="sxs-lookup"><span data-stu-id="60856-p126">The activity is invoked when the authorization server sends a response. Request an access token with the response from the authorization server. Go to your **AuthenticationManager** and find the following code in the class.</span></span>

   ```java
    /**
     * Authenticates the user and lets the user authorize the app for the requested permissions.
     * An authentication token is returned via the getAuthInteractiveCalback method
     * @param activity
     * @param authenticationCallback
     */
    public void connect(Activity activity, final MSALAuthenticationCallback authenticationCallback){
        mActivityCallback = authenticationCallback;
        mPublicClientApplication.acquireToken(
                activity, Constants.SCOPES, getAuthInteractiveCallback());
    }


     /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

     /**
     * Returns the access token obtained in authentication
     *
     * @return mAccessToken
     */
    public String getAccessToken() throws AuthenticatorException, IOException, OperationCanceledException {
        return  mAuthResult.getAccessToken();
    }

   ```

<br/>

## <a name="call-microsoft-graph"></a><span data-ttu-id="60856-196">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="60856-196">Call Microsoft Graph</span></span>

<span data-ttu-id="60856-197">可以 [使用 Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) 或 [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) 调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="60856-197">You can [use the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) or the [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) to call Microsoft Graph.</span></span>

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a><span data-ttu-id="60856-198">使用 Microsoft Graph SDK 调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="60856-198">Call Microsoft Graph using the Microsoft Graph SDK</span></span>

<span data-ttu-id="60856-p127">[适用于 Android 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-android) 提供可从 Microsoft Graph 生成请求和处理结果的类。请按照以下步骤使用 Microsoft Graph SDK。</span><span class="sxs-lookup"><span data-stu-id="60856-p127">The [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) provides classes that build requests and process results from Microsoft Graph. Follow these steps to use the Microsoft Graph SDK.</span></span>

1. <span data-ttu-id="60856-p128">将 Internet 权限添加到应用打开 **AndroidManifest** 文件并将以下子级添加到清单元素。</span><span class="sxs-lookup"><span data-stu-id="60856-p128">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
    ```


2. <span data-ttu-id="60856-203">将依赖项添加到 Microsoft Graph SDK 和 GSON。</span><span class="sxs-lookup"><span data-stu-id="60856-203">Add dependencies to the Microsoft Graph SDK and GSON.</span></span>
   
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. <span data-ttu-id="60856-204">使用 **AuthenticateRequest** 帮助程序方法，将身份验证令牌添加到新请求中。</span><span class="sxs-lookup"><span data-stu-id="60856-204">Add authentication token to new requests by using the **AuthenticateRequest** helper method.</span></span> <span data-ttu-id="60856-205">此方法通过 Microsoft Graph 身份验证 **IAuthenticationProvider** 接口，实现相同的方法。</span><span class="sxs-lookup"><span data-stu-id="60856-205">This method implements the same method from the Microsoft Graph Authentication **IAuthenticationProvider** interface.</span></span>
    
   ```java
    /**
     * Appends an access token obtained from the {@link AuthenticationManager} class to the
     * Authorization header of the request.
     * @param request
     */
    @Override
    public void authenticateRequest(IHttpRequest request)  {
        try {
            request.addHeader("Authorization", "Bearer "
                    + AuthenticationManager.getInstance()
                    .getAccessToken());
            // This header has been added to identify this sample in the Microsoft Graph service.
            // If you're using this code for your project please remove the following line.
            request.addHeader("SampleID", "android-java-connect-sample");
        } catch (AuthenticatorException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        }  catch (OperationCanceledException e) {
            e.printStackTrace();
        } catch (NullPointerException e) {
            e.printStackTrace();
        }
    }
   ```


4. <span data-ttu-id="60856-206">使用以下帮助程序方法，通过 **GraphServiceController** 帮助程序类，创建并发送草稿电子邮件。</span><span class="sxs-lookup"><span data-stu-id="60856-206">Create a draft email and send it by using the following helper methods from the **GraphServiceController** helper class.</span></span>

   ```java
    /**
     * Creates a draft email message using the Microsoft Graph API on Office 365. The mail is sent
     * from the address of the signed in user.
     *
     * @param senderPreferredName The mail senders principal user name (email addr)
     * @param emailAddress        The recipient email address.
     * @param subject             The subject to use in the mail message.
     * @param body                The body of the message.
     * @param callback            The callback method to invoke on completion of the POST request
     */
    public void createDraftMail(
            final String senderPreferredName,
            final String emailAddress,
            final String subject,
            final String body,
            ICallback<Message> callback
    ) {
        try {
            // create the email message
            Message message = createMessage(subject, body, emailAddress);
            mGraphServiceClient
                    .getMe()
                    .getMessages()
                    .buildRequest()
                    .post(message, callback);

        } catch (Exception ex) {
            showException(ex, "exception on send mail","Send mail failed", "The send mail method failed");
        }
    }

        /**
     * Creates a new Message object 
     */
    Message createMessage(
            String subject,
            String body,
            String address) {

        if (address == null || address.isEmpty()) {
            throw new IllegalArgumentException("The address parameter can't be null or empty.");
        } else {
            // perform a simple validation of the email address
            String addressParts[] = address.split("@");
            if (addressParts.length != 2 || addressParts[0].length() == 0 || addressParts[1].indexOf('.') == -1) {
                throw new IllegalArgumentException(
                        String.format("The address parameter must be a valid email address {0}", address)
                );
            }
        }
        Message message = new Message();
        EmailAddress emailAddress = new EmailAddress();
        emailAddress.address = address;
        Recipient recipient = new Recipient();
        recipient.emailAddress = emailAddress;
        message.toRecipients = Collections.singletonList(recipient);
        ItemBody itemBody = new ItemBody();
        itemBody.content = body;
        itemBody.contentType = BodyType.html;
        message.body = itemBody;
        message.subject = subject;
        return message;
    }
    /**
     * Sends a draft message to the specified recipients
     *
     * @param messageId String. The id of the message to send
     * @param callback
     */
    public void sendDraftMessage(String messageId,
                                 ICallback<Void> callback) {
        try {

            mGraphServiceClient
                    .getMe()
                    .getMessages(messageId)
                    .getSend()
                    .buildRequest()
                    .post(callback);

        } catch (Exception ex) {
            showException(ex, "exception on send draft message ","Send draft mail failed", "The send draft mail method failed");
        }
    }

   ```
  

### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a><span data-ttu-id="60856-207">使用 Microsoft Graph REST API 调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="60856-207">Call Microsoft Graph using the Microsoft Graph REST API</span></span>

<span data-ttu-id="60856-p130">[Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) 通过一个 REST API 终结点从 Microsoft 云服务公开了多个 API。按照下列步骤使用 REST API。</span><span class="sxs-lookup"><span data-stu-id="60856-p130">The [Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) exposes multiple APIs from Microsoft cloud services through a single REST API endpoint. Follow these steps to use the REST API.</span></span>

1. <span data-ttu-id="60856-p131">将 Internet 权限添加到应用打开 **AndroidManifest** 文件并将以下子级添加到清单元素。</span><span class="sxs-lookup"><span data-stu-id="60856-p131">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```


2. <span data-ttu-id="60856-212">将依赖项添加到 Volley HTTP 库。</span><span class="sxs-lookup"><span data-stu-id="60856-212">Add a dependency to the Volley HTTP library.</span></span>

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   

3. <span data-ttu-id="60856-p132">用以下代码替换行`String accessToken = tokenResponse.accessToken;`。将电子邮件地址插入标记为 **\<YOUR_EMAIL_ADDRESS\>** 的占位符中。</span><span class="sxs-lookup"><span data-stu-id="60856-p132">Replace the line `String accessToken = tokenResponse.accessToken;` with the following code. Insert your email address in the placeholder marked with **\<YOUR_EMAIL_ADDRESS\>**.</span></span>
   
   ```java
    final String accessToken = tokenResponse.accessToken;

    final RequestQueue queue = Volley.newRequestQueue(getApplicationContext());
    String url ="https://graph.microsoft.com/v1.0/me/sendMail";
    final String body = "{" +
        "  Message: {" +
        "    subject: 'Sent using the Microsoft Graph REST API'," +
        "    body: {" +
        "      contentType: 'text'," +
        "      content: 'This is the email body'" +
        "    }," +
        "    toRecipients: [" +
        "      {" +
        "        emailAddress: {" +
        "          address: '<YOUR_EMAIL_ADDRESS>'" +
        "        }" +
        "      }" +
        "    ]}" +
        "}";

    final StringRequest stringRequest = new StringRequest(Request.Method.POST, url,
        new Response.Listener<String>() {
            @Override
            public void onResponse(String response) {
                Log.d("Response", response);
            }
        },
        new Response.ErrorListener() {
            @Override
            public void onErrorResponse(VolleyError error) {
                Log.d("ERROR","error => " + error.getMessage());
            }
        }
    ) {
        @Override
        public Map<String, String> getHeaders() throws AuthFailureError {
            Map<String,String> params = new HashMap<>();
            params.put("Authorization", "Bearer " + accessToken);
            params.put("Content-Length", String.valueOf(body.getBytes().length));
            return params;
        }
        @Override
        public String getBodyContentType() {
            return "application/json";
        }
        @Override
        public byte[] getBody() throws AuthFailureError {
            return body.getBytes();
        }
    };

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            queue.add(stringRequest);
        }
    });
   ```


## <a name="run-the-app"></a><span data-ttu-id="60856-215">运行应用</span><span class="sxs-lookup"><span data-stu-id="60856-215">Run the app</span></span>
<span data-ttu-id="60856-216">可以尝试运行 Android 应用。</span><span class="sxs-lookup"><span data-stu-id="60856-216">You're ready to try your Android app.</span></span>

1. <span data-ttu-id="60856-217">启动 Android 模拟器，或将物理设备连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="60856-217">Start your Android emulator or connect your physical device to your computer.</span></span>
2. <span data-ttu-id="60856-218">在 Android Studio 中，按 Shift+F10 运行应用。</span><span class="sxs-lookup"><span data-stu-id="60856-218">In Android Studio, press Shift+F10 to run your app.</span></span>
3. <span data-ttu-id="60856-219">从部署对话框中选择 Android 模拟器或设备。</span><span class="sxs-lookup"><span data-stu-id="60856-219">Choose your Android emulator or device from the deployment dialog box.</span></span>
4. <span data-ttu-id="60856-220">点击主要活动的“浮动操作”**** 按钮。</span><span class="sxs-lookup"><span data-stu-id="60856-220">Tap the **Floating Action** button on the main activity.</span></span>
5. <span data-ttu-id="60856-221">使用个人帐户/工作或学校帐户登录，并授予请求的权限。</span><span class="sxs-lookup"><span data-stu-id="60856-221">Sign in with your personal or work or school account and grant the requested permissions.</span></span>
6. <span data-ttu-id="60856-222">在“应用选择”对话框中，点击应用即可继续。</span><span class="sxs-lookup"><span data-stu-id="60856-222">In the app selection dialog, tap your app to continue.</span></span>

<span data-ttu-id="60856-223">检查在[调用 Microsoft Graph](#call-microsoft-graph) 中配置的电子邮件地址的收件箱。</span><span class="sxs-lookup"><span data-stu-id="60856-223">Check the Inbox of the email address that you configured in [Call Microsoft Graph](#call-microsoft-graph).</span></span> <span data-ttu-id="60856-224">应该会收到从应用登录帐户发送的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="60856-224">You should have an email from the account that you used to sign in to the app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="60856-225">后续步骤</span><span class="sxs-lookup"><span data-stu-id="60856-225">Next steps</span></span>

- <span data-ttu-id="60856-226">试用 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="60856-226">Try out the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="60856-227">在 [Android 代码段示例](https://github.com/microsoftgraph/android-java-snippets-sample)中，查找常见操作示例，或浏览 GitHub 上的其他 [Android 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android)。</span><span class="sxs-lookup"><span data-stu-id="60856-227">Find examples of common operations in the [Snippets Sample for Android](https://github.com/microsoftgraph/android-java-snippets-sample), or explore our other [Android samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="60856-228">另请参阅</span><span class="sxs-lookup"><span data-stu-id="60856-228">See also</span></span>

- [<span data-ttu-id="60856-229">适用于 Android 的 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="60856-229">Microsoft Graph SDK for Android</span></span>](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [<span data-ttu-id="60856-230">获取访问令牌以调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="60856-230">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="60856-231">代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="60856-231">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="60856-232">不代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="60856-232">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
