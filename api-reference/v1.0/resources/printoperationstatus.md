---
title: printOperationStatus 资源类型
description: 表示长时间运行的通用打印操作的当前状态。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: dd5e7e912ea6810a4a0d501d47a8711830e91ae0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944891"
---
# <a name="printoperationstatus-resource-type"></a>printOperationStatus 资源类型

命名空间：microsoft.graph

表示长时间运行的通用打印操作的当前状态。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|state|printOperationProcessingState|printOperation 的当前处理状态。 下表介绍了有效值。 只读。|
|说明|String|可读的 printOperation 当前处理状态的说明。 只读。|

### <a name="printoperationprocessingstate-values"></a>printOperationProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|notStarted|0|操作尚未开始。|
|running|1|操作正在运行。|
|succeeded|2|操作成功完成。|
|failed|3|操作失败。|
|unknownFutureValue|4|可发展枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printOperationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperationStatus",
  "state": "String",
  "description": "String"
}
```

