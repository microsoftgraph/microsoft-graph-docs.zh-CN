---
title: printService 资源类型
description: 表示对打印服务实例的特定于 Azure AD 租户的说明。 打印基础结构的每个组件都有服务 (例如，发现、通知、注册和 IPP) 并具有一个或多个终结点。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 00ba50369f2396250df632c13ed3945e8c9d40d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052537"
---
# <a name="printservice-resource-type"></a>printService 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对打印服务实例的特定于 Azure AD 租户的说明。 打印基础结构的每个组件都存在的服务 (发现、通知、注册和 IPP) 并具有一个或多个终结点。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出服务](../api/print-list-services.md) | [printService](printservice.md) 集合 | 获取通用打印服务的列表。 |
| [获取服务](../api/printservice-get.md) | [printService](printservice.md) | 读取服务对象的属性和关系。 |
| [List endpoints](../api/printservice-list-endpoints.md) | [printServiceEndpoint](printserviceendpoint.md) 集合 | 获取服务提供的终结点列表。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|服务的标识符。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
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

