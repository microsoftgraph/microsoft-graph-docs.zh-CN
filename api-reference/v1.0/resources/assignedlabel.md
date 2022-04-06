---
title: assignedLabel 资源类型
description: 表示分配给组分配的Microsoft 365标签。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a4992960d63c90efb06d3799944c9df66616759c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588321"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel 资源类型

命名空间：microsoft.graph

表示分配给组分配的Microsoft 365标签。 敏感度标签允许管理员通过向组分配分类（如"机密 (高度机密"或"常规"策略）来对组强制执行特定) 。 敏感度标签由安全与合规Microsoft 365中心中的&发布，作为Microsoft 信息保护的一部分。 有关敏感度标签详细信息，请参阅敏感度 [标签概述](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)。

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                               |
| :---------- | :----- | :---------------------------------------- |
| labelId     | String | 标签的唯一标识符。       |
| displayName | String | 标签显示名称。 只读。 |

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
