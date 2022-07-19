---
title: emailThreatSubmission 资源类型
description: 向Microsoft Defender for Office 365报告可疑的垃圾邮件、恶意软件或网络钓鱼电子邮件。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 387d4531a6f2e4d4b9184e4006ae43ddac4c15ed
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856639"
---
# <a name="emailthreatsubmission-resource-type"></a>emailThreatSubmission 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于向Microsoft Defender for Office 365报告可疑垃圾邮件、恶意软件或网络钓鱼电子邮件的抽象类型。 还可以提交不应被Microsoft Defender for Office 365阻止的误报案例，例如，错误地将电子邮件分类为垃圾邮件或垃圾邮件。

继承自 [threatSubmission](../resources/security-threatsubmission.md)。 [emailContentThreatSubmission](../resources/security-emailcontentthreatsubmission.md) 和 [emailUrlThreatSubmission](../resources/security-emailurlthreatsubmission.md) 的基本类型。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 emailThreatSubmissions](../api/security-emailthreatsubmission-list.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md) 集合|获取 [emailThreatSubmission](../resources/security-emailthreatsubmission.md) 对象及其属性的列表。|
|[创建 emailThreatSubmission](../api/security-emailthreatsubmission-post-emailthreats.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|创建新的 [emailThreatSubmission](../resources/security-emailthreatsubmission.md) 对象。|
|[获取 emailThreatSubmission](../api/security-emailthreatsubmission-get.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|读取 [emailThreatSubmission](../resources/security-emailthreatsubmission.md) 对象的属性和关系。|
|[检讨](../api/security-emailthreatsubmission-review.md)|无|由管理员查看来自最终用户的威胁提交。|

## <a name="properties"></a>属性
| 属性     | 类型    | Description    |
|:-----------------------------|:-----------------------------|:-------------------------------------------------------------------------------------------------------|
| attackSimulationInfo         | [security.attackSimulationInfo](../resources/security-attacksimulationinfo.md) | 如果电子邮件是网络钓鱼模拟，则此字段不会为 null。|
| internetMessageId            | String                       | 指定要提交的电子邮件的 Internet 消息 ID。 此信息存在于电子邮件标头中。 |
| originalCategory             | submissionCategory           | 提交的原始类别。 可能的值是：`notJunk`、`spam`、`phishing``malware`和 `unkownFutureValue`。 |
| receivedDateTime             | DateTimeOffset               | 指定收到电子邮件时的日期和时间戳。  | 
| recipientEmailAddress        | String                       | 指定接收电子邮件的收件人) 以 smtp 格式 (的电子邮件地址。 |
| sender                       | String                       | 指定发件人的电子邮件地址。 | 
| senderIP                     | String                       | 指定发件人 IP 地址。 |
| subject                      | String                       | 指定电子邮件的主题。 |
| tenantAllowOrBlockListAction | [security.tenantAllowOrBlockListAction](../resources/security-tenantalloworblocklistaction.md) | 它用于自动添加允许的组件，如 URL、文件、发件人;Microsoft 认为这些消息不好，因此将来可以允许类似的消息。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.emailThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.emailThreatSubmission",
  "id": "String (identifier)",
  "tenantId": "String",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "category": "String",
  "source": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.security.submissionUserIdentity"
  },
  "status": "String",
  "result": {
    "@odata.type": "microsoft.graph.security.submissionResult"
  },
  "adminReview": {
    "@odata.type": "microsoft.graph.security.submissionAdminReview"
  },
  "clientSource": "String",
  "recipientEmailAddress": "String",
  "internetMessageId": "String",
  "subject": "String",
  "sender": "String",
  "senderIP": "String",
  "receivedDateTime": "String (timestamp)",
  "originalCategory": "String",
  "attackSimulationInfo": {
    "@odata.type": "microsoft.graph.security.attackSimulationInfo"
  },
  "tenantAllowOrBlockListAction": {
    "@odata.type": "microsoft.graph.security.tenantAllowOrBlockListAction"
  }
}
```

