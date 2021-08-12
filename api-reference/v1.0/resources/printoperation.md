---
title: printOperation 资源类型
description: 代表长时间运行的通用打印操作。 操作类型（如 printerCreateOperation）的基类。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0630d05e30d415ad60f4dd7ea4e7f729506e41b2cc20bded955e1593a6f56161
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138456"
---
# <a name="printoperation-resource-type"></a>printOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

代表长时间运行的通用打印操作。 操作类型的基类，如 [printerCreateOperation](printercreateoperation.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
| [获取操作](../api/printoperation-get.md) | [printOperation](printoperation.md) | 在当前用户或应用的租户中检索长时间运行的操作。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|操作标识符。 只读。|
|status|[printOperationStatus](printoperationstatus.md)|操作的状态。 只读。|
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

