# <a name="get-started-with-microsoft-graph-in-an-android-app"></a>在 Android 应用中开始使用 Microsoft Graph

> **为企业客户生成应用？**如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。在这种情况下，你可能不知道，而且客户可能会遇到错误。 

> 若要在**所有企业方案**中支持**所有企业客户**，必须使用 Azure AD 终结点并使用 [Azure 管理门户](https://aka.ms/aadapplist)管理应用。有关详细信息，请参阅 [在 Azure AD 和 Azure AD v2.0 终结点之间进行选择](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。

本文介绍了从 Azure AD v2.0 终结点获取访问令牌和调用 Microsoft Graph 所需的任务。介绍了生成 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)的步骤，并说明实现在面向 Android 的应用中使用 Microsoft Graph 的主要概念。本文还介绍如何通过使用[用于 Android 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-android) 或原始 REST 调用来访问 Microsoft Graph。

若要在面向 Android 的应用中使用 Microsoft Graph，则需要向用户显示 Microsoft 登录页，如以下屏幕截图中所示。

![Android 上的 Microsoft 帐户登录页](images/AndroidConnect.png)

**不想生成一个应用吗？**通过下载本文所基于的 [Android 连接示例](https://github.com/microsoftgraph/android-java-connect-sample)快速准备就绪并开始运行。


## <a name="prerequisites"></a>先决条件

若要开始，将需要以下各项： 

- 一个 [Microsoft 帐户](https://www.outlook.com/)或者一个[工作或学校帐户](http://dev.office.com/devprogram)
- Android Studio 2.0 或更高版本


## <a name="register-the-application"></a>注册应用程序
在 Microsoft 应用注册门户上注册一个应用。这会生成用于配置此应用的应用程序 ID 和密码。

1. 使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。

2. 选择“**添加应用**”。

3. 输入应用的名称，并选择“**创建应用程序**”。 
    
    将显示注册页，其中列出应用的属性。

4. 复制应用程序 ID。这是应用的唯一标识符。 

5. 选择“**添加平台**”和“**移动应用程序**”。

    > **注意：**应用程序注册门户提供值为 *urn: ietf:wg:oauth:2.0:oob* 的重定向 URI。但是，你将使用默认的重定向 URI 值 *https://login.microsoftonline.com/common/oauth2/nativeclient*。

6. 选择“**保存**”。


## <a name="configure-the-project"></a>配置项目

在 Android Studio 中开始一个新项目。可以保留大多数向导的默认值，只需确保选择下列选项：

* 目标 Android 设备 - **电话和平板电脑**
    * 最小 SDK - **API 16：Android 4.1 (Jelly Bean)**
* 将活动添加到移动电话 - **基本活动**
 
这为你提供一个带有活动和按钮的 Android 项目，可以用来对用户进行身份验证。

> 注意：还可以使用 [初学者项目](https://github.com/microsoftgraph/android-java-connect-sample/tree/master/starter-project) 进行项目配置，这样就可以专注于此次演练的编码部分。

## <a name="authenticate-the-user-and-get-an-access-token"></a>对用户进行身份验证并获取一个访问令牌
可以使用 OAuth 库来简化身份验证流程。[OpenID](http://openid.net) 提供了 [适用于 Android 的 AppAuth](https://github.com/openid/AppAuth-Android)，它是可以在此项目中使用的一个库。

### <a name="add-the-dependency-to-appbuildgradle"></a>向 app/build.gradle 添加依赖项

在应用模块中打开 `build.gradle` 文件，并包括以下依赖项：

```gradle
compile 'net.openid:appauth:0.3.0'
```

### <a name="start-the-authentication-flow"></a>开始身份验证流

1. 在 **onCreate** 方法中打开 **MainActivity** 文件并声明一个 **AuthorizationService** 对象。
    ```java
    final AuthorizationService authorizationService =
        new AuthorizationService(this);
    ```
    
2. 找到 *FloatingActionButton* 单击事件的事件处理程序。用以下代码替换 **onClick** 方法。将应用中的**应用程序 ID** 插入到标记为 **\<YOUR_APPLICATION_ID\>** 的占位符中。
    ```java
    @Override
    public void onClick(View view) {
        Uri authorizationEndpoint =
            Uri.parse("https://login.microsoftonline.com/common/oauth2/v2.0/authorize");
        Uri tokenEndpoint =
            Uri.parse("https://login.microsoftonline.com/common/oauth2/v2.0/token");
        AuthorizationServiceConfiguration config =
            new AuthorizationServiceConfiguration(
                    authorizationEndpoint,
                    tokenEndpoint,null);

        List<String> scopes = new ArrayList<>(
            Arrays.asList("openid mail.send".split(" ")));

        AuthorizationRequest authorizationRequest = new AuthorizationRequest.Builder(
            config,
            "<YOUR_APPLICATION_ID>",
            ResponseTypeValues.CODE,
            Uri.parse("https://login.microsoftonline.com/common/oauth2/nativeclient"))
            .setScopes(scopes)
            .build();

        Intent intent = new Intent(view.getContext(), MainActivity.class);

        PendingIntent redirectIntent =
            PendingIntent.getActivity(
                    view.getContext(),
                    authorizationRequest.hashCode(),
                    intent, 0);

        authorizationService.performAuthorizationRequest(
            authorizationRequest,
            redirectIntent);
    }
    ```
    
此时，应具有带按钮的 Android 应用。如果按下该按钮，应用会使用设备浏览器显示身份验证页。下一步是处理授权服务器发送到重定向 URI 的代码，并用它来交换访问令牌。

### <a name="exchange-the-authorization-code-for-an-access-token"></a>用授权代码交换访问令牌

需要让应用准备就绪，以处理授权服务器的响应，其中包含用于交换访问令牌的代码。

1. 需要告诉 Android 系统，**MainActivity** 可以处理对 *https://login.microsoftonline.com/common/oauth2/nativeclient* 的请求。若要执行此操作，请打开 **AndroidManifest** 文件并将以下子集添加到 MainActivity 的 **intent-filter** 元素中。
    ```xml
    <action android:name="android.intent.action.VIEW"/>
    <category android:name="android.intent.category.DEFAULT"/>
    <category android:name="android.intent.category.BROWSABLE"/>
    <data android:scheme="https"/>
    <data android:host="login.microsoftonline.com"/>
    <data android:path="/common/oauth2/nativeclient"/>
    ```

2. 授权服务器发送响应时，将调用活动。可以使用授权服务器的相应请求一个访问令牌。返回 **MainActivity**，并将以下代码追加到 **onCreate** 方法中。
    ```java
    Bundle extras = getIntent().getExtras();
    if (extras != null) {
        AuthorizationResponse authorizationResponse = AuthorizationResponse.fromIntent(getIntent());
        AuthorizationException authorizationException = AuthorizationException.fromIntent(getIntent());
        final AuthState authState = new AuthState(authorizationResponse, authorizationException);

        if (authorizationResponse != null) {
            HashMap<String, String> additionalParams = new HashMap<>();
            TokenRequest tokenRequest = authorizationResponse.createTokenExchangeRequest(additionalParams);

            authorizationService.performTokenRequest(
                tokenRequest,
                new AuthorizationService.TokenResponseCallback() {
                    @Override
                    public void onTokenRequestCompleted(
                            @Nullable TokenResponse tokenResponse,
                            @Nullable AuthorizationException ex) {
                        authState.update(tokenResponse, ex);
                        if (tokenResponse != null) {
                            String accessToken = tokenResponse.accessToken;
                        }
                    }
                });
        } else {
            Log.i("MainActivity", "Authorization failed: " + authorizationException);
        }
    }
    ```

请注意，在行 `String accessToken = tokenResponse.accessToken;` 中有一个访问令牌。现在可以添加代码调用 Microsoft Graph。 

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph
可以 [使用 Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) 或 [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) 调用 Microsoft Graph。

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a>使用 Microsoft Graph SDK 调用 Microsoft Graph
[适用于 Android 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-android) 提供可从 Microsoft Graph 生成请求和处理结果的类。请按照以下步骤使用 Microsoft Graph SDK。

1. 将 Internet 权限添加到应用打开 **AndroidManifest** 文件并将以下子级添加到清单元素。
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. 将依赖项添加到 Microsoft Graph SDK 和 GSON。
    ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.0.0'
    compile 'com.google.code.gson:gson:2.7'
    ```
   
3. 用以下代码替换行`String accessToken = tokenResponse.accessToken;`。将电子邮件地址插入标记为 **\<YOUR_EMAIL_ADDRESS\>** 的占位符中。
    ```java
    final String accessToken = tokenResponse.accessToken;
    final IClientConfig clientConfig = 
            DefaultClientConfig.createWithAuthenticationProvider(new IAuthenticationProvider() {
        @Override
        public void authenticateRequest(IHttpRequest request) {
            request.addHeader("Authorization", "Bearer " + accessToken);
        }
    });

    final IGraphServiceClient graphServiceClient = new GraphServiceClient
        .Builder()
        .fromConfig(clientConfig)
        .buildClient();

    final Message message = new Message();
    EmailAddress emailAddress = new EmailAddress();
    emailAddress.address = "<YOUR_EMAIL_ADDRESS>";
    Recipient recipient = new Recipient();
    recipient.emailAddress = emailAddress;
    message.toRecipients = Collections.singletonList(recipient);
    ItemBody itemBody = new ItemBody();
    itemBody.content = "This is the email body";
    itemBody.contentType = BodyType.text;
    message.body = itemBody;
    message.subject = "Sent using the Microsoft Graph SDK";

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            graphServiceClient
                .getMe()
                .getSendMail(message, false)
                .buildRequest()
                .post();
        }
    });
    ```

### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a>使用 Microsoft Graph REST API 调用 Microsoft Graph
[Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) 通过一个 REST API 终结点从 Microsoft 云服务公开了多个 API。按照下列步骤使用 REST API。

1. 将 Internet 权限添加到应用打开 **AndroidManifest** 文件并将以下子级添加到清单元素。
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. 将依赖项添加到 Volley HTTP 库。

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. 用以下代码替换行`String accessToken = tokenResponse.accessToken;`。将电子邮件地址插入标记为 **\<YOUR_EMAIL_ADDRESS\>** 的占位符中。
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

## <a name="run-the-app"></a>运行应用
可以尝试运行 Android 应用。

1. 启动 Android 仿真程序或将物理设备连接至计算机。
2. 在 Android Studio 中，按 Shift + F10 运行应用。
3. 从部署对话框中选择 Android 仿真程序或设备。
4. 点击主要活动上的浮动操作按钮。
5. 使用你的个人、工作或学校帐户登录，并授予所请求的权限。
6. 在“应用选择”对话框中，点击应用以继续。

请检查在 [调用 Microsoft Graph](#call-microsoft-graph) 中配置的电子邮件地址的收件箱。你应该会收到一封用于登录该应用的帐户所发送的电子邮件。

## <a name="next-steps"></a>后续步骤
- 试用 [Microsoft Graph 资源管理器](https://graph.microsoft.io/graph-explorer)。
- 在 [Android 的代码段示例](https://github.com/microsoftgraph/android-java-snippets-sample)中查找常见操作的示例，或浏览 GitHub 上的其他 [Android 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android)。


## <a name="see-also"></a>另请参阅
* [适用于 Android 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-android) 
* [Azure AD v2.0 协议](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
* [Azure AD v2.0 令牌](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
