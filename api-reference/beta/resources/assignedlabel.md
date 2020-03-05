---
title: assignedLabel 资源类型
description: 代表分配给 Office 365 组的敏感度标签。 通过将分类（如机密、高度机密或常规）分配给组，允许管理员在组上强制实施特定的组设置。
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4f4f1fd854885668160b46f2b1ee9396dcf954fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508217"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表分配给 Office 365 组的敏感度标签。 通过将分类（如机密、高度机密或常规）分配给组，允许管理员在组上强制实施特定的组设置。 敏感度标签由 Microsoft 365 Security & 合规性中心中的管理员发布，作为 Microsoft 信息保护功能的一部分。 有关敏感度标签的详细信息，请参阅[敏感度标签概述](/Office365/SecurityCompliance/sensitivity-labels)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|labelId|String|标签的唯一标识符。|
|displayName|String|标签的显示名称。 只读。|

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
