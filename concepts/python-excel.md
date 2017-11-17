# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a><span data-ttu-id="ca236-101">使用 Microsoft Graph 在 Python 应用中访问 Excel</span><span class="sxs-lookup"><span data-stu-id="ca236-101">Use Microsoft Graph to access Excel in a Python app</span></span>

<span data-ttu-id="ca236-102">可以使用 Microsoft Graph API 读取和更新存储在受支持的在线存储平台（包括 OneDrive 和 SharePoint）中的工作簿。</span><span class="sxs-lookup"><span data-stu-id="ca236-102">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The  (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> <span data-ttu-id="ca236-103">`Workbook`（或 Excel 文件）资源包含所有其他 Excel 资源，应用可以通过简单的导航来访问它们。</span><span class="sxs-lookup"><span data-stu-id="ca236-103">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The `Workbook` (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> 

<span data-ttu-id="ca236-104">可以通过使用标准 REST API 访问一组 Excel 对象（例如表、区域或图表），以便对工作簿执行创建、读取、更新和删除 (CRUD) 操作。</span><span class="sxs-lookup"><span data-stu-id="ca236-104">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, </span></span> <span data-ttu-id="ca236-105">例如，`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span><span class="sxs-lookup"><span data-stu-id="ca236-105">For example:`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="ca236-106">返回属于工作簿的工作表对象的集合。</span><span class="sxs-lookup"><span data-stu-id="ca236-106">returns a collection of worksheet objects that are part of the workbook.</span></span>    

<span data-ttu-id="ca236-107">本演练介绍如何从 Python Web 应用将请求发送到 Excel REST API。</span><span class="sxs-lookup"><span data-stu-id="ca236-107">This walkthrough describes how to make requests to the Excel REST API from a Python web app.</span></span> 

##  <a name="prerequisites"></a><span data-ttu-id="ca236-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca236-108">Prerequisites</span></span>

* [<span data-ttu-id="ca236-109">Python 3.5.2</span><span class="sxs-lookup"><span data-stu-id="ca236-109">Python 3.5.2</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="ca236-110">Flask-OAuthlib</span><span class="sxs-lookup"><span data-stu-id="ca236-110">Flask-OAuthlib</span></span>](https://github.com/lepture/flask-oauthlib)
* <span data-ttu-id="ca236-111">[工作或学校帐户](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span><span class="sxs-lookup"><span data-stu-id="ca236-111">A [work or school account](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span></span>


## <a name="authorization-and-scopes"></a><span data-ttu-id="ca236-112">授权和范围</span><span class="sxs-lookup"><span data-stu-id="ca236-112">Authorization and scopes</span></span>
<span data-ttu-id="ca236-113">可以使用 [Azure AD v2.0 终结点](https://graph.microsoft.io/en-us/docs/concepts/converged_auth)验证 Excel REST API 调用。</span><span class="sxs-lookup"><span data-stu-id="ca236-113">You can use the [Azure AD v2.0 endpoint](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) to authenticate Excel REST API calls. All APIs require the  HTTP header.</span></span> <span data-ttu-id="ca236-114">所有 API 都需要有 `Authorization: Bearer {access-token}` HTTP 头。</span><span class="sxs-lookup"><span data-stu-id="ca236-114">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="ca236-115">要使用 Excel 资源，需要以下 [权限范围](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) 之一：</span><span class="sxs-lookup"><span data-stu-id="ca236-115">One of the following [permission scopes](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="ca236-116">Files.Read</span><span class="sxs-lookup"><span data-stu-id="ca236-116">Files.Read</span></span> 
* <span data-ttu-id="ca236-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca236-117">Files.ReadWrite</span></span>

## <a name="sessions-and-persistence"></a><span data-ttu-id="ca236-118">会话和永久性</span><span class="sxs-lookup"><span data-stu-id="ca236-118">Sessions and persistence</span></span>

<span data-ttu-id="ca236-119">可以在以下任一模式下调用 Excel API：</span><span class="sxs-lookup"><span data-stu-id="ca236-119">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="ca236-p104">永久会话 - 保持（保存）对工作簿所做的全部更改。这是常用的操作模式。</span><span class="sxs-lookup"><span data-stu-id="ca236-p104">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="ca236-p105">非永久会话 - 不会将 API 所做的更改保存到源位置。相反，Excel 后端服务器保留文件的临时副本，体现在特定 API 会话期间所做的更改。Excel 会话过期时，这些更改将丢失。此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。</span><span class="sxs-lookup"><span data-stu-id="ca236-p105">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="ca236-126">若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。</span><span class="sxs-lookup"><span data-stu-id="ca236-126">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

## <a name="register-the-application-in-azure-active-directory"></a><span data-ttu-id="ca236-127">在 Azure Active Directory 中注册应用程序</span><span class="sxs-lookup"><span data-stu-id="ca236-127">Register the application in Azure Active Directory</span></span>

<span data-ttu-id="ca236-p106">首先，需要注册应用程序并设置 Microsoft Graph 的使用权限。此操作允许用户使用工作或学校帐户登录应用程序。</span><span class="sxs-lookup"><span data-stu-id="ca236-p106">First, you need to register your application and set permissions to use Microsoft Graph. This lets users sign in to the application with work or school accounts.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="ca236-130">注册应用程序</span><span class="sxs-lookup"><span data-stu-id="ca236-130">Register the application</span></span>

<span data-ttu-id="ca236-p107">在 Microsoft 应用注册门户上注册一个应用。这会生成用于配置此应用的应用程序 ID 和密码，并进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="ca236-p107">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="ca236-133">使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="ca236-133">Sign in to the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="ca236-134">选择“添加应用”****。</span><span class="sxs-lookup"><span data-stu-id="ca236-134">Choose **Add an app**.</span></span>

3. <span data-ttu-id="ca236-135">输入应用的名称，并选择“**创建应用程序**”。</span><span class="sxs-lookup"><span data-stu-id="ca236-135">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="ca236-136">将显示注册页，其中列出应用的属性。</span><span class="sxs-lookup"><span data-stu-id="ca236-136">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="ca236-p108">复制应用程序 ID。这是应用的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ca236-p108">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="ca236-p109">在“应用程序机密”****下，选择“生成新密码”****。从“生成的新密码”****对话框复制应用机密。</span><span class="sxs-lookup"><span data-stu-id="ca236-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>

    <span data-ttu-id="ca236-141">将使用此应用程序 ID 和应用机密配置应用。</span><span class="sxs-lookup"><span data-stu-id="ca236-141">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="ca236-142">在“平台”****下，选择“添加平台”**** > “Web”****。</span><span class="sxs-lookup"><span data-stu-id="ca236-142">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="ca236-143">请确保已选中“允许隐式流”****复选框，并输入应用的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="ca236-143">Make sure the **Allow Implicit Flow** check box is selected, and enter your app's Redirect URI.</span></span>

    <span data-ttu-id="ca236-144">使用“允许隐式流”****选项，可以启用 OpenID Connect 混合流。</span><span class="sxs-lookup"><span data-stu-id="ca236-144">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow.</span></span> <span data-ttu-id="ca236-145">在身份验证过程中，这可以让应用程序同时接收登录信息 (**id_token**)，以及应用程序用来获取访问令牌的项目（在此示例中为授权代码）。</span><span class="sxs-lookup"><span data-stu-id="ca236-145">During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app can use to obtain an access token.</span></span>

8. <span data-ttu-id="ca236-146">选择“保存”****。</span><span class="sxs-lookup"><span data-stu-id="ca236-146">Choose **Save**.</span></span>

### <a name="create-oauth-client"></a><span data-ttu-id="ca236-147">创建 OAuth 客户端</span><span class="sxs-lookup"><span data-stu-id="ca236-147">Create OAuth client</span></span>

<span data-ttu-id="ca236-148">应用需要注册 Flask-OAuth 客户端实例，用于启动 OAuth 流并获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="ca236-148">Your app needs to register an instance of the Flask-OAuth client that you'll use to start the OAuth flow and get an access token.</span></span> <span data-ttu-id="ca236-149">请注意，需要 *Files.ReadWrite* 范围才能获取支持永久更改的 Excel 会话。</span><span class="sxs-lookup"><span data-stu-id="ca236-149">Note that the *Files.ReadWrite* scope is required to obtain an Excel session that supports persisted changes.</span></span>

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key = client_id,
        consumer_secret = client_secret,
        request_token_params = {'scope': 'User.Read Files.ReadWrite'},
        base_url = 'https://graph.microsoft.com/v1.0/',
        request_token_url = None,
        access_token_method = 'POST',
        access_token_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a><span data-ttu-id="ca236-150">在答复 URL 页中接收授权代码</span><span class="sxs-lookup"><span data-stu-id="ca236-150">Receive an authorization code in your reply URL page</span></span>

<span data-ttu-id="ca236-p112">用户登录后，浏览器将重定向到回复 URL。成功授权后，将在响应正文中返回访问令牌（用于授权其他请求）。</span><span class="sxs-lookup"><span data-stu-id="ca236-p112">After the user signs in, the browser is redirected to your reply URL. Upon successful authorization, the access token (which will be used to authorize additional requests) will be returned in the response body.</span></span> 

```python
    @app.route('/login/authorized')
    def authorized():
        response = microsoft.authorized_response()
        if response is None:
            return "Access Denied: Reason=%s\nError=%s" % (
                request.args['error'], 
                request.args['error_description']
            )
    
        # Check response for state
        if str(session['state']) != str(request.args['state']):
            raise Exception('State has been messed with, end authentication')
        # Remove state session variable to prevent reuse.
        session['state'] = ""
            
        # Okay to store this in a local variable, encrypt if it's going to client
        # machine or database. Treat as a password. 
        session['microsoft_token'] = (response['access_token'], '')
        # Store the token in another session variable for easy access
        session['access_token'] = response['access_token']
```

## <a name="make-requests-to-the-excel-api"></a><span data-ttu-id="ca236-153">对 Excel API 发出请求</span><span class="sxs-lookup"><span data-stu-id="ca236-153">Make requests to the Excel API</span></span>

### <a name="request-headers"></a><span data-ttu-id="ca236-154">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca236-154">Request headers</span></span> 
<span data-ttu-id="ca236-p113">使用访问令牌，您的应用可以对 Microsoft Graph API 提出身份验证请求。您的应用必须将访问令牌附加到各个请求的**授权**头中。</span><span class="sxs-lookup"><span data-stu-id="ca236-p113">With an access token, your app can make authenticated requests to the Microsoft Graph API. Your app must append the access token to the **Authorization** header of each request.</span></span>

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
```
> <span data-ttu-id="ca236-157">**注意** 该请求还必须发送包含 Graph API 接受的值的 **Content-Type** 标头，例如 `application/json`。</span><span class="sxs-lookup"><span data-stu-id="ca236-157">**Note** The request must also send a **Content-Type** header with a value accepted by the Graph API, for example, `application/json`.</span></span>

### <a name="getting-an-excel-session"></a><span data-ttu-id="ca236-158">获取 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="ca236-158">Getting an Excel Session</span></span>
#### <a name="request"></a><span data-ttu-id="ca236-159">请求</span><span class="sxs-lookup"><span data-stu-id="ca236-159">Request</span></span> 

<span data-ttu-id="ca236-160">通过将 `persistChanges` 值设置为 `true` 或 `false` 可传递一个 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ca236-160">Pass a JSON object by setting the `persistChanges` value to `true` or `false`.</span></span> <span data-ttu-id="ca236-161">如果 `persistChanges` 值设置为 `false`，返回非永久会话 ID。</span><span class="sxs-lookup"><span data-stu-id="ca236-161">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span> <span data-ttu-id="ca236-162">此示例使用[请求](http://docs.python-requests.org/en/latest/user/quickstart) HTTP 库</span><span class="sxs-lookup"><span data-stu-id="ca236-162">This example uses the [Requests](http://docs.python-requests.org/en/latest/user/quickstart) HTTP library</span></span> 

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/createSession'
    # Set request headers
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
    # Specify type of session
    body = {
        'persistChanges': True
    }
    
    response = requests.post(url, headers = headers, json = body)
```

#### <a name="response"></a><span data-ttu-id="ca236-163">响应</span><span class="sxs-lookup"><span data-stu-id="ca236-163">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="ca236-164">用法</span><span class="sxs-lookup"><span data-stu-id="ca236-164">Usage</span></span> 

<span data-ttu-id="ca236-165">将前一个调用中返回的会话 ID 传递为 **Workbook-Session-Id** HTTP 标头中后续 API 请求上的标头。</span><span class="sxs-lookup"><span data-stu-id="ca236-165">The session ID returned from the previous call is passed as a header on subsequent API requests in the **Workbook-Session-Id** HTTP header. For instance, to list worksheets in that Excel workbook.</span></span> <span data-ttu-id="ca236-166">例如，列出该 Excel 工作簿中的工作表。</span><span class="sxs-lookup"><span data-stu-id="ca236-166">For instance, to list worksheets in that Excel workbook.</span></span>

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/worksheets'
    # Set request headers - note the session header 
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Workbook-Session-Id': 'cluster=PP1&session=12.a04039942e021.A272...'
    }
    
    response = requests.get(url, headers = headers)
```

#### <a name="response"></a><span data-ttu-id="ca236-167">响应</span><span class="sxs-lookup"><span data-stu-id="ca236-167">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets",
    "value": [
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0000-000000000000}",
        "name": "Session 1",
        "position": 0,
        "visibility": "Visible"
    },
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0100-000000000000}",
        "name": "Session 2",
        "position": 1,
        "visibility": "Visible"
    }]
}
```

## <a name="next-steps"></a><span data-ttu-id="ca236-168">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ca236-168">Next steps</span></span>

<span data-ttu-id="ca236-169">通过 **Workbook-Session-Id** HTTP 标头，可以开始发出请求以获取数据、创建图表以及更多操作。</span><span class="sxs-lookup"><span data-stu-id="ca236-169">With the **Workbook-Session-Id** HTTP header, you can begin issuing requests to fetch data, create charts, and much more.</span></span> 

* [<span data-ttu-id="ca236-170">常见的 Excel API 方案</span><span class="sxs-lookup"><span data-stu-id="ca236-170">Common Excel API scenarios</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [<span data-ttu-id="ca236-171">在 Microsoft Graph 中使用 Excel</span><span class="sxs-lookup"><span data-stu-id="ca236-171">Working with Excel in Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

<span data-ttu-id="ca236-p116">Microsoft Graph 中的 Excel REST API 提供了访问 Excel 工作簿中的数据并与其进行交互的有效方式。探究使用 Microsoft Graph 还能执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="ca236-p116">The Excel REST API in Microsoft Graph provides a powerful way to access and interact with data in Excel workbooks. Explore what else is possible with Microsoft Graph.</span></span>

* [<span data-ttu-id="ca236-174">Microsoft Graph 概述</span><span class="sxs-lookup"><span data-stu-id="ca236-174">Overview of Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs)
* [<span data-ttu-id="ca236-175">在 Python 应用中开始使用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca236-175">Get started with Microsoft Graph in a Python app</span></span>](https://developer.microsoft.com/graph/docs/get-started/python)
