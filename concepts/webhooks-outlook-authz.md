---
title: 减少 Outlook 资源丢失的订阅和更改通知（预览版）
description: 由于用户密码重置等安全事件，Outlook 可能会暂停传递更改通知。 需要处理特殊生命周期事件（`subscriptionRemoved` 和 `missed`），以确保传递更改通知不间断。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 2c299f2438ede2dc019fab63b7b84948fc0968af
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408062"
---
# <a name="reduce-missing-subscriptions-and-change-notifications-for-outlook-resources-preview"></a>减少 Outlook 资源丢失的订阅和更改通知（预览版） 

订阅 Outlook 资源更改通知的应用可能会删除其订阅并错过一些更改通知。 应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续更改通知流程。

Outlook 中的某些事件可能导致订阅被删除。 这些事件包括：

- 用户的密码已重置
- 用户的设备不合规
-   用户的帐户已吊销

发生此类事件时，Outlook 将发送特殊生命周期通知 `subscriptionRemoved`。

如果无法将更改通知传递到应用，Outlook 还会发送另一个生命周期通知 `missed`。

订阅 Outlook 资源更改通知的应用（如**邮件**和**事件**）应收听 `subscriptionRemoved` 和 `missed` 信号，并执行以下操作：

- 收到 `subscriptionRemoved` 生命周期通知后，该应用应重新创建订阅以保持连续流程。
- 收到 `missed` 生命周期通知后，该应用使用 Microsoft Graph 重新同步资源数据。

若要接收生命周期通知，你可以使用已接收更改通知的现有 **notificationUrl** 终结点，也可以注册单独的 **lifecycleNotificationUrl** 以在单独的终结点中接收 `subscriptionRemoved` 和 `missed` 生命周期通知。

## <a name="creating-a-subscription"></a>创建订阅

创建订阅时，你必须使用 **lifecycleNotificationUrl** 属性指定单独的通知终结点。 如果指定终结点，所有当前和未来类型的生命周期通知都将传递到那里。 否则，将无法传递 `subscriptionRemoved` 和 `missed` 生命周期通知。

> **注意：** 只能使用 Microsoft Graph beta API 设置或读取 **lifecycleNotificationUrl** 属性。 但是，使用 beta API 创建的订阅与使用 v1.0 创建的订阅存储在同一个生产环境中，因此除了使用 v1.0 API 创建的订阅外，还可以实现新 Outlook 流程。

> 通过 v1.0 API 创建的订阅将收到生命周期通知。 

### <a name="subscription-request-example"></a>订阅请求示例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> **重要提示：** 对两个通知 URL 使用相同的主机名。 

> **注意：** 需要按照[管理订阅](webhooks.md#managing-subscriptions)中的说明验证两个终结点。
如果选择对两个终结点使用相同的 URL，将收到并响应两个验证请求。

> **注意：** 无法更新 (`PATCH`) 现有订阅以添加 **lifecycleNotificationUrl** 属性。 应删除此类现有订阅，创建新订阅并指定 **lifecycleNotificationUrl** 属性。 没有 **lifecycleNotificationUrl** 属性的现有订阅将接收 `subscriptionRemoved` 和 `missed`。

## <a name="responding-to-subscriptionremoved-notifications"></a>响应 subscriptionRemoved 通知

`subscriptionRemoved` 生命周期通知会通知你订阅已删除，如果想要继续接收更改通知，应重新创建。 

可以创建长期订阅（3 天），更改通知将开始流向 **notificationUrl**。 但是，资源数据的访问条件可能会随时间变化。 例如，Outlook 服务中的事件可能会发生，需要应用程序对于用户重新进行身份验证。 在此类情况下，流程如下所示：

1. Outlook 检测到需要从 Microsoft Graph 删除订阅。
    
    这些事件没有固定的节奏。 对于某些资源，它们可能经常发生，而对于其他资源，几乎永远不会发生。

2. Microsoft Graph 将发送 `subscriptionRemoved` 生命周期通知到 **lifecycleNotificationUrl**（如果指定）。  

3. 可以通过为同一资源创建新订阅来响应此生命周期通知。 为此，你需要提供有效的访问令牌；在某些情况下，这意味着应用程序需要重新验证用户以获取新的有效访问令牌。

4. 如果成功创建新订阅，更改通知将再次开始流动。 但是，如果失败（例如，应用程序无法获取有效的访问令牌），将不会发送更改通知。

5. 创建新订阅后，可以同步资源数据以标识任何缺失的更改。

### <a name="subscriptionremoved-notification-example"></a>subscriptionRemoved 通知示例

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

有关此类型通知的一些注意事项：
- `"lifecycleEvent": "subscriptionRemoved"` 字段将此通知指定为与订阅删除相关。 其他类型的生命周期通知也是可能的，将来会引入新的通知。
- 生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。
- 与更改通知类似，生命周期通知可以一起批处理（在**值**数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。 相应地批处理每个生命周期通知。

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="actions-to-take"></a>要采取的操作

1. 通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。
2. [验证](webhooks.md#change-notifications)生命周期通知的真实性。
3. 确保应用程序具有执行下一步操作的有效访问令牌。 
  > **注意：** 如果使用其中一个[身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。 请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。

4. 使用[此处](webhooks.md#subscription-request-example)描述的标准流程创建新订阅。

  > **注意：** 此操作可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户访问资源。 应用程序可能需要从用户处获取新的访问令牌以成功重新授权订阅。 以后可以随时重试这些操作，例如，当访问条件发生变化时。 从生命周期通知发送到应用程序成功重新创建订阅的时间段内的任何资源更改都将丢失。 该应用需要自己获取这些更改。

5. 创建新订阅后，从收到此资源的更改通知的上次已知时间同步任何缺失的资源数据；例如：`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`

## <a name="responding-to-missed-notifications"></a>响应错过的通知

这些信号通知你可能尚未发送某些更改通知。 你应决定是否忽略或处理这些信号。

### <a name="notification-example"></a>通知示例

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

有关此类型通知的一些注意事项：
- `"lifecycleEvent": "missed"` 字段将此指定为有关错过的更改通知的信号。 其他类型的生命周期通知也是可能的，将来会引入新的通知。
- 生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。
- 与更改通知类似，生命周期通知可以一起批处理（在**值**数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。 相应地批处理每个生命周期通知。

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="actions-to-take"></a>要采取的操作

1. 通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。
    - 如果忽略这些信号，则无需执行其他任何操作。 或者：
2. [验证](webhooks.md#change-notifications)生命周期通知的真实性。
3. 执行资源的完整数据重新同步，以标识未作为通知发送的更改。 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a>前瞻性的代码处理生命周期通知

将来，Microsoft Graph 将添加更多类型的订阅生命周期通知。 它们将被发布到相同的终结点：**lifecycleNotificationUrl**，但是它们在 **lifecycleEvent** 下将具有不同的值，并且可能包含稍微不同的模式和属性，这些模式和属性特定于将为其发布的方案。

你应该以前瞻性的方式实现代码，以便在 Microsoft Graph 引入新类型的生命周期通知时不会中断。 建议使用以下方法：

1. 使用 **lifecycleEvent** 属性将每个生命周期通知显式标识为你支持的事件。 例如，查找 `"lifecycleEvent": "subscriptionRemoved"` 属性标识特定事件并处理它。

2. 注意有关新方案的生命周期通知公告。 将来可能会有更多类型的生命周期通知。

3. 在你的应用中，忽略应用无法识别的任何生命周期通知，并记录它们以获得认知。

4. 你可以自行决定查找新生命周期通知的相关文档，并根据需要实施对它们的支持。

## <a name="see-also"></a>另请参阅

- [订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)
- [获取订阅](/graph/api/subscription-get?view=graph-rest-1.0)
- [创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [删除订阅](/graph/api/subscription-delete?view=graph-rest-1.0)
- [更新订阅](/graph/api/subscription-update?view=graph-rest-1.0)
