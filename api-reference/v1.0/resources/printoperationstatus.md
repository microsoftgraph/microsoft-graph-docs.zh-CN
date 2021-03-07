---
title: printOperationStatus 资源类型
description: 表示长时间运行的通用打印操作的当前状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 787a584b32c6f34d78d14fa4d676b1be30a62c25
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516991"
---
# <a name="printoperationstatus-resource-type"></a>printOperationStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示长时间运行的通用打印操作的当前状态。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|state|printOperationProcessingState|printOperation 的当前处理状态。 下表介绍了有效值。 只读。|
|说明|String|可读的 printOperation 当前处理状态的说明。 只读。|

### <a name="printoperationprocessingstate-values"></a>printOperationProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|notStarted|0|操作尚未启动。|
|正在运行|1 |操作正在运行。|
|succeeded|2 |操作成功完成。|
|failed|3 |操作失败。|
|unknownFutureValue|4 |可发展枚举 sentinel 值。 请勿使用。|

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

