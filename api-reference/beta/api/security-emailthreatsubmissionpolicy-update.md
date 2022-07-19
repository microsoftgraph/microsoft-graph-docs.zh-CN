---
title: 更新 emailThreatSubmissionPolicy
description: 更新 emailThreatSubmissionPolicy 对象的属性。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 78ceedcdc0436f8f8eb941d6f95c65a0e6d10bba
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856532"
---
# <a name="update-emailthreatsubmissionpolicy"></a>更新 emailThreatSubmissionPolicy
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [emailThreatSubmissionPolicy 对象的](../resources/security-emailthreatsubmissionpolicy.md) 属性。

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
PATCH security/threatSubmission/emailThreatSubmissionPolicies/{emailThreatSubmissionPoliciesId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

这些属性与 **用户报告的消息设置** 相关。 有关详细信息，请参阅 [用户报告的消息设置](/microsoft-365/security/office-365-security/user-submission.md)。

| 属性                                 | 类型    | Description                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | String  | 指定发件人的电子邮件地址，从中向最终用户发送电子邮件通知，告知他们电子邮件是垃圾邮件、网络钓鱼还是干净。 默认值为 `null`。 可选，用于创建。                   |
| customizedReportRecipientEmailAddress    | String  | 指定最终用户报告的邮件在报告网络钓鱼、垃圾或垃圾邮件时将登陆的目标。 默认值为 `null`。 可选，用于创建。 |
| isAlwaysReportEnabledForUsers            | 布尔 | 指示最终用户是否可以直接将邮件报告为垃圾邮件、网络钓鱼或垃圾邮件，而无需确认 (弹出窗口) 。 默认值为 `true`。  可选，用于创建。          |
| isAskMeEnabledForUsers                   | Boolean | 指示最终用户在将邮件报告为垃圾邮件、网络钓鱼或垃圾邮件之前是否可以使用弹出窗口进行确认。 默认值为 `true`。  可选，用于创建。 |
| isCustomizedMessageEnabled               | 布尔 | 指示发送给最终用户的电子邮件通知是否已自定义电子邮件、垃圾邮件或垃圾邮件时通知他们。 默认值为 `false`。 可选，用于创建。                  |
| isCustomizedMessageEnabledForPhishing    | Boolean | 如果启用，自定义邮件仅在电子邮件报告为网络钓鱼时显示。 默认值为 `false`。 可选，用于创建。 |
| isCustomizedNotificationSenderEnabled    | Boolean | 指示是否使用自定义NotificationSenderEmailAddress 将电子邮件通知发送给最终用户的发件人电子邮件地址集。 默认值为 `false`。 可选，用于创建。               |
| isNeverReportEnabledForUsers             | Boolean | 指示最终用户是否可以根据垃圾邮件、网络钓鱼或垃圾邮件的操作将消息从一个文件夹移动到另一个文件夹，而无需实际报告。 默认值为 `true`。 可选，用于创建。         |
| isOrganizationBrandingEnabled            | Boolean | 指示是否应在发送给最终用户的电子邮件通知中使用品牌徽标。 默认值为 `false`。 可选，用于创建。        |
| isReportFromQuarantineEnabled            | Boolean | 指示最终用户是否可以从隔离页提交。 默认值为 `true`。 可选，用于创建。              |
| isReportToCustomizedEmailAddressEnabled  | Boolean | 指示是否应将最终用户报告的电子邮件发送到使用 customizedReportRecipientEmailAddress 配置的自定义邮箱。  默认值为 `false`。 可选，用于创建。              |
| isReportToMicrosoftEnabled               | Boolean | 如果启用，电子邮件将发送到 Microsoft 进行分析。 默认值为 `false`。 重新请求创建。  |
| isReviewEmailNotificationEnabled         | Boolean | 指示是否向最终用户发送电子邮件通知，该用户在管理员审阅电子邮件后报告电子邮件。默认值为 `false`. 可选，用于创建。  |



## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "update_emailthreatsubmissionpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/threatSubmission/emailthreatSubmissionPolicies/DefaultReportSubmissionPolicy
Content-type: application/json

{
  "isReportToMicrosoftEnabled": false
}
```


### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

