---
author: daspek
ms.author: dspektor
title: mentionAction 资源类型
description: MentionAction 对象提供有关在活动过程中提及的内容的信息。
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: de6bf1657e9b9ba21d589a6ef27292553bf93f7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534247"
---
# <a name="mentionaction-resource-type"></a>mentionAction 资源类型

命名空间：microsoft.graph

**MentionAction** 资源提供了有关提到人员的[活动][]的信息。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[活动]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型                       | 说明
|:--------------|:---------------------------|:-----------------------------
| mentionees    | [identitySet][] 集合 | 此操作提及的用户的标识。

[identitySet]: identityset.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->
