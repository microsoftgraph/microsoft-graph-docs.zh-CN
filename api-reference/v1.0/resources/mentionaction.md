---
author: daspek
title: mentionAction 资源类型
description: MentionAction 对象提供有关在活动期间被提及者的信息。
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bdcef79492604aa5ee2afae0897361eb41dd6889229b4b41259cc3d47f72bf92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152381"
---
# <a name="mentionaction-resource-type"></a>mentionAction 资源类型

命名空间：microsoft.graph

**MentionAction** 资源提供了有关提到人员的 [活动][]的信息。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

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
  "@type&quot;: &quot;microsoft.graph.mentionAction"
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

