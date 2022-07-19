---
title: 创建 emailThreatSubmissionPolicy
description: 创建新的 emailThreatSubmissionPolicy 对象。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 93209290935f35d25e3f349622070aa8dc88b40c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856627"
---
# <a name="create-emailthreatsubmissionpolicy"></a>创建 emailThreatSubmissionPolicy

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ThreatSubmissionPolicies.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|ThreatSubmissionPolicy.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/threatSubmission/emailThreatSubmissionPolicies
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象的 JSON 表示形式。

还可以在创建 **emailThreatSubmissionPolicy** 时指定以下属性。 这些属性与用户报告的消息设置相关。 有关详细信息，请参阅 [用户报告的消息设置](/microsoft-365/security/office-365-security/user-submission.md)。

| 属性                                 | 类型    | Description                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | String  | 指定发件人的电子邮件地址，从中向最终用户发送电子邮件通知，告知他们电子邮件是垃圾邮件、网络钓鱼还是干净。 默认值为 `null`。 可选，用于创建。                   |
| customizedReportRecipientEmailAddress    | String  | 指定最终用户报告的邮件在报告网络钓鱼、垃圾或垃圾邮件时将登陆的目标。 默认值为 `null`。 可选，用于创建。 |
| isAlwaysReportEnabledForUsers            | Boolean | 指示最终用户是否可以直接将邮件报告为垃圾邮件、网络钓鱼或垃圾邮件，而无需确认 (弹出窗口) 。 默认值为 `true`。  可选，用于创建。          |
| isAskMeEnabledForUsers                   | Boolean | 指示最终用户在将邮件报告为垃圾邮件、网络钓鱼或垃圾邮件之前是否可以使用弹出窗口进行确认。 默认值为 `true`。  可选，用于创建。 |
| isCustomizedMessageEnabled               | Boolean | 指示发送给最终用户的电子邮件通知是否已自定义电子邮件、垃圾邮件或垃圾邮件时通知他们。 默认值为 `false`。 可选，用于创建。                  |
| isCustomizedMessageEnabledForPhishing    | Boolean | 如果启用，自定义邮件仅在电子邮件报告为网络钓鱼时显示。 默认值为 `false`。 可选，用于创建。 |
| isCustomizedNotificationSenderEnabled    | Boolean | 指示是否使用自定义NotificationSenderEmailAddress 将电子邮件通知发送给最终用户的发件人电子邮件地址集。 默认值为 `false`。 可选，用于创建。               |
| isNeverReportEnabledForUsers             | Boolean | 指示最终用户是否可以根据垃圾邮件、网络钓鱼或垃圾邮件的操作将消息从一个文件夹移动到另一个文件夹，而无需实际报告。 默认值为 `true`。 可选，用于创建。         |
| isOrganizationBrandingEnabled            | Boolean | 指示是否应在发送给最终用户的电子邮件通知中使用品牌徽标。 默认值为 `false`。 可选，用于创建。        |
| isReportFromQuarantineEnabled            | Boolean | 指示最终用户是否可以从隔离页提交。 默认值为 `true`。 可选，用于创建。              |
| isReportToCustomizedEmailAddressEnabled  | Boolean | 指示是否应将最终用户报告的电子邮件发送到使用 customizedReportRecipientEmailAddress 配置的自定义邮箱。  默认值为 `false`。 可选，用于创建。              |
| isReportToMicrosoftEnabled               | Boolean | 如果启用，电子邮件将发送到 Microsoft 进行分析。 默认值为 `false`。 重新请求创建。  |
| isReviewEmailNotificationEnabled         | Boolean | 指示是否向最终用户发送电子邮件通知，该用户在管理员审阅电子邮件后报告电子邮件。默认值为 `false`. 可选，用于创建。  |


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_emailthreatsubmissionpolicy_from_emailthreatsubmissionpolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/threatSubmission/emailthreatSubmissionPolicies
Content-type: application/json

{
  "isReportToMicrosoftEnabled": true
}
```


### <a name="response"></a>响应
下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.emailThreatSubmissionPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.emailThreatSubmissionPolicy",
  "id": "DefaultReportSubmissionPolicy",
  "isReportToMicrosoftEnabled": true,
  "isReportToCustomizedEmailAddressEnabled": false,
  "isAskMeEnabledForUsers": true,
  "isAlwaysReportEnabledForUsers": true,
  "isNeverReportEnabledForUsers": true,
  "isCustomizedMessageEnabledForPhishing": false,
  "isCustomizedMessageEnabled": false,
  "customizedReportRecipientEmailAddress": null,
  "isReviewEmailNotificationEnabled": false,
  "isCustomNotificationSenderEnabled": false,
  "isOrganizationBrandingEnabled": false,
  "customizedNotificationSenderEmailAddress": null,
  "isReportFromQuarantineEnabled": false
}
```

