---
title: archivedPrintJob 资源类型
description: "\"最终状态\"记录 (用于报告目的) 打印作业已完成、中止或失败。 这不是活动的打印作业。"
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2132b5a7cdf5024fb13845c57844220594ba6e1f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517213"
---
# <a name="archivedprintjob-resource-type"></a>archivedPrintJob 资源类型

命名空间：microsoft.graph

"最终状态"记录 (用于报告目的) 打印作业已完成、中止或失败。 这不是活动的打印作业。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|已存档打印作业的 GUID。 只读。|
|printerId|String|作业排队的打印机 ID。 只读。|
|processingState|printJobProcessingState|打印作业的最终处理状态。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的日期时间Offset。 只读。|
|acquiredDateTime|DateTimeOffset|打印机获取作业的日期时间Offset（如果有）。 只读。|
|completionDateTime|DateTimeOffset|作业完成、取消或中止时的日期时间Offset。 只读。|
|acquiredByPrinter|Boolean|如此 如果打印机获取作业;否则为 false。 只读。|
|copiesPrinted|Int32|打印的副本数。 只读。|
|createdBy|[userIdentity](useridentity.md)|创建打印作业的用户。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->
```json
    {   
  "@odata.type": "#microsoft.graph.archivedPrintJob",   
  "id": "String (identifier)",  
  "printerId": "String",    
  "processingState": "String",  
  "createdDateTime": "String (timestamp)",  
  "acquiredDateTime": "String (timestamp)", 
  "completionDateTime": "String (timestamp)",   
  "acquiredByPrinter": "Boolean",   
  "copiesPrinted": "Integer",   
  "createdBy": {    
    "@odata.type": "microsoft.graph.userIdentity"   
  } 
}
```