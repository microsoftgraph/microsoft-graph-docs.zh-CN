---
title: 订阅使用 Microsoft Graph 更改云打印 API 的通知
description: 了解如何使用 Microsoft Graph API 更改打印作业事件的通知。
author: jahsu
localization_priority: Priority
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: d7b4aa230e3f3b93997de51e014c52581d5f9f8b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920388"
---
# <a name="subscribe-to-change-notifications-from-cloud-printing-apis-using-microsoft-graph"></a>订阅使用 Microsoft Graph 更改云打印 API 的通知

通用打印可帮助客户将其打印基础结构移动到云，是提供高级打印功能的合作伙伴解决方案强大生产力的一部分。 当您使用 Microsoft Graph 中的云打印 API 与通用打印集成时，这些解决方案甚至会更加强大。

许多合作伙伴解决方案需要将打印作业从用户的设备发送到打印机时实时处理，这意味着当打印作业可进行处理时，需要收到通知。 通用打印为在云中移动作业时通知打印供应商解决方案提供的连接，以及可管理打印机和打印作业的 API。

本文介绍如何订阅各种打印作业事件的通知。


## <a name="get-started-with-change-notifications"></a>更改通知入门

必须先在 Azure [中注册应用程序，](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) Azure Active Directory （Azure AD） 租户中预配应用程序，才能利用通过 Microsoft Graph 更改通知。 确保应用程序已启用所需的权限范围，如本文稍后所述。


### <a name="notifications-and-subscriptions"></a>通知和订阅

通用打印当前支持两种打印作业相关方案的通知：

* PrintTask 被触发（作业启动）：应用程序可以在其 printTask（hook） 触发时订阅以接收通知。
若要详细了解如何触发任务，请参阅扩展通用 [以支持将打印内容拉取](./universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing)。 目前，仅能为作业启动事件触发 printTask。 成功创建打印作业、上传有效负载并开始作业处理后，将发生作业启动事件。  

* 作业可保存：作业启动后，第三方打印应用程序或通用打印可能会执行某些处理（例如将 XPS 有效负载转换为 PDF，用于 PDF 打印机）。 处理完成后，如果有效负载已准备好由打印机下载，则针对相应的打印作业将发生 JobFable 事件。

>[!NOTE]
>为收听 JobFableable 事件更改通知， **printTaskDefinition** 更改通知。

### <a name="create-an-application-to-listen-to-notifications"></a>创建可收听通知的应用程序

若要了解如何收听 Microsoft Graph 通知，请参阅 [通过 Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges/) 使用更改通知和修订 [设置用户数据更改通知 - 代码示例](./webhooks.md#code-samples)。


### <a name="scopes"></a>Scopes

若要订阅打印作业通知，应用程序必须具有在客户的 Azure AD 租户中批准的下列权限范围： 

* 对于 printTask 触发（作业启动）事件，"获取任务定义 [中列出的权限](/graph/api/printtaskdefinition-get?view=graph-rest-v1.0&tabs=http%22%20%5Cl%20%22permissions%22%20%5C)。 

* 对于 JobFable 事件，"创建订阅" [中列出的](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http)。

应用程序必须 [Microsoft Graph API 请求标头中生成](/graph/auth-v2-service?context=graph%2Fapi%2F1.0) Azure AD 安全令牌。 安全令牌包含按管理员批准的客户 Azure AD 租户范围内声明声明。  


## <a name="create-subscription-printtask-triggered-jobstarted-event"></a>创建订阅：printTask 触发（作业启动）事件 

某些应用程序监视传入作业的打印队列，希望在队列中具有有效作业时收到通知。 收到通知后，他们可以收集相关的作业元数据，甚至可以在打印作业中执行修改，包括中止作业或相应地修改作业属性后将作业从当前打印队列重定向到另一个队列。 

在创建打印任务 **-** 事件的通知之前，请确保应用程序创建了以下应用程序： 

- 一[Azure AD](/graph/api/print-post-taskdefinitions?view=graph-rest-v1.0&tabs=http) printTaskDefinition 应用程序。 单个任务定义可在同一 Azure AD 租户中的一个或多个打印机关联。 

- 针对 [开始新打印作业时，合作伙伴希望接收其通知的每个打印机队列的](/graph/api/printer-post-tasktriggers?view=graph-rest-v1.0&tabs=http) "PrintTaskTri你邮件"标签。 **printTaskDefinition** 需要绑定到 **PrintTaskDefinition**。 

>[!NOTE]
>一个打印机只能与一个 **printTaskTriition** 和一个 **printTaskTriition** 只能与一 **printTaskDefinition**。 但是，一 **printTaskDefinition** 可以具有一 **一个或多个 printTaskTriitions** 与其关联。 

使用客户的 Azure A [D 租户 **printTaskDefinition**，该应用程序可以使用 printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-v1.0&tabs=http)为 printTask 触发（作业启动）事件创建订阅。 创建订阅时：  

* `resource` 字段需要设置为 `print/taskDefinitions/{printTaskDefinition ID}/tasks`。 
* `changeType` 字段需要设置为 `created`。 
* " `expirationDateTime` "字段需要小于 [最大到期日期](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type)。 

如需了解更多详情，请参阅 [openTypeExtension 资源类型](/graph/api/resources/subscription?view=graph-rest-v1.0#properties)。

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions 
Content-Type: application/json
{ 
    "changeType":"created", 
    "resource":"print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "clientState":"secret", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "expirationDateTime":"2020-01-30T22:42:09Z" 
} 
```

### <a name="response"></a>响应

以下示例显示了相应的响应。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "applicationId": "{application ID}", 
    "changeType": "created", 
    "clientState": "secret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": null, 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null 
}
```


## <a name="create-subscription-jobfetchable-event"></a>创建订阅：作业可创建事件 
一些云应用程序需要准备好后从通用打印中下载打印作业。 由于在云中运行的这些应用程序不在客户的防火墙后面，因此可在下载打印作业时使用 Microsoft Graph 更改通知。

>[!NOTE]
>打印作业进入作业可打印状态时不可修改。
需要针对每个打印机队列创建可作业通知。 创建订阅时：
* " `resource` "字段需要设置为"print/printer/{printer id}/jobs"。 
* `changeType` 字段需要设置为 `updated`。 
* `notificationQueryOptions` 字段需要设置为 `$filter = isFetchable eq true`。 
* " `expirationDateTime` "字段需要小于 [最大到期日期](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type)。 

如需了解更多详情，请参阅 [openTypeExtension 资源类型](/graph/api/resources/subscription?view=graph-rest-v1.0#properties)。

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
    "changeType":"updated",
    "resource":"print/printers/{printer id}/jobs",
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}",
    "expirationDateTime":"2020-12-30T22:42:09Z",
    "clientState":"mysecret"
} 
```

### <a name="response"></a>响应

以下示例显示了相应的响应。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/printers/{printer ID}/jobs", 
    "applicationId": "{Application ID}", 
    "changeType": "updated", 
    "clientState": "mysecret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null
}
```


## <a name="renewing-a-notification-subscription"></a>续订通知订阅

Microsoft Graph 对到期时间有限制。 有关详细信息，请参阅 [的到期日期](/graph/api/resources/subscription?view=graph-rest-v1.0#maximum-length-of-subscription-per-resource-type)。 若要继续接收通知，需使用更新订阅 API 更新 [定期续订](/graph/api/subscription-update?view=graph-rest-v1.0&tabs=http)。 

## <a name="other-operations-on-notification-subscriptions"></a>通知订阅的其他操作 

应用程序 [获取](/graph/api/subscription-get?view=graph-rest-v1.0&tabs=http) 的详细信息，或者 [删除](/graph/api/subscription-delete?view=graph-rest-v1.0&tabs=http) 订阅。 有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](/graph/api/resources/webhooks?view=graph-rest-v1.0)。


## <a name="faqs"></a>常见问题
### <a name="how-does-microsoft-graph-validate-notification-urls"></a>Microsoft Graph 如何验证通知 URL？
Microsoft Graph 将验证创建订阅前订阅请求的 **notificationurl** 属性中提供的通知终结点。
有关详细信息，请参阅 [终结点验证](./webhooks.md#notification-endpoint-validation)。

### <a name="what-are-applications-expected-to-do-after-receiving-a-change-notification"></a>收到更改通知后，应用程序应执行哪些操作？
应用程序应处理和确认他们收到的每个更改通知。 有关详细信息，请参阅 [更改通知](./webhooks.md#processing-the-change-notification)。

### <a name="how-can-i-get-a-list-of-active-subscriptions"></a>如何获取活动订阅列表？
若要详细了解如何检索 Web 网站订阅列表，请参阅 [订阅](/graph/api/subscription-list?view=graph-rest-v1.0&tabs=http)。


## <a name="see-also"></a>另请参阅

- 若要深入了解 Microsoft Graph 中的云打印 API，请参阅 [云打印 API 概述](/graph/universal-print-concept-overview)。 
- 有关 Microsoft Graph 中的云打印 API 的建议或反馈，请访问 [通用打印技术社区](https://aka.ms/community/UniversalPrint)。
