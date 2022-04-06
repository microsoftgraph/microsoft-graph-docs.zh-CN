---
title: caseOperation 资源类型
description: 表示长时间运行电子数据展示过程的抽象实体。
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6ac5cdfefb33fea8edc4eff92ef8c0b808092de6
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608126"
---
# <a name="caseoperation-resource-type"></a>caseOperation 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行电子数据展示过程的抽象实体。 它包含一组在继承实体之间共享的常见属性。  派生自 **caseOperation 的实体** 包括：

- [caseExportOperation](../resources/ediscovery-caseexportoperation.md)
- [tagOperation](../resources/ediscovery-tagoperation.md)
- [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| 操作表示的操作类型。 可能的值是： `addToReviewSet`、`applyTags`、`contentExport`、`convertToPdf`、`estimateStatistics`、 `purgeData`|
|completedDateTime|DateTimeOffset| 操作完成的日期和时间。 |
|createdBy|[identitySet](../resources/identityset.md)| 创建操作的用户。 |
|createdDateTime|DateTimeOffset| 创建该操作的日期和时间。 |
|id|String| 操作 ID。 只读。 |
|percentProgress|Int32| 操作的进度。 |
|resultInfo|[resultInfo](../resources/resultinfo.md)| 包含特定于成功和失败的结果信息。 |
|状态|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| 案例操作的状态。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|

### <a name="caseaction-values"></a>caseAction 值

|成员|说明|
|:----|-----------|
| addToReviewSet | 此操作表示从电子数据展示集合向审阅集添加数据。 |
| applyTags | 此操作表示为指定的审阅集查询在审阅集内批量标记文档。 |
| contentExport | 操作表示从审阅集导出的内容。 |
| convertToPdf | 此操作表示使用修订将文档转换为 PDF。 |
| estimateStatistics  | 此操作表示针对 Microsoft 365 服务（如 Exchange、SharePoint 和 OneDrive for business）进行搜索。 |
| purgeData | 此操作表示清除源工作负荷中的内容。 |

### <a name="caseoperationstatus-values"></a>caseOperationStatus 值

|成员|说明|
|:----|-----------|
| notStarted | 操作尚未开始。 |
| submissionFailed | 操作提交失败。 |
| running | 操作当前正在运行。 |
| succeeded | 操作成功完成，没有任何错误。 |
| partiallySucceeded | 操作已完成，但出现错误 - 有关错误详细信息， [请参阅 resultInfo](../resources/resultinfo.md) 。 |
| failed | 操作失败 - 有关错误详细信息，请参阅结果信息。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
