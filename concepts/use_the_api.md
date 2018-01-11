# <a name="use-the-microsoft-graph-api"></a>使用 Microsoft Graph API

Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API. 在[注册应用](auth_register_app_v2.md)并[获取身份验证令牌以用于用户](auth_v2_user.md)或[服务](auth_v2_service.md)后，可以向 Microsoft Graph API 发送请求。

> **重要说明：**条件访问策略应用于 Microsoft Graph 的方式正在发生变化。 应用程序需要进行更新以处理配置了条件访问策略的应用场景。 有关详细信息和指南，请参阅 [Azure Active Directory 条件访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)。

要在资源（如用户或电子邮件）中读取或写入资源，可以创建如下请求：

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

请求的组成部分包括：

* [HTTP 方法](#http-methods) - 在 Microsoft Graph 请求上所使用的 HTTP 方法。
* [`{version}`](#version) - 你的应用程序正在使用的 Microsoft Graph API 版本。
* [`{resource}`](#resource) - 你正在引用的 Microsoft Graph 中的资源。
* [查询参数](#query-parameters-optional) - 一组用于修改请求或响应的可选参数。

发出请求后，返回一个响应，其中包括： 

* 状态代码 - 表示成功或失败的 HTTP 状态代码。 有关 HTTP 错误代码的详细信息，请参阅[错误](errors.md)。
* 响应消息 - 所请求的数据或操作结果。对于某些操作，响应消息可以为空。
* **下一步**链接 - 如果请求返回大量数据，则需要通过选择“下一步”****浏览。 有关详细信息，请参阅[分页](paging.md)。

## <a name="http-methods"></a>HTTP 方法

Microsoft Graph 使用请求上的 HTTP 方法来确定请求正在执行的操作。API 支持以下方法。


|**方法** |**说明**                             |
| :----- | :------------------------------------------- |
| GET    | 从资源中读取数据。                   |
| POST   | 创建新的资源，或执行某个操作。 |
| PATCH  | 用新值更新资源。           |
| PUT    | 替换为新资源。           |
| DELETE | 删除资源。                           |

* 对于 **GET** 和 **DELETE** 方法，不需要任何请求正文。
* **POST**、**PATCH** 和 **PUT** 方法需要通常以 JSON 格式指定的请求正文，此正文包含了其他信息，如资源的属性值。

## <a name="version"></a>版本

Microsoft Graph 目前支持两种版本：`v1.0` 和 `beta`。

* `v1.0` 包括通常可用的 API。 为所有生产应用使用 v1.0 版本。
* `beta` 包括目前处于预览中的 API。 因为我们可能会为试用的 API引入更大更改，我们建议你仅对开发中的测试应用使用试用版；请勿在生产应用中使用试用版 API。

我们一直在寻求有关试用版 API 的反馈。 要提供反馈或开通功能，请参阅 [UserVoice](https://officespdev.uservoice.com/) 页面。

有关 API 版本的详细信息，请参阅[版本控制和支持](versioning_and_support.md)。

## <a name="resource"></a>资源

你的 URL 将包含你正在请求中与之交互的一个或多个资源，如 `me`、`users`、`groups`、`drives` 和 `sites`。 每个顶级资源也包括可以用来访问其他资源的**关系**（如 `me/messages` 或 `me/drive`）。 还可以使用**方法**与资源交互；例如，若要发送电子邮件，可以使用 `me/sendMail`。

若要详细了解如何导航资源关系和方法，请参阅[遍历图](traverse_the_graph.md)。 

每个资源可能需要不同的权限来访问它。通常，你需要用来创建或更新资源的权限比读取时要求的权限更高。有关所需权限的详细信息，请参见方法引用主题。 

有关权限的详细信息，请参阅[权限引用](permissions_reference.md)。

## <a name="query-parameters-optional"></a>查询参数（可选）

你可以使用可选的查询参数，在 Microsoft Graph 应用中自定义响应。使用查询参数来包含比默认响应更多或更少的属性、过滤匹配自定义查询项目的响应，或为方法提供其他参数。

例如，添加以下筛选器参数会将返回的邮件限制为仅 `emailAddress` 属性为 `jon@contoso.com` 的邮件。

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

有关查询参数的详细信息，请参阅[自定义响应](query_parameters.md)。

## <a name="next-steps"></a>后续步骤

你可以随时开始使用和运行 Microsoft Graph。 若要了解详细信息，请转到 [Graph 资源管理器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)尝试发出某些请求、尝试[快速启动](https://developer.microsoft.com/zh-CN/graph/quick-start)，或使用 [SDK 和代码示例](https://developer.microsoft.com/zh-CN/graph/code-samples-and-sdks)之一开始使用。
