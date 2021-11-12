---
title: printServiceEndpoint 资源类型
description: 表示打印服务实例的 URI 和标识信息。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 812e9367be06760e56299bd62c88c154f1c25c49
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924199"
---
# <a name="printserviceendpoint-resource-type"></a>printServiceEndpoint 资源类型

命名空间：microsoft.graph

表示打印服务实例的 URI 和标识信息。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
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

