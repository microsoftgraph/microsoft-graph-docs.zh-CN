---
title: printServiceEndpoint 资源类型
description: 表示打印服务实例的 URI 和标识信息。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7534e538c81c543671d996c7765125eafcad9d67cddbb13ad406d06edb8b9912
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178036"
---
# <a name="printserviceendpoint-resource-type"></a>printServiceEndpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印服务实例的 URI 和标识信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
| [Get endpoint](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | 读取 endpoint 对象的属性和关系。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|终结点的可读显示名称。|
|id|String|标识终结点提供的服务的唯一名称。 可能的值包括 `discovery` ： (Discovery Service) 、 (`notification` Notification Service) 、 (IPP Service) 和 `ipp` (Registration Service `registration`) 。 只读。|
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

