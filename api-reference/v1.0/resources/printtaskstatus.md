---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d0222192b8c4e7a9fe644edbd956a98a5ad899a7
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60946865"
---
# <a name="printtaskstatus-resource-type"></a>printTaskStatus 资源类型

命名空间：microsoft.graph

表示 [printTask 的当前执行状态](printtask.md)。 

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|state|printTaskProcessingState|[printTask 的当前处理状态](printtask.md)。 下表介绍了有效值。|
|description|String|可读的 [printTask](printtask.md)当前处理状态的说明。|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|pending|0|任务执行挂起。|
|processing|1|任务执行正在进行中。|
|已完成|2|任务执行已完成。|
|aborted|3|任务执行已中止。|
|unknownFutureValue|4|可发展枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

