---
title: emailThreatSubmissionPolicy 资源类型
description: 表示组织报告潜在威胁和垃圾邮件的准则。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d34e239e9c7717aaf21d2619a47ab3a005b42d7b
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856680"
---
# <a name="emailthreatsubmissionpolicy-resource-type"></a>emailThreatSubmissionPolicy 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示组织报告潜在威胁和垃圾邮件的准则。 它用于在 Microsoft Outlook 中报告潜在威胁和垃圾邮件时自定义组织的最终用户威胁提交体验。


继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 emailThreatSubmissionPolicies](../api/security-emailthreatsubmissionpolicy-list.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 集合|获取 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象及其属性的列表。|
|[创建 emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-post-emailthreatsubmissionpolicies.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|创建新的 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象。|
|[获取 emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-get.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|读取 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象的属性和关系。|
|[更新 emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-update.md)|无|更新 [emailThreatSubmissionPolicy 对象的](../resources/security-emailthreatsubmissionpolicy.md) 属性。|
|[删除 emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-delete.md)|无|删除 [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) 对象。|

## <a name="properties"></a>属性
| 属性                                 | 类型    | Description                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | String  | 指定发件人的电子邮件地址，从中向最终用户发送电子邮件通知，告知他们电子邮件是垃圾邮件、网络钓鱼还是干净。 默认值为 `null`。 可选，用于创建。                   |
| customizedReportRecipientEmailAddress    | String  | 指定最终用户报告的邮件在报告网络钓鱼、垃圾或垃圾邮件时将登陆的目标。 默认值为 `null`。 可选，用于创建。 |
| id                                       | String  | 仅支持一个 ID。 默认值为 `DefaultReportSubmissionPolicy`。 |
| isAlwaysReportEnabledForUsers            | Boolean | 指示最终用户是否可以直接将邮件报告为垃圾邮件、网络钓鱼或垃圾邮件，而无需确认 (弹出窗口) 。 默认值为 `true`。  可选，用于创建。          |
| isAskMeEnabledForUsers                   | Boolean | 指示最终用户在将邮件报告为垃圾邮件、网络钓鱼或垃圾邮件之前是否可以使用弹出窗口进行确认。 默认值为 `true`。  可选，用于创建。   |
| isCustomizedMessageEnabled               | Boolean | 指示发送给最终用户的电子邮件通知是否已自定义电子邮件、垃圾邮件或垃圾邮件时通知他们。 默认值为 `false`。 可选，用于创建。    |
| isCustomizedMessageEnabledForPhishing    | Boolean | 如果启用，自定义邮件仅在电子邮件报告为网络钓鱼时显示。 默认值为 `false`。 可选，用于创建。 |
| isCustomizedNotificationSenderEnabled    | Boolean | 指示是否使用自定义NotificationSenderEmailAddress 将电子邮件通知发送给最终用户的发件人电子邮件地址集。 默认值为 `false`。 可选，用于创建。  |
| isNeverReportEnabledForUsers             | Boolean | 指示最终用户是否可以根据垃圾邮件、网络钓鱼或垃圾邮件的操作将消息从一个文件夹移动到另一个文件夹，而无需实际报告。 默认值为 `true`。 可选，用于创建。         |
| isOrganizationBrandingEnabled            | Boolean | 指示是否应在发送给最终用户的电子邮件通知中使用品牌徽标。 默认值为 `false`。 可选，用于创建。        |
| isReportFromQuarantineEnabled            | Boolean | 指示最终用户是否可以从隔离页提交。 默认值为 `true`。 可选，用于创建。  |
| isReportToCustomizedEmailAddressEnabled  | Boolean | 指示是否应将最终用户报告的电子邮件发送到使用 customizedReportRecipientEmailAddress 配置的自定义邮箱。  默认值为 `false`。 可选，用于创建。              |
| isReportToMicrosoftEnabled               | Boolean | 如果启用，电子邮件将发送到 Microsoft 进行分析。 默认值为 `false`。 创建所必需。  |
| isReviewEmailNotificationEnabled         | Boolean | 指示是否向最终用户发送电子邮件通知，该用户在管理员审阅电子邮件后报告电子邮件。默认值为 `false`. 可选，用于创建。  |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.emailThreatSubmissionPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.emailThreatSubmissionPolicy",
  "id": "String (identifier)",
  "isReportToMicrosoftEnabled": "Boolean",
  "isReportToCustomizedEmailAddressEnabled": "Boolean",
  "isAskMeEnabledForUsers": "Boolean",
  "isAlwaysReportEnabledForUsers": "Boolean",
  "isNeverReportEnabledForUsers": "Boolean",
  "isCustomizedMessageEnabledForPhishing": "Boolean",
  "isCustomizedMessageEnabled": "Boolean",
  "customizedReportRecipientEmailAddress": "String",
  "isReviewEmailNotificationEnabled": "Boolean",
  "isCustomizedNotificationSenderEnabled": "Boolean",
  "isOrganizationBrandingEnabled": "Boolean",
  "customizedNotificationSenderEmailAddress": "String",
  "isReportFromQuarantineEnabled": "Boolean"
}
```

