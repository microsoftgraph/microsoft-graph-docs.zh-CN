---
title: printService 资源类型
description: 表示打印服务实例Azure AD特定于租户的说明。 打印基础结构 (的每个组件都存在服务，例如发现、通知、注册和 IPP) ，并且有一个或多个终结点。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: df904704f6efb9d069832a6b9767ab1314e261ee
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176758"
---
# <a name="printservice-resource-type"></a>printService 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印服务实例Azure AD特定于租户的说明。 打印基础结构 (发现、通知、注册和 IPP) 的每个组件都存在服务，并且有一个或多个终结点。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [列出服务](../api/print-list-services.md) | [printService](printservice.md) 集合 | 获取通用打印服务的列表。 |
| [获取服务](../api/printservice-get.md) | [printService](printservice.md) | 读取服务对象的属性和关系。 |
| [List endpoints](../api/printservice-list-endpoints.md) | [printServiceEndpoint](printserviceendpoint.md) 集合 | 获取服务提供的终结点列表。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|服务的标识符。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | Description |
|:-------------|:------------|:------------|
|endpoints|[printServiceEndpoint](printserviceendpoint.md) 集合| 可用于访问服务的终结点。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printService",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "endpoints": [ {"@odata.type": "microsoft.graph.printServiceEndpoint"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

