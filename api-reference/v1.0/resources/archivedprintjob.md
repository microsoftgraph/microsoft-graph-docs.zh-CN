---
title: archivedPrintJob 资源类型
description: 用于报告目的的 (打印作业) 完成、中止或失败的"最终状态"记录。 这不是活动的打印作业。
author: nilakhan
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9f6818801a12eb635a86350432108d3d0e3b6332
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109519"
---
# <a name="archivedprintjob-resource-type"></a>archivedPrintJob 资源类型

命名空间：microsoft.graph

用于报告目的的 (打印作业) 完成、中止或失败的"最终状态"记录。 这不是活动的打印作业。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|已存档打印作业的 GUID。 只读。|
|printerId|String|作业已排队的打印机 ID。 只读。|
|processingState|printJobProcessingState|打印作业的最终处理状态。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的日期时间Offset。 只读。|
|acquiredDateTime|DateTimeOffset|打印机获取作业的 dateTimeOffset（如果有）。 只读。|
|completionDateTime|DateTimeOffset|作业完成、取消或中止的 dateTimeOffset。 只读。|
|acquiredByPrinter|布尔值|如此 如果打印机获取作业;否则为 false。 只读。|
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
