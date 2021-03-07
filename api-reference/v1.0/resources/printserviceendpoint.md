---
title: printServiceEndpoint 资源类型
description: 表示打印服务实例的 URI 和标识信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0dd339d433be593e6982b6c38818635830a2d471
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516988"
---
# <a name="printserviceendpoint-resource-type"></a>printServiceEndpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印服务实例的 URI 和标识信息。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [Get endpoint](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | 读取 endpoint 对象的属性和关系。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|终结点的可读显示名称。|
|id|String|标识终结点提供的服务的唯一名称。 可能的值包括 `discovery` ： (发现服务) 、 (通知服务 `notification`) 、 (IPP 服务) 和 `ipp` (`registration` 注册服务) 。 只读。|
|uri|String|可用于访问服务的 URI。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```

