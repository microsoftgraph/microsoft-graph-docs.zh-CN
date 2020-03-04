---
title: 设置用户数据更改的通知
description: Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: ea8e56a657e32a5de1057f8199d27d256ab44168
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394622"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>设置用户数据更改的通知

Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。

Microsoft Graph 接受订阅请求之后，将通知推送到订阅中指定的 URL。 然后应用根据其业务逻辑执行操作。 例如，它提取更多数据、更新缓存和视图等。


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [使用 .NET Core 生成 Webhook 应用](/graph/tutorials/change-notifications)

默认情况下，更改通知不包含资源数据，`id` 除外。 如果应用需要资源数据，则可以调用 Microsoft Graph API 以获取完整资源。 本文使用**用户**资源作为使用通知的示例。

应用还可订阅包含资源数据的更改通知，避免执行其他 API 调用来访问数据。 此类应用将需要实现额外的代码来处理此类通知的要求，具体而言：响应订阅生命周期通知，验证通知的真实性，以及解密资源数据。 将来会有更多资源类型支持此类型的通知。 有关如何使用这些通知的详细信息，请参阅[设置包含资源数据的更改通知（预览版）](webhooks-with-resource-data.md)。

## <a name="supported-resources"></a>支持的资源

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

- Outlook [邮件][]
- Outlook [事件][]
- Outlook 个人[联系人][]
- [用户][]
- [组][]
- Office 365 组[对话][]
- 用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容
- OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容
- 安全[警报][]
- Teams [callRecord][]（预览版）

可以创建对特定 Outlook 文件夹的订阅，例如收件箱：`me/mailFolders('inbox')/messages`

或以下顶级资源的订阅：`me/messages`、`me/contacts`、`me/events`、`users` 或 `groups`

或以下特定资源实例的订阅：`users/{id}`、`groups/{id}`、`groups/{id}/conversations`

或用户个人 OneDrive 中任何文件夹的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`

或 SharePoint/OneDrive for Business 驱动器根文件夹的订阅：`/drive/root`

或对新[安全性 API](security-concept-overview.md) 警报的订阅：`/security/alerts?$filter=status eq 'newAlert'`、`/security/alerts?$filter=vendorInformation/provider eq 'ASC'`

### <a name="azure-ad-resource-limitations"></a>Azure AD 资源限制

基于 Azure AD 的资源（用户、组）采用了某些限制，超出限制时将会产生错误：

> **请注意**：这些限制不适用于来自 Azure AD 以外的服务的资源。 例如，应用可以创建许多更多的 `message` 或 `event` 资源订阅，这些订阅受到 Microsoft Graph 中的 Exchange Online 服务支持。

- 最大订阅配额：

  - 每个应用：总订阅数 50,000
  - 每个租户：所有应用的总订阅数 1000
  - 每个应用和租户组合：总订阅数 100

超出限制时，尝试创建订阅将导致[错误响应](errors.md) - `403 Forbidden`。 `message` 属性将说明已超出什么限制。

- 不支持 Azure AD B2C 租户。

- 个人 Microsoft 帐户不支持用户实体的通知。

### <a name="outlook-resource-limitations"></a>Outlook 资源限制

订阅 Outlook 资源（如**邮件**、**事件**或**联系人**）时，如果选择使用资源路径中的*用户主体名称* UPN，则在 UPN 包含撇号的情况下，订阅请求可能会失败。 请考虑使用 GUID 用户 ID 而不是 UPN，以避免遇到此问题。 例如，请勿使用资源路径：

`/users/sh.o'neal@contoso.com/messages`

请使用： 

`/users/{guid-user-id}/messages`

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

`resource` 属性指定要被监视以进行更改的资源。 例如，可以创建特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`，或代表由管理员同意的用户：`users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。

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
| tenantId | string | 发出通知的租户的 ID。 |

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
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
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

1. 将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。 如果 Microsoft Graph 未收到 2xx 类代码，它将在大约 4 小时的一段时间内尝试多次发布通知，之后，通知将被删除，且不会发送。

    > **注意：** 收到通知后立即发送 `202 - Accepted` 状态代码，甚至在验证其真实性之前。 只是确认接收通知，防止不必要的重试。 当前超时是 30 秒，但将来可能会减少，以优化服务性能。

1. 验证 `clientState` 属性。 它必须与最初使用订阅创建请求提交的值匹配。

    > **注意：** 如果不符合这个条件，无需将其视为有效通知。 通知可能不是来自 Microsoft Graph，并且可能是由未授权操作者发送的。 还应调查通知来自何处并采取适当的措施。

1. 基于业务逻辑更新应用程序。

对请求中的其他通知重复该过程。

## <a name="code-samples"></a>代码示例

可在 GitHub 上获取以下代码示例。

- [Microsoft Graph 培训模块 - 在 Microsoft Graph 中使用变更通知和变更跟踪](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [面向 Node.js 的 Microsoft Graph Webhooks 示例](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [面向 ASP.NET 的 Microsoft Graph Webhooks 示例](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [使用 WebJobs SDK 的 Microsoft Graph 用户 Webhooks 示例](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a>另请参阅

- [订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)
- [获取订阅](/graph/api/subscription-get?view=graph-rest-1.0)
- [创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [更改通知教程](/graph/tutorials/change-notifications)
- [生命周期通知（预览版）](/graph/concepts/webhooks-outlook-authz.md)

[联系人]: /graph/api/resources/contact?view=graph-rest-1.0
[对话]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[事件]: /graph/api/resources/event?view=graph-rest-1.0
[组]: /graph/api/resources/group?view=graph-rest-1.0
[邮件]: /graph/api/resources/message?view=graph-rest-1.0
[用户]: /graph/api/resources/user?view=graph-rest-1.0
[警报]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-beta
