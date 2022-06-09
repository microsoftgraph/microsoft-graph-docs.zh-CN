---
title: archivedPrintJob 资源类型
description: 用于报告目的 (已完成、中止或失败的) 打印作业的“最终状态”记录。 这不是活动打印作业。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 90e694b0a6bd4019fd75f871b03bcc34d999df3a
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971383"
---
# <a name="archivedprintjob-resource-type"></a>archivedPrintJob 资源类型

命名空间：microsoft.graph

用于报告目的 (已完成、中止或失败的) 打印作业的“最终状态”记录。 这不是活动打印作业。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|字符串|存档的打印作业的 GUID。 只读。|
|printerId|String|作业排队的打印机 ID。 只读。|
|processingState|printJobProcessingState|打印作业的最终处理状态。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的 dateTimeOffset。 只读。|
|acquiredDateTime|DateTimeOffset|打印机获取作业时的 dateTimeOffset（如果有）。 只读。|
|completionDateTime|DateTimeOffset|作业完成、取消或中止时的 dateTimeOffset。 只读。|
|acquiredByPrinter|布尔值|如此 如果作业是由打印机获取的;否则为 false。 只读。|
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
