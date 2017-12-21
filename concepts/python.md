# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>在 Python 应用中开始使用 Microsoft Graph 

本文介绍了从 Azure AD 获取访问令牌和调用 Microsoft Graph 所需的任务。 本文逐步演示了如何[使用 Python 通过 Microsoft Graph 发送邮件](https://github.com/microsoftgraph/python-sample-send-mail)，并说明了使用 Microsoft Graph API 要实现的主要概念。 本文介绍了如何使用 REST 直接调用来访问 Microsoft Graph。

![发送邮件表单](https://raw.githubusercontent.com/microsoftgraph/python-sample-send-mail/master/static/images/sendmail.png)

## <a name="choosing-an-authentication-library"></a>选择身份验证库

若要调用 Microsoft Graph，应用必须包含从 Microsoft 云标识服务 Azure Active Directory (Azure AD) 获取的有效访问令牌，且每次调用 Microsoft Graph REST API 时，必须在 HTTP 头中传递令牌。 Graph 采用的身份验证方法以 OAuth 2.0 和 Open ID Connect 标准为依据。因此，为了在应用中实现身份验证，有许多[身份验证库](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-v2-libraries)可供选择。

下述示例使用 [Flask-OAuthlib](https://flask-oauthlib.readthedocs.io/en/latest/) 库来实现 OAuth 2.0 [授权代码授权](https://tools.ietf.org/html/rfc6749#section-4.1)工作流，这是适合使用 Python 编写的 Web 应用的推荐身份验证工作流。 若要了解其他身份验证选项，请参阅 [Microsoft Graph 的 Python 身份验证示例](https://github.com/microsoftgraph/python-sample-auth)。

## <a name="installing-and-running-the-send-mail-sample"></a>安装和运行“发送邮件”示例

若要安装和配置示例应用，请按照[安装 Python REST 示例](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md)中的说明操作。 对于下述“发送邮件”示例，使用以下命令克隆存储库：

    ```git clone https://github.com/microsoftgraph/python-sample-send-mail.git```

按照[安装说明](https://github.com/microsoftgraph/python-sample-auth/blob/master/installation.md)中所述注册应用时，请务必添加 **User.Read** 和 **Mail.Send** 权限，这些是此示例的必需权限。

完成安装/配置后，可以按照[运行示例](https://github.com/microsoftgraph/python-sample-send-mail#running-the-sample)中的说明操作，运行示例应用。

## <a name="code-walkthrough"></a>代码演练

下面大致介绍了示例应用的[源代码](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py)。

前几行代码是此示例中使用的 Python 模块和包的[导入](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L4-L11)部分：

* 标准库中的 **base64** 模块用于编码电子邮件附件。
* 标准库中的 **pprint** 模块用于优质打印 Graph 返回的任何错误消息。 （例如，如果尝试发送到的电子邮件地址无效。）
* 标准库中的 **uuid** 模块用于生成包含 36 个字符的随机字符串，以唯一标识每个 Graph 请求。 这可用于进行调试。
* **flask** 包是此示例的 Web 框架。
* **flask_oauthlib.client** 的 **OAuth** 类是 Flask 应用的包装器，用于实现 OAuth 2.0 身份验证工作流。
* **config** 模块包含上面安装过程中配置的应用注册设置。

接下来，先[创建 Flask 应用](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L13-L15)，再创建名为 **MSGRAPH** 的 [Graph 客户端对象](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L17-L26)。

完成初始设置步骤后，将处理下列三个实现身份验证工作流的 Flask 路由处理程序函数：[homepage()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L28-L31)、[login()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L33-L37) 和 [authorized()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L39-L46)。 若要详细了解身份验证工作流，请参阅 Python 身份验证示例存储库的[示例体系结构](https://github.com/microsoftgraph/python-sample-auth#sample-architecture)部分。

下一个路由处理程序 [mailform()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L48-L54) 是指定电子邮件收件人、主题和正文的表单。 请注意，此函数也负责首次调用 Graph：[检索用户配置文件](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L51-L51)，以获取当前用户的显示名称和电子邮件地址，这些信息将被[传递到 mailform.html 模板](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L52-L54)。

下一个 [send_mail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L56-L73) 函数发送电子邮件，并显示 Graph API 返回的响应。 它使用 sendmail() 帮助程序函数，同时向它传递从表单公布的查询字符串参数：

```python
response = sendmail(MSGRAPH,
                    subject=flask.request.args['subject'],
                    recipients=flask.request.args['email'].split(';'),
                    html=flask.request.args['body'])
```

只要调用 Graph，Flask-OAuthlib 客户端实例 (```MSGRAPH```) 都是使用 [get_token()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L75-L78) 函数来获取访问令牌。 虽然访问令牌在名为 **Authorization** 的 HTTP 头中传递，但无需在代码中对此进行处理。 只需通过客户端的 HTTP 谓词方法（例如，get() 或 post()）调用 Graph，客户端实例就会知道调用 ```get_token()``` 来获取令牌，因为此函数是使用 ```tokengetter``` 进行[修饰](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L75-L75)。

下一个 [request_headers()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L80-L85) 函数返回随每次 Graph 调用一起发送的 HTTP 头的字典。

最后一个 [sendmail()](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L87-L129) 是用于发送电子邮件的帮助程序函数。 它使用 Microsoft Graph API 中的 ```me/microsoft.graph.sendMail``` 终结点发送邮件。无论何时需要通过 Microsoft Graph 发送电子邮件，都可以在自己的代码中重用此函数。 若要了解如何调用此函数，请参阅 [docstring](https://github.com/microsoftgraph/python-sample-send-mail/blob/master/sample.py#L88-L97)。

## <a name="other-python-rest-samples"></a>其他 Python REST 示例

除了上述示例外，下面的示例展示了如何通过 Python 使用 Microsoft Graph 的其他功能：

* [Microsoft Graph 的 Python 身份验证示例](https://github.com/microsoftgraph/python-sample-auth)
* [在 Python 中处理分页 Microsoft Graph 响应](https://github.com/microsoftgraph/python-sample-pagination)
* [在 Python 中使用 Graph 开放扩展](https://github.com/microsoftgraph/python-sample-open-extensions)

若要查看某个特定示例，请通过[提交问题](https://github.com/microsoftgraph/python-sample-auth/issues)告诉我们。 我们非常期待收到大家就希望在 Python 中生成的任何 Microsoft Graph 方案提供的反馈。

Microsoft Graph API 的功能非常强大，统一了可用于与各种 Microsoft 数据进行交互的 API。 请查看[开发人员文档](https://developer.microsoft.com/zh-CN/graph/docs/concepts/overview)或 [Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)，了解还可以使用 Microsoft Graph 做什么。
