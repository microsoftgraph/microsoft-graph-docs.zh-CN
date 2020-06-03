---
title: 设置用户数据更改的通知
description: Microsoft Graph API 使用 webhook 机制将更改通知传递给客户端。客户端是一种 web 服务，可用于配置自己的 URL 以接收更改通知。客户端应用使用更改通知在更改时更新其状态。
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 562eaccdd776ed22a4e171f6c0107f83be6acaab
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524251"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>设置用户数据更改的通知

Microsoft Graph API 使用 webhook 机制将更改通知传递给客户端。客户端是一种 web 服务，可用于配置自己的 URL 以接收更改通知。客户端应用使用更改通知在更改时更新其状态。

在 Microsoft Graph 接受订阅请求后，它会将更改通知推送到订阅中指定的 URL。 然后应用根据其业务逻辑执行操作。 例如，它提取更多数据、更新缓存和视图等。


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [使用 .NET Core 生成 Webhook 应用](/graph/tutorials/change-notifications)

默认情况下，更改通知不包含资源数据，`id` 除外。 如果应用需要资源数据，则可以调用 Microsoft Graph API 以获取完整资源。 本文使用**用户**资源作为使用更改通知的示例。

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
- 团队[callRecord][]
- Teams [chatMessage][]（预览）

可以创建对特定 Outlook 文件夹的订阅，例如收件箱：`me/mailFolders('inbox')/messages`

或者顶级资源：、、、、 `/me/messages` `/me/contacts` `/me/events` `users` `groups` 或`/communications/callRecords`

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

- 个人 Microsoft 帐户不支持用户实体的 Changfe 通知。

- 用户和租订阅存在一个[已知问题](known-issues.md#change-notifications)。

### <a name="outlook-resource-limitations"></a>Outlook 资源限制

订阅 Outlook 资源（如**邮件**、**事件**或**联系人**）时，如果选择使用资源路径中的*用户主体名称* UPN，则在 UPN 包含撇号的情况下，订阅请求可能会失败。 请考虑使用 GUID 用户 ID 而不是 UPN，以避免遇到此问题。 例如，请勿使用资源路径：

`/users/sh.o'neal@contoso.com/messages`

请使用： 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a>订阅生命周期

订阅的生命周期有限。 应用需要在订阅到期前续订订阅。 否则，需要新建订阅。 有关最长有效期的列表，请参阅[每个资源类型的最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。

应用还可以随时取消订阅以停止获取更改通知。

## <a name="managing-subscriptions"></a>管理订阅

客户端可以创建订阅、续订订阅和删除订阅。

### <a name="creating-a-subscription"></a>创建订阅

创建订阅是开始接收对资源的更改通知的第一步。订阅过程如下所示：

1. 客户端发送特定资源的订阅 (POST) 请求。

1. Microsoft Graph 验证请求。

    - 如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。
    - 如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。

1. 客户端将验证令牌发送回 Microsoft Graph。

1. Microsoft Graph 将响应发送回客户端。

客户端必须存储订阅 ID，才能将更改通知与订阅关联。

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

尽管 `clientState` 不是必需的，但必须将其包括在内，才能符合我们建议的更改通知处理过程。 通过设置此属性，可以确认收到的更改通知来自 Microsoft Graph 服务。 因此，该属性的值应保密，并且只有你的应用程序和 Microsoft Graph 服务知道。

如果成功，Microsoft Graph 将在正文中返回 `201 Created` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。

#### <a name="notification-endpoint-validation"></a>通知终结点验证

Microsoft Graph 在创建订阅之前验证订阅请求的 `notificationUrl` 属性中提供的通知终结点。 验证流程如下所示：

1. Microsoft Graph 将 POST 请求发送到通知 URL：

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **重要说明：** 由于 `validationToken` 是查询参数，因此客户端必须根据 HTTP 编码做法正确解码它。 如果客户端没有解码令牌，而是在下一步（响应）中使用已编码值，那么验证将会失败。 此外，客户端还应将令牌值视为不透明，因为令牌格式今后可能会更改，而不另行通知。

1. 客户端必须在 10 秒内提供具有以下特性的响应：

    - 200 (OK) 状态代码。
    - 内容类型必须是 `text/plain`。
    - 正文必须包括 Microsoft Graph 提供的验证令牌。

在响应中提供验证令牌之后，客户端应放弃验证令牌。

另外，可以使用 [Microsoft Graph Postman Collection](use-postman.md) 来确认终结点能否正确实现验证请求。 “杂项”**** 文件夹中的“订阅验证”**** 请求提供了单元测试，可验证终结点提供的响应。  

![验证响应测试结果](images/change-notifications/validation-request-tests-results.png)

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

客户端可以通过使用其 ID 删除订阅来停止接收更改通知。

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

如果成功，Microsoft Graph 将返回 `204 No Content` 代码。

## <a name="change-notifications"></a>更改通知

客户端在创建订阅后开始接收更改通知。 资源发生更改时，Microsoft Graph 将 POST 请求发送到通知 URL。 仅为订阅中指定类型的更改发送更改通知，例如 `created` 。

> **注意：** 如果使用多个订阅来监视相同的资源类型并使用相同的通知 URL，则可以发送包含不同订阅 Id 的多个更改通知的帖子。 无法保证帖子中的所有更改通知都属于单个订阅。

### <a name="change-notification-example"></a>更改通知示例

> **注意：** 有关在传递更改通知时发送的数据的完整说明，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

当用户收到电子邮件时，Microsoft Graph 将发送一条更改通知，如下所示：

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "sequenceNumber": 10,
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

> **注意：** 该 `value` 字段是一个对象数组。 当多个更改通知被排入队列时，Microsoft Graph 可能会在一个请求中发送多个项目。 来自不同订阅的更改通知可以包含在同一个请求中。

### <a name="processing-the-change-notification"></a>处理更改通知

应处理应用程序收到的每个更改通知。 以下是您的应用程序处理更改通知时必须执行的最低任务：

1. 将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。 如果 Microsoft Graph 没有收到2xx 类代码，它会在大约4小时的一段时间内尝试发布更改通知一段时间。之后，更改通知将被丢弃，并且不会被传递。

    > **注意：**`202 - Accepted`收到更改通知后立即发送状态代码，即使在验证其真实性之前也是如此。 您只需确认收到更改通知并防止不必要的重试。 当前超时是 30 秒，但将来可能会减少，以优化服务性能。

1. 验证 `clientState` 属性。 它必须与最初使用订阅创建请求提交的值匹配。

    > **注意：** 如果不满足此条件，则不应将其视为有效的更改通知。 更改通知可能不是来自 Microsoft Graph，可能是由恶意参与者发送的。 您还应调查更改通知的来源，并采取相应的措施。

1. 基于业务逻辑更新应用程序。

对请求中的其他更改通知重复此操作。

## <a name="code-samples"></a>代码示例

可在 GitHub 上获取以下代码示例。

- [Microsoft Graph 培训模块 - 在 Microsoft Graph 中使用变更通知和变更跟踪](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [面向 Node.js 的 Microsoft Graph Webhooks 示例](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [适用于 ASP.NET Core 的 Microsoft Graph Webhook 示例](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [面向 Java Spring 的 Microsoft Graph Webhooks 示例](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a>防火墙配置

可选择性地配置防火墙，以保护通知 URL，仅允许来自 Microsoft Graph 的入站连接。 这使您可以减少发送到通知 URL 的无效更改通知的暴露风险。 这些无效的更改通知可尝试触发您实现的自定义逻辑。 有关 Microsoft Graph 用于传递更改通知的 IP 地址的完整列表，请参阅 [Office 365 的其他终结点](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls)。

> **注意：** 用于传递更改通知的已列出 IP 地址可以随时更新，恕不另行通知。

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
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
