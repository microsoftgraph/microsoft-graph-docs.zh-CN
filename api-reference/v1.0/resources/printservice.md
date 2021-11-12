---
title: printService 资源类型
description: 表示Azure AD服务实例的租户特定说明。 打印基础结构的每个组件都有服务 (例如发现、通知、注册和 IPP) 具有一个或多个终结点。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7319ee78846f98f0d41faab9deecff6bc2b1830b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936955"
---
# <a name="printservice-resource-type"></a>printService 资源类型

命名空间：microsoft.graph

表示Azure AD服务实例的租户特定说明。 打印基础结构的每个组件都有服务 (发现、通知、注册和 IPP) 具有一个或多个终结点。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [列出服务](../api/print-list-services.md) | [printService](printservice.md) 集合 | 获取通用打印服务的列表。 |
| [获取服务](../api/printservice-get.md) | [printService](printservice.md) | 读取服务对象的属性和关系。 |
| [List endpoints](../api/printservice-list-endpoints.md) | [printServiceEndpoint](printserviceendpoint.md) 集合 | 获取服务提供的终结点列表。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|服务的标识符。 只读。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|endpoints|[printServiceEndpoint](printserviceendpoint.md) 集合| 可用于访问服务的终结点。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

