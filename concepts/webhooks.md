---
title: 设置用户数据更改的通知
description: Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。
ms.openlocfilehash: faaa1be8330118f1cbebf5362903f0e114816b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091908"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>设置用户数据更改的通知

Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。

Microsoft Graph 接受订阅请求之后，将通知推送到订阅中指定的 URL。 然后应用根据其业务逻辑执行操作。 例如，它将获取更多数据、更新其缓存和视图等。

## <a name="supported-resources"></a>支持的资源

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

- 邮件
- 事件
- 联系人
- 用户
- 组
- 组对话
- OneDrive 上共享的内容，包括与 SharePoint 网站关联的驱动器。
- 用户的个人 OneDrive 文件夹
- 安全警报

例如，可以创建对特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`

或以下顶级资源的订阅：`me/messages`、`me/contacts`、`me/events`、`users` 或 `groups`

或以下特定资源实例的订阅：`users/{id}`、`groups/{id}`、`groups/{id}/conversations`

或以下 Sharepoint/OneDrive for Business 驱动器的订阅：`/drive/root`

或对用户个人 OneDrive 的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`

或对新[安全性 API 警报](security-concept-overview.md)的订阅：`/security/alerts?$filter=status eq ‘New’`、`/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`

### <a name="azure-ad-resource-limitations"></a>Azure AD 资源限制

基于 Azure AD 的资源（用户、组）采用了某些限制，超出限制时可能会产生错误：

- 最大订阅配额：

  - 每个应用：总订阅数 50,000
  - 每个租户：所有应用的总订阅数 35
  - 每个应用和租户组合：总订阅数 7

- 不支持 Azure AD B2C 租户。

- 个人 Microsoft 帐户不支持用户实体的通知。

## <a name="subscription-lifetime"></a>订阅生命周期

订阅的生命周期有限。 应用需要在订阅到期前续订订阅。 否则，需要新建订阅。 有关最长有效期的列表，请参阅[每个资源类型的最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。

应用还可以随时取消订阅，以停止接收通知。

## <a name="managing-subscriptions"></a>管理订阅

客户端可以创建订阅、续订订阅和删除订阅。

### <a name="creating-a-subscription"></a>创建订阅

创建订阅是开始接收资源通知的第一步。订阅流程如下所示：

1. 客户端发送特定资源的订阅 (POST) 请求。

1. Microsoft Graph 验证请求。

    - 如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。
    - 如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。

1. 客户端将验证令牌发送回 Microsoft Graph。

1. Microsoft Graph 将响应发送回客户端。

客户端必须存储订阅 ID 以便将通知与订阅关联。

#### <a name="subscription-request-example"></a>订阅请求示例

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

`changeType`、`notificationUrl`、`resource` 和 `expirationDateTime` 属性是必需的。 如需属性定义和值，请参阅[订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)。

虽然不需要 `clientState`，但必须包括它才能符合我们建议的通知处理过程。 通过设置此属性后，可以确认收到的通知来自 Microsoft Graph 服务。 因此，该属性的值应保密，并且只有你的应用程序和 Microsoft Graph 服务知道。

如果成功，Microsoft Graph 将在正文中返回 `201 Created` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。

#### <a name="notification-endpoint-validation"></a>通知终结点验证

Microsoft Graph 在创建订阅之前验证订阅请求的 `notificationUrl` 属性中提供的通知终结点。 验证流程如下所示：

1. Microsoft Graph 将 POST 请求发送到通知 URL：

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **重要说明：** 由于 `validationToken` 是查询参数，因此客户端必须根据 HTTP 编码做法正确解码它。 如果客户端没有解码令牌，而是在下一步（响应）中使用已编码值，那么验证将会失败。 此外，客户端还应将令牌值视为不透明，因为令牌格式今后可能会更改，而不另行通知。

1. 客户端必须在 10 秒内提供具有以下特性的响应：

    - 200 (OK) 状态代码。
    - 内容类型必须是 `text/plain`。
    - 正文必须包括 Microsoft Graph 提供的验证令牌。

在响应中提供验证令牌之后，客户端应放弃验证令牌。

### <a name="renewing-a-subscription"></a>续订订阅

客户端可以续订特定过期日期的订阅，自请求时间起长达三天。 `expirationDateTime` 属性是必需的。

#### <a name="subscription-renewal-example"></a>订阅续订示例

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

如果成功，Microsoft Graph 将在正文中返回 `200 OK` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。 subscription 对象包括新的 `expirationDateTime` 值。

### <a name="deleting-a-subscription"></a>删除订阅

客户端可以通过使用其 ID 删除订阅来停止接收通知。

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

如果成功，Microsoft Graph 将返回 `204 No Content` 代码。

## <a name="notifications"></a>通知

客户端在创建订阅后开始接收通知。 资源发生更改时，Microsoft Graph 将 POST 请求发送到通知 URL。 仅针对订阅中指定类型的更改发送通知，例如 `created`。

> **注意：** 使用监视同一资源类型并使用同一通知 URL 的多个订阅时，可以发送包含具有不同订阅 ID 的多个通知的 POST。 无法保证 POST 中的所有通知都属于单个订阅。

### <a name="notification-properties"></a>通知属性

notification 对象具有以下属性：

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| subscriptionId | string | 生成通知的订阅的 ID。 |
| subscriptionExpirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | 订阅的过期时间。 |
| clientState | string | 订阅请求中指定的 `clientState` 属性（如果有）。 |
| changeType | string | 引发通知的事件类型。 例如，邮件接收时为 `created`，或将邮件标记为已读时为 `updated`。 |
| resource | string | 资源相对于 `https://graph.microsoft.com` 的 URI。 |
| resourceData | object | 此属性的内容取决于要订阅资源的类型。 |

例如，对于 Outlook 资源，`resourceData` 包含以下字段：

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| @odata.type | string | Microsoft Graph 中描述所表示对象的 OData 实体类型。 |
| @odata.id | string | 对象的 OData 标识符。 |
| @odata.etag | string | 表示对象版本的 HTTP 实体标记。 |
| id | string | 对象的标识符。 |

> **注意：**`resourceData` 中提供的 `id` 值在生成通知时有效。 某些操作（例如将邮件移动到另一个文件夹）可能会导致 `id` 在处理通知时不再有效。

### <a name="notification-example"></a>通知示例

用户收到电子邮件时，Microsoft Graph 将发送如下所示的通知：

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

请注意，`value` 字段是一个对象数组。 如果有很多排队的通知，Microsoft Graph 可能会在单个请求中发送多个项目。 来自不同订阅的通知可以包含在同一通知请求中。

### <a name="processing-the-notification"></a>处理通知

应处理你的应用收到的每个通知。 应用程序必须至少执行以下任务来处理通知：

1. 验证 `clientState` 属性。 它必须与最初使用订阅创建请求提交的值匹配。

    > **注意：** 如果不符合这个条件，无需将其视为有效通知。 通知可能不是来自 Microsoft Graph，并且可能是由未授权操作者发送的。 还应调查通知来自何处并采取适当的措施。

1. 基于业务逻辑更新应用程序。

1. 将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。 如果 Microsoft Graph 没有收到 2xx 类代码，它将重试多次发送通知。

    > **注意：** 即使 `clientState` 属性与订阅请求提交的属性不匹配，也应发送 `202 - Accepted` 状态代码。 这是一个很好的做法，因为它可以防止潜在的未授权操作者发现你可能不信任他们的通知，并且可能使用该信息来猜测 `clientState` 属性的值。

对请求中的其他通知重复该过程。

## <a name="code-samples"></a>代码示例

可在 GitHub 上获取以下代码示例。

- [面向 Node.js 的 Microsoft Graph Webhooks 示例](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [面向 ASP.NET 的 Microsoft Graph Webhooks 示例](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [使用 WebJobs SDK 的 Microsoft Graph 用户 Webhooks 示例](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a>另请参阅

- [订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)
- [获取订阅](/graph/api/subscription-get?view=graph-rest-1.0)
- [创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
