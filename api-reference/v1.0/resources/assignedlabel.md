---
title: assignedLabel 资源类型
description: 表示分配给 Microsoft 365 组的敏感度标签。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: bcc89583a1611093c58f4cd7cbe2ec6907820945
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883948"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel 资源类型

命名空间：microsoft.graph

表示分配给 Microsoft 365 组的敏感度标签。 敏感度标签允许管理员通过将分类分配给组 (（如机密、高度机密或常规) ）对组强制实施特定的组设置。 敏感度标签由 Microsoft 365 安全&合规中心的管理员发布，作为 Microsoft Purview 信息保护功能的一部分。 有关敏感度标签的详细信息，请参阅 [敏感度标签概述](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)。

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                               |
| :---------- | :----- | :---------------------------------------- |
| labelId     | String | 标签的唯一标识符。       |
| displayName | String | 标签的显示名称。 只读。 |

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
