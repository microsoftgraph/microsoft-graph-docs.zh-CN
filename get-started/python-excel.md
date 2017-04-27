# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a>使用 Microsoft Graph 在 Python 应用中访问 Excel

可以使用 Microsoft Graph API 读取和更新存储在受支持的在线存储平台（包括 OneDrive 和 SharePoint）中的工作簿。`Workbook`（或 Excel 文件）资源包含所有其他 Excel 资源，应用可以通过简单的导航来访问它们。 

可以通过使用标准 REST API 访问一组 Excel 对象（例如表、区域或图表），以便对工作簿执行创建、读取、更新和删除 (CRUD) 操作。例如，`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
返回属于工作簿的工作表对象的集合。    

本演练介绍如何从 Python Web 应用将请求发送到 Excel REST API。 

##  <a name="prerequisites"></a>先决条件

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* [工作或学校帐户](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. -->


## <a name="authorization-and-scopes"></a>授权和范围
可以使用 [Azure AD v2.0 终结点](https://graph.microsoft.io/en-us/docs/authorization/converged_auth) 对 Excel REST API 调用进行身份验证。所有 API 都要求提供 `Authorization: Bearer {access-token}` HTTP 标头。   
  
要使用 Excel 资源，需要以下 [权限范围](https://graph.microsoft.io/en-us/docs/authorization/permission_scopes) 之一：

* Files.Read 
* Files.ReadWrite

## <a name="sessions-and-persistence"></a>会话和永久性

可以在以下任一模式下调用 Excel API： 

1. 永久会话 - 保持（保存）对工作簿所做的全部更改。这是常用的操作模式。 
2. 非永久会话 - 不会将 API 所做的更改保存到源位置。相反，Excel 后端服务器保留文件的临时副本，体现在特定 API 会话期间所做的更改。Excel 会话过期时，这些更改将丢失。此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。   

若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。 

## <a name="register-the-application-in-azure-active-directory"></a>在 Azure Active Directory 中注册应用程序

首先，需要注册应用程序并设置 Microsoft Graph 的使用权限。此操作允许用户使用工作或学校帐户登录应用程序。

### <a name="register-the-application"></a>注册应用程序

在 Microsoft 应用注册门户上注册一个应用。这会生成用于配置此应用的应用程序 ID 和密码，并进行身份验证。

1. 使用个人或工作或学校帐户登录到 [Microsoft 应用注册门户](https://apps.dev.microsoft.com/)。

2. 选择“添加应用”****。

3. 输入应用的名称，并选择“**创建应用程序**”。

    将显示注册页，其中列出应用的属性。

4. 复制应用程序 ID。这是应用的唯一标识符。

5. 在“应用程序机密”****下，选择“生成新密码”****。从“生成的新密码”****对话框复制应用机密。

    将使用此应用程序 ID 和应用机密配置应用。

6. 在“平台”****下，选择“添加平台”**** > “Web”****。

7. 请确保已选中“允许隐式流”****复选框，并输入应用的重定向 URI。

    “允许隐式流”****选项可启用 OpenID Connect 混合流。在身份验证过程中，这可使应用同时接收登录信息 (**id_token**) 以及应用用来获取访问令牌的项目（在这种情况下，项目为授权代码）。

8. 选择“保存”****。

### <a name="create-oauth-client"></a>创建 OAuth 客户端

应用需要注册 Flask-OAuth 客户端实例，用于启动 OAuth 流并获取访问令牌。请注意，需要 *Files.ReadWrite* 范围才能获取支持永久更改的 Excel 会话。

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

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a>在回复 URL 页面中接收授权代码

用户登录后，浏览器将重定向到回复 URL。成功授权后，将在响应正文中返回访问令牌（用于授权其他请求）。 

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

## <a name="make-requests-to-the-excel-api"></a>对 Excel API 发出请求

### <a name="request-headers"></a>请求标头 
使用访问令牌，您的应用可以对 Microsoft Graph API 提出身份验证请求。您的应用必须将访问令牌附加到各个请求的**授权**头中。

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
         'Accept' : 'application/json',
         'Content-Type' : 'application/json'
    }
```
> **注意** 该请求还必须发送包含 Graph API 接受的值的 **Content-Type** 标头，例如 `application/json`。

### <a name="getting-an-excel-session"></a>获取 Excel 会话
#### <a name="request"></a>请求 

通过将 `persistChanges` 值设置为 `true` 或 `false` 可传递一个 JSON 对象。当 `persistChanges` 值设置为 `false` 时，则返回非永久会话 id。此示例使用[请求](http://docs.python-requests.org/en/latest/user/quickstart) HTTP 库 

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

#### <a name="response"></a>响应

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201, Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a>用法 

将前一个调用中返回的会话 ID 传递为 **Workbook-Session-Id** HTTP 标头中后续 API 请求上的标头。例如，列出该 Excel 工作簿中的工作表。

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

#### <a name="response"></a>响应

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200, OK
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

## <a name="next-steps"></a>后续步骤

通过 **Workbook-Session-Id** HTTP 标头，可以开始发出请求以获取数据、创建图表以及更多操作。 

* [常见的 Excel API 方案](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [在 Microsoft Graph 中使用 Excel](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

Microsoft Graph 中的 Excel REST API 提供了访问 Excel 工作簿中的数据并与其进行交互的有效方式。探究使用 Microsoft Graph 还能执行哪些操作。

* [Microsoft Graph 概述](https://developer.microsoft.com/graph/docs)
* [在 Python 应用中开始使用 Microsoft Graph](https://developer.microsoft.com/graph/docs/get-started/python)
