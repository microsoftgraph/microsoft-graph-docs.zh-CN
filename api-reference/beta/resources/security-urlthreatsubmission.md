---
title: urlThreatSubmission 资源类型
description: 表示与 URL 相关的威胁提交
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5f04e14d1482a935868f4a0a7985b43b6faf5188
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856659"
---
# <a name="urlthreatsubmission-resource-type"></a>urlThreatSubmission 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与 URL 相关的威胁提交。

此资源用于将可疑网络钓鱼 URL 提交到Microsoft Defender for Office 365。 它还可用于提交不应被阻止的误报案例，例如安全 URL。

继承自 [threatSubmission](../resources/security-threatsubmission.md)。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 urlThreatSubmissions](../api/security-urlthreatsubmission-list.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md) 集合|获取 [urlThreatSubmission](../resources/security-urlthreatsubmission.md) 对象及其属性的列表。|
|[创建 urlThreatSubmission](../api/security-urlthreatsubmission-post-urlthreats.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|创建新的 [urlThreatSubmission](../resources/security-urlthreatsubmission.md) 对象。|
|[获取 urlThreatSubmission](../api/security-urlthreatsubmission-get.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|读取 [urlThreatSubmission](../resources/security-urlthreatsubmission.md) 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性 | 类型   | 说明                 |
|:---------|:-------|:----------------------------|
| WebUrl   | String | 表示需要提交的 webUrl。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.urlThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.urlThreatSubmission",
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
  "webUrl": "String"
}
```

