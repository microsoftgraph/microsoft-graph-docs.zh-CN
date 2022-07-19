---
title: threatSubmission 资源类型
description: 表示威胁提交，用于向 Microsoft Defender 提交可疑的电子邮件、UTL 或文件威胁。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23651a4b66c68ce1c8d128268dd786dfcf667cf8
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856632"
---
# <a name="threatsubmission-resource-type"></a>threatSubmission 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示威胁提交，它是一种抽象类型，用于表示可疑的垃圾邮件、恶意软件、网络钓鱼和被阻止的合法电子邮件;恶意软件、网络钓鱼和阻止的合法 URL;网络钓鱼、恶意软件和阻止Microsoft Defender for Office 365的合法电子邮件附件，以及要Microsoft Defender for Endpoint的可疑文件。

此资源还可用于提交不应被Microsoft Defender for Office 365阻止的误报案例;例如，不是垃圾邮件、安全 URL 和安全电子邮件附件。

这是一种抽象类型。 继承自 [entity](../resources/entity.md)。 [emailThreatSubmission](../resources/security-emailthreatsubmission.md)、[urlThreatSubmission](../resources/security-urlthreatsubmission.md)、[fileThreatSubmissin](../resources/security-filethreatsubmission.md) 的基本类型。

## <a name="properties"></a>属性
| 属性        | 类型                       | Description                                                                      |
|:----------------|:---------------------------|:---------------------------------------------------------------------------------|
| adminReview     | [security.submissionAdminReview](../resources/security-submissionadminreview.md)| 指定管理员评审属性，该属性由谁审阅了用户提交、何时以及标识为何种内容组成。 |
| “类别”        | submissionCategory         | 指定提交类别。 支持 `$filter = category eq 'value'`。 可能的值是：`notJunk`、`spam`、`phishing``malware`和 `unkownFutureValue`。|
| clientSource    | submissionClientSource     | 指定提交源。 可能的值为： `microsoft`和  `other` `unkownFutureValue`. |
| contentType     | submissionContentType      | 指定要提交的内容类型。 可能的值是：`email`、`url`、`file``app`和 `unkownFutureValue`。  |
| createdBy       | [security.submissionUserIdentity](../resources/security-submissionuseridentity.md)     | 指定将电子邮件提交为威胁的人员。 支持 `$filter = createdBy/email eq 'value'`。 |
| createdDateTime | DateTimeOffset  | 指定何时创建威胁提交。 支持 `$filter = createdDateTime ge 2022-01-01T00:00:00Z and createdDateTime lt 2022-01-02T00:00:00Z`。             |
| id              | String                     | 指定威胁提交 ID。 |
| result          | [security.submissionResult](../resources/security-submissionresult.md)          | 指定 Microsoft 执行的分析结果。  |
| source          | submissionSource           | 指定提交者的角色。 支持 `$filter = source eq 'value'`。 可能的值为： `administrator`和  `user` `unkownFutureValue`.  |
| status          | longRunningOperationStatus | 指示是否已由 Microsoft 分析威胁提交。 支持 `$filter = status eq 'value'`。 可能的值是：`notStarted`、`running`、`succeeded`、`failed``skipped`和 `unkownFutureValue`。 |
| tenantId        | String                     | 指示提交程序的租户 ID。 使用 `POST` 操作创建时不需要。 它从后 API 调用的令牌中提取。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.threatSubmission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.threatSubmission",
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
  "clientSource": "String"
}
```

