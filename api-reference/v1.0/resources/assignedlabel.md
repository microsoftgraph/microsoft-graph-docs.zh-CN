---
title: assignedLabel 资源类型
description: 表示分配给组分配的Microsoft 365标签。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 197ea28fa330c9a91e158cd915d8fb4bb72bca3940dd1d867776424d0cbb116a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135370"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel 资源类型

命名空间：microsoft.graph

表示分配给组分配的Microsoft 365标签。 敏感度标签允许管理员通过向组分配分类（如"机密 (高度机密"或"常规"策略）对组强制执行特定) 。 敏感度标签由安全与合规Microsoft 365中心中的&发布，作为Microsoft 信息保护的一部分。 有关敏感度标签详细信息，请参阅敏感度 [标签概述](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)。

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