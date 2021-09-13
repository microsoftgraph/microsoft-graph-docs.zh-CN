---
title: 减少缺失订阅和更改通知
description: 订阅更改通知的应用可能会删除其订阅并错过一些更改通知。 应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续更改通知流程。
author: davidmu1
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 519178ee7609d615c32c628721b3154853273422
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108749"
---
# <a name="reduce-missing-subscriptions-and-change-notifications"></a>减少缺失订阅和更改通知

订阅更改通知的应用可能会删除其订阅并错过一些更改通知。 应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续更改通知流程。

某些事件可能导致订阅被删除。这些事件包括:

- 用户的密码已重置
- 用户的设备不合规
-   用户的帐户已吊销

发生此类事件时，Microsoft Graph 将发送特殊生命周期通知，`subscriptionRemoved`。

如果无法将更改通知传递到应用，Microsoft Graph 还会发送另一个生命周期通知 `missed`。

订阅更改通知的应用应收听 `subscriptionRemoved` 和 `missed` 信号，并执行以下操作：

- 收到 `subscriptionRemoved` 生命周期通知后，该应用应重新创建订阅以保持连续流程。
- 收到 `missed` 生命周期通知后，该应用使用 Microsoft Graph 重新同步资源数据。

若要接收生命周期通知，你可以使用已接收更改通知的现有 **notificationUrl** 终结点，也可以注册单独的 **lifecycleNotificationUrl** 以在单独的终结点中接收 `subscriptionRemoved` 和 `missed` 生命周期通知。

在以下资源类型上创建的订阅支持生命周期通知：

- Outlook [邮件][]
- Outlook [事件][]
- Outlook 个人[联系人][]
- Teams [chatMessage][]

对于其他资源类型，在创建订阅时仍然可以提供 `lifecycleNotificationUrl`，并且只要资源实现订阅，应用程序就会收到生命周期通知。

## <a name="creating-a-subscription"></a>创建订阅

创建订阅时，你必须使用 **lifecycleNotificationUrl** 属性指定单独的通知终结点。 如果指定终结点，所有当前和未来类型的生命周期通知都将传递到那里。 否则，将无法传递 `subscriptionRemoved` 和 `missed` 生命周期通知。 此终结点可与 **notificationUrl** 相同。

### <a name="subscription-request-example"></a>订阅请求示例

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2020-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> [!IMPORTANT]
> 对两个通知 URL 使用相同的主机名 (FQDN)。 

需要按照 [管理订阅](webhooks.md#managing-subscriptions)中的说明验证两个终结点。 如果选择针对两个终结点使用同一 URL，将收到并响应两个验证请求。

> **注意：** 无法更新 (`PATCH`) 现有订阅以添加 **lifecycleNotificationUrl** 属性。 应删除此类现有订阅，创建新订阅并指定 **lifecycleNotificationUrl** 属性。 没有 **lifecycleNotificationUrl** 属性的现有订阅将接收 `subscriptionRemoved` 和 `missed` 通知。

## <a name="responding-to-subscriptionremoved-notifications"></a>响应 subscriptionRemoved 通知

`subscriptionRemoved` 生命周期通知会通知你订阅已删除，如果想要继续接收更改通知，应重新创建。 

可以创建长期订阅（3 天），更改通知将开始流向 **notificationUrl**。 但是，资源数据的访问条件可能会随时间变化。 例如，服务中的事件可能会发生，需要应用程序对于用户重新进行身份验证。 在此类情况下，流程如下所示：

1. 服务检测到需要从 Microsoft Graph 删除订阅。
    
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
- 与更改通知类似，生命周期通知可以一起批处理（在 **值** 数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。 相应地批处理每个生命周期通知。

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="actions-to-take"></a>要采取的操作

1. 通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。
2. [验证](webhooks.md#change-notifications)生命周期通知的真实性。
3. 确保应用程序具有执行下一步操作的有效访问令牌。 
  > **注意：** 如果使用其中一个 [身份验证库](/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。 请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。

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
- 与更改通知类似，生命周期通知可以一起批处理（在 **值** 数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。 相应地批处理每个生命周期通知。

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="actions-to-take"></a>要采取的操作

1. 通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。
    - 如果忽略这些信号，则无需执行其他任何操作。否则:
2. [验证](webhooks.md#change-notifications)生命周期通知的真实性。
3. 执行资源的完整数据重新同步，以标识未作为通知发送的更改。 

## <a name="responding-to-reauthorizationrequired-notifications"></a>响应 reauthorizationRequired 通知

收到`reauthorizationRequired`生命周期通知时，必须重新授权该订阅以保持数据流。

可以创建长期订阅（3 天），更改通知流向 **notificationUrl**。 自订阅创建起访问条件发生变化时，Microsoft Graph 可能要求你重新授权订阅，证明仍能访问资源数据。 下面是影响数据访问的更改示例：

- 租户管理员可能会吊销应用程序读取资源的权限。
- 在交互方案中，向应用程序提供身份验证令牌的用户，可能会受限于基于多种因素的动态策略，如位置、设备状态或风险评估。 例如，如果用户更改了物理位置，则该用户可能无法再访问该数据，并且应用程序无法重新授权订阅。 有关控制访问的动态策略的详细信息，请参阅 [Azure AD 条件性访问策略](/azure/active-directory/conditional-access/overview)。 

以下步骤代表活动的订阅的授权质询流：

1. Microsoft Graph 需要重新授权的订阅。
    
    发生这种情况的原因可能随资源而异，可能随着时间推移而发生变化。 无论重新授权事件如何造成的，你都必须对作出响应。

2. Microsoft Graph 向 **lifecycleNotificationUrl** 发送授权质询通知。

    请注意，更改通知流可能会持续一段时间，为你提供额外的响应时间。 但是更改通知传递将最终暂停，直至执行了所需操作。

3. 采用以下两种方法之一来响应此生命周期通知：
    - 重新授权订阅。这不会延长订阅的到期日期。
    - 续订订阅。这会重新授权并延长到期日期。

    注意：两项操作都要求提供有效的身份验证令牌，类似于[新建订阅](webhooks.md#creating-a-subscription)或[到期前续订订阅](webhooks.md#renewing-a-subscription)。

4. 如果成功重新授权或续订订阅，更改通知将继续。否则，更改通知将保持暂停。

### <a name="reauthorizationrequired-notification-example"></a>reauthorizationRequired 通知示例

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

有关此类型通知的一些注意事项：

- “`"lifecycleEvent": "reauthorizationRequired"`”字段将通知标识为授权质询。 其他类型的生命周期通知也是可能的，将来会引入新的通知。
- 生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。
- 与更改通知类似，可以共同对生命周期通知进行批处理（**值** 集），各通知可能有不同的 **lifecycleEvent** 值。 相应地批处理每个生命周期通知。

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="actions-to-take"></a>要采取的操作

1. 通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。
2. [验证](webhooks.md#change-notifications)生命周期通知的真实性。
3. 确保应用程序具有执行下一步操作的有效访问令牌。 
  > **注意：** 如果使用其中一个 [身份验证库](/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。 请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。

4. 调用下列两个API中的任意一个。 如果 API 调用成功，则更改通知流将继续。

    - 调用`/reauthorize`操作以重新批准订阅，但不延长到期日期：
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - 执行定期续订操作，以同时进行重新授权和续订：
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      续订可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户对资源的访问权限。 应用程序可能需要从用户获取新的访问令牌以成功重新授权订阅。 
      
      以后可以随时重试这些操作，例如访问条件发生变化时。 生命周期通知发送至应用再次成功重新创建订阅之间的有关资源更改的任何通知将丢失。 在这种情况下，应用程序应单独获取这些更改。

### <a name="additional-information"></a>其他信息

以下信息可帮助你了解身份验证质询：

- 授权质询不会替代到期前续订资源更改通知的需要。 

    虽然可以选择在收到授权质询时续订订阅，但 Microsoft Graph 可能不会对所有订阅进行质询。 例如，没有任何活动且没有更改通知挂起传递的订阅不表示对应用有任何重新授权质询。 请务必在订阅到期前 [续订订阅](webhooks.md#renewing-a-subscription)。

- 授权质询的频率可能会发生更改。

    不要对授权质询频率进行假设。 这些生命周期通知会告诉你执行操作的时间，无需跟踪需要重新授权的订阅。 准备好每隔几分钟处理每个订阅的授权质询，极少情况下，只针对部分订阅。

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a>前瞻性的代码处理生命周期通知

将来，Microsoft Graph 将添加更多类型的订阅生命周期通知。 它们将被发布到相同的终结点：**lifecycleNotificationUrl**，但是它们在 **lifecycleEvent** 下将具有不同的值，并且可能包含稍微不同的模式和属性，这些模式和属性特定于将为其发布的方案。

你应该以前瞻性的方式实现代码，以便在 Microsoft Graph 引入新类型的生命周期通知时不会出错。建议使用以下方法:

1. 使用 **lifecycleEvent** 属性将每个生命周期通知显式标识为你支持的事件。 例如，查找 `"lifecycleEvent": "subscriptionRemoved"` 属性标识特定事件并处理它。

2. 请留意新方案的通知公告。将来可能会有更多类型的生命周期通知。

3. 在你的应用中，忽略应用无法识别的任何生命周期通知，并记录它们以获得认知。

4. 你可以自行决定查找新生命周期通知的相关文档，并根据需要实施对它们的支持。

## <a name="see-also"></a>另请参阅

- [订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)
- [获取订阅](/graph/api/subscription-get?view=graph-rest-1.0)
- [创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [删除订阅](/graph/api/subscription-delete?view=graph-rest-1.0)
- [更新订阅](/graph/api/subscription-update?view=graph-rest-1.0)


[联系人]: /graph/api/resources/contact?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
