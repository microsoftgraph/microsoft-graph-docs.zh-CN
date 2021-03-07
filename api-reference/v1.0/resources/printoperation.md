---
title: printOperation 资源类型
description: 代表长时间运行的通用打印操作。 操作类型（如 printerCreateOperation）的基类。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a397a0166ad62a503027499e9e0f5fd4f127b1e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517290"
---
# <a name="printoperation-resource-type"></a>printOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

代表长时间运行的通用打印操作。 操作类型（如 [printerCreateOperation）的基类](printercreateoperation.md)。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [获取操作](../api/printoperation-get.md) | [printOperation](printoperation.md) | 在当前用户或应用的租户中检索长时间运行的操作。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|操作标识符。 只读。|
|状态|[printOperationStatus](printoperationstatus.md)|操作的状态。 只读。|
|createdDateTime|DateTimeOffset|创建操作时的日期时间Offset。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

