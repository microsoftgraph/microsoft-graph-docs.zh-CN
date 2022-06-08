---
title: caseOperation 资源类型
description: 表示长时间运行的进程的抽象实体。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 84ea673ad768042ff79f5db0a41fe1d1a4af3e3a
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945330"
---
# <a name="caseoperation-resource-type"></a>caseOperation 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

继承自 [entity](../resources/entity.md)。

表示长时间运行的电子数据展示过程的抽象实体。 它包含在继承实体之间共享的一组常见属性。  派生自 **caseOperation 的** 实体包括：

- [索引操作](../resources/security-ediscoveryindexoperation.md)
- [保留操作](../resources/security-ediscoveryholdoperation.md)
- [清除数据操作](../resources/security-ediscoverypurgedataoperation.md)
- [估算操作](../resources/security-ediscoveryestimateoperation.md)
- [添加到审阅集操作](../resources/security-ediscoveryaddtoreviewsetoperation.md)
- [标记操作](../resources/security-ediscoverytagoperation.md)
- [导出操作](../resources/security-ediscoveryexportoperation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List caseOperations](../api/security-ediscoverycase-list-operations.md)|[microsoft.graph.security.caseOperation](../resources/security-caseoperation.md) 集合|获取 [caseOperation](../resources/security-caseoperation.md) 对象及其属性的列表。|
|[获取 caseOperation](../api/security-caseoperation-get.md)|[microsoft.graph.security.caseOperation](../resources/security-caseoperation.md)|读取 [caseOperation](../resources/security-caseoperation.md) 对象的属性和关系。|

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

### <a name="caseaction-values"></a>caseAction 值

|成员|说明|
|:----|-----------|
| addToReviewSet | 该操作表示从电子数据展示集合向审阅集添加数据。 |
| applyTags | 该操作表示指定审阅集查询的审阅集中批量标记文档。 |
| contentExport | 该操作表示从审阅集导出的内容。 |
| convertToPdf | 该操作表示使用修订将文档转换为 PDF。 |
| estimateStatistics  | 该操作表示针对 Microsoft 365 服务（如 Exchange、SharePoint 和 OneDrive for Business）进行搜索。 |
| holdUpdate | 该操作表示更新法定保留 (为保管人和非保管数据源应用/删除) 。
| index | 该操作表示为保管人和非保管数据源的数据源编制索引，使其可搜索。 |
| purgeData | 该操作表示从源工作负荷中清除内容。 |

### <a name="caseoperationstatus-values"></a>caseOperationStatus 值

|成员|说明|
|:----|-----------|
| notStarted | 操作尚未启动。 |
| submissionFailed | 操作提交失败。 |
| 运行 | 此操作当前正在运行。 |
| 成功 | 操作已成功完成，没有任何错误。 |
| partiallySucceeded | 操作已完成，但存在错误 - 有关错误详细信息，请参阅 [resultInfo](../resources/resultinfo.md) 。 |
| 失败 | 操作失败 - 有关错误详细信息，请参阅结果信息。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.caseOperation",
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