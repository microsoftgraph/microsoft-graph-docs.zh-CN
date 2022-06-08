---
title: ediscoveryHoldOperation 资源类型
description: 表示对数据源（包括保管人和非保管数据源）应用保留的过程。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a23b2d95519e1f3f69f05c4199d3ae3b843c3a72
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945173"
---
# <a name="ediscoveryholdoperation-resource-type"></a>ediscoveryHoldOperation 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对数据源（包括保管人和非保管数据源）应用保留的过程。

继承自 [caseOperation](../resources/security-caseoperation.md)。

## <a name="methods"></a>方法

无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| 操作表示的操作类型。 可能的值为：，`addToReviewSet``applyTags`，，`contentExport``convertToPdf`，`estimateStatistics`，`purgeData`|
|completedDateTime|DateTimeOffset| 操作完成的日期和时间。 |
|createdBy|[identitySet](../resources/identityset.md)| 创建操作的用户。 |
|createdDateTime|DateTimeOffset| 创建操作的日期和时间。 |
|id|String| 操作的 ID。 只读。 |
|percentProgress|Int32| 操作的进度。 |
|resultInfo|[resultInfo](../resources/resultinfo.md)| 包含成功和失败特定的结果信息。 |
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| 事例操作的状态。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryHoldOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryHoldOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```

