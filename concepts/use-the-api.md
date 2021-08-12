---
title: 使用 Microsoft Graph API
description: Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API。在你注册应用并获取身份验证令牌以用于用户或服务后，可以向 Microsoft Graph API 发送请求。
author: jackson-woods
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 6fc4de0eba8feb09668d0b1fd5b059dc6c9f3140a02bf4f99ae31743e1a9d5f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54157872"
---
# <a name="use-the-microsoft-graph-api"></a>使用 Microsoft Graph API

Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API。在你[注册应用](auth-register-app-v2.md)并[获取身份验证令牌以用于用户](auth-v2-user.md)或[服务](auth-v2-service.md)后，可以向 Microsoft Graph API 发送请求。

> **重要说明：** 条件访问策略应用于 Microsoft Graph 的方式在发生变化。 应用程序需要进行更新以处理配置了条件访问策略的应用场景。 有关详细信息和指南，请参阅 [Azure Active Directory 条件访问开发人员指南](/azure/active-directory/develop/active-directory-conditional-access-developer)。

## <a name="odata-namespace"></a>OData 命名空间

Microsoft Graph API 在 [Microsoft Graph 元数据](traverse-the-graph.md#microsoft-graph-api-metadata)的 OData 命名空间 `microsoft.graph` 中，定义它的大多数资源、方法和枚举。 少量的 API 集在其子命名空间中定义，例如[调用记录 API](/graph/api/resources/callrecords-api-overview) 定义诸如 `microsoft.graph.callRecords`中的 [callRecord](/graph/api/resources/callrecords-callrecord) 等资源。 

除非在相应主题中明确指定，否则假定类型、方法和枚举是 `microsoft.graph` 命名空间的一部分。

## <a name="call-a-rest-api-method"></a>调用 REST API 方法

要在资源（如用户或电子邮件）中读取或写入资源，可以创建如下请求：

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

请求的组成部分包括：

* [{HTTP method}](#http-methods) - 在 Microsoft Graph 请求上所使用的 HTTP 方法。
* [{version}](#version) - 你的应用程序正在使用的 Microsoft Graph API 版本。
* [{resource}](#resource) - 你正在引用的 Microsoft Graph 中的资源。 
* [{query-parameters}](#query-parameters) - 可自定义响应的可选 OData 查询选项或 REST 方法参数。

在你发出请求后，响应便会返回，其中包括： 

* 状态代码 - 表示成功或失败的 HTTP 状态代码。若要详细了解 HTTP 错误代码，请参阅[错误](errors.md)。
* 响应消息 - 请求获取的数据或操作结果。对于某些操作，响应消息可能为空。
* `nextLink` - 如果请求返回大量数据，则需要使用 `@odata.nextLink` 中返回的 URL 对其进行翻页。有关详细信息，请参阅[分页](paging.md)。

## <a name="http-methods"></a>HTTP 方法

Microsoft Graph 使用请求上的 HTTP 方法来确定请求正在执行的操作。API 支持以下方法。

|**方法** |**说明**                             |
| :----- | :------------------------------------------- |
| GET    | 从资源中读取数据。                   |
| POST   | 创建新的资源，或执行某个操作。 |
| PATCH  | 用新值更新资源。           |
| PUT    | 替换为新资源。           |
| DELETE | 删除资源。                           |

* 对于 CRUD 方法 `GET` 和 `DELETE`，不需要任何请求正文。
* `POST`、`PATCH` 和 `PUT` 方法需要通常以 JSON 格式指定的请求正文，此正文包含了其他信息，如资源的属性值。

## <a name="version"></a>版本

Microsoft Graph 目前支持以下两种版本：`v1.0` 和 `beta`。

* `v1.0` 包括正式可用 API。请对所有生产应用使用 v1.0 版本。
* `beta` 包括目前处于预览中的 API。因为我们可能会为试用的 API引入更大更改，我们建议你仅对开发中的测试应用使用试用版；请勿在生产应用中使用试用版 API。

我们一直在寻求有关试用版 API 的反馈。若要提供反馈或请求功能，请参阅 [Microsoft 365 开发者平台创意论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)。

若要详细了解 API 版本，请参阅[版本控制和支持](versioning-and-support.md)。

## <a name="resource"></a>Resource

资源可以是实体或复杂类型，通常使用属性定义。 实体与复杂类型的不同之处在于前者始终包含 **id** 属性。

你的 URL 将包含你正在请求中与之交互的资源，如`me`、**用户**、**组**、**驱动器** 和 **网站**。通常，顶级资源还包括可以用来访问其他资源的 _关系_（如 `me/messages` 或 `me/drive`）。你还可以使用 _方法_ 与资源交互；例如，要发送电子邮件，则使用 `me/sendMail`。有关详细信息，请参阅 [通过导航 Microsoft Graph 访问数据和方法](traverse-the-graph.md)。

每个资源可能需要不同的权限来访问它。通常，你需要用来创建或更新资源的权限比读取时要求的权限更高。有关所需权限的详细信息，请参见方法引用主题。 

有关权限的详细信息，请参阅[权限引用](permissions-reference.md)。

## <a name="query-parameters"></a>查询参数

查询参数可以是 OData 系统查询选项，也可以是方法接受的用于自定义其响应的其他字符串。

你可以使用可选的 OData 系统查询选项来包含比默认响应更多或更少的属性、过滤与自定义查询匹配的项的响应，或为方法提供其他参数。

例如，添加以下 `filter` 参数会将返回的邮件限制为 `emailAddress` 属性仅为 `jon@contoso.com` 的邮件。

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

有关 OData 查询选项的详细信息，请参阅[使用查询参数自定义响应](query-parameters.md)。

除 OData 查询选项之外，某些方法还需要将参数值指定为查询 URL 的一部分。 例如，你可以通过查询 **用户** 的 **calendarView** 关系，并将时段 `startDateTime` 和 `endDateTime` 值指定为查询参数来获取用户日历中某个时间段内发生的事件的集合：

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="tools-for-interacting-with-microsoft-graph"></a>用于与 Microsoft Graph 交互的工具

### <a name="graph-explorer"></a>Graph 浏览器

Graph 浏览器是一个基于 Web 的工具，可用于通过 Microsoft Graph API 构建和测试请求。可在以下位置访问 Graph Explorer：[https://developer.microsoft.com/graph/graph-explorer](https://developer.microsoft.com/graph/graph-explorer)。

可在不登录的情况下访问演示数据，或者可登录自己的租户。请按照以下步骤生成请求：

1. 选择 HTTP 方法。
2. 选择要使用的 API 版本。
3. 在请求文本框中键入查询。
4. 选择“**运行查询**”。 

以下示例显示返回演示租户中的用户相关信息的请求：

![Graph 浏览器屏幕截图，突出显示 GET 用户请求](./images/graph-explorer.png)

Graph 浏览器中提供了示例查询，让你能够更快地运行常见请求。 若要查看可用示例，请选择“**显示更多示例**”。 对于要查看的示例集选择“**打开**”，然后在关闭选择窗口后，应会看到预定义的请求列表。

发送请求后将显示状态代码和消息，并在“**响应预览**”选项卡中显示响应。

### <a name="postman"></a>Postman

Postman 浏览器是一款可用于使用 Microsoft Graph API 构建和测试请求的工具。 可在以下位置下载 Postman：[https://www.getpostman.com/](https://www.getpostman.com/)。 若要在 Postman 中与 Microsoft Graph 进行交互，请使用 Microsoft Graph 集合。

有关详细信息，请参阅[结合使用 Postman 和 Microsoft Graph API](./use-postman.md)。

## <a name="next-steps"></a>后续步骤

你可以随时开始使用和运行 Microsoft Graph。请尝试“[快速入门](https://developer.microsoft.com/graph/quick-start)”或开始使用我们的其中一个 [SDK 和代码示例](https://developer.microsoft.com/graph/code-samples-and-sdks)。
