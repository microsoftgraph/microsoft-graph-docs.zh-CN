---
title: assignedLabel 资源类型
description: 表示分配给组或组的Microsoft 365标签。 敏感度标签允许管理员通过向组分配分类（如"机密 (高度机密"或"常规"策略）对组强制执行特定) 。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b54236376979d064a86eb1e4852919e2b5ff9e49
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680456"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示分配给组或组的Microsoft 365标签。 敏感度标签允许管理员通过向组分配分类（如"机密 (高度机密"或"常规"策略）对组强制执行特定) 。 敏感度标签由 Microsoft 信息保护Microsoft 365安全&中心中的管理员发布。 有关敏感度标签详细信息，请参阅敏感度 [标签概述](/Office365/SecurityCompliance/sensitivity-labels)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|labelId|String|标签的唯一标识符。|
|displayName|String|标签显示名称。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


