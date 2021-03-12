---
title: assignedLabel 资源类型
description: 表示分配给 Microsoft 365 组的敏感度标签。
localization_priority: Normal
author: jpettere
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 9602e10dda5d558110c55f1fb4ee166e53187989
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720891"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel 资源类型

命名空间：microsoft.graph

表示分配给 Microsoft 365 组的敏感度标签。 敏感度标签允许管理员通过向组分配分类（如"机密 (高度机密"或"常规"策略）对组强制执行特定) 。 敏感度标签由 Microsoft 365 安全与合规& Microsoft 信息保护功能的一部分发布。 有关敏感度标签详细信息，请参阅敏感度 [标签概述](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|labelId|字符串|标签的唯一标识符。|
|displayName|字符串|标签显示名称。 只读。|

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