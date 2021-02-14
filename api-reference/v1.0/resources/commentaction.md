---
author: daspek
title: commentAction 资源类型
description: commentAction 对象提供有关对项目进行注释的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2f3ab7f0798ee1020b107c38262a912fdae53ef
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238412"
---
# <a name="commentaction-resource-type"></a>commentAction 资源类型

命名空间：microsoft.graph

**commentAction** 资源提供有关对项目进行注释 [][]活动的信息。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[活动]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称    | 类型                       | 说明
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | 如果为 true，此活动是对现有注释线程的回复。
| parentAuthor     | [identitySet][]            | 启动注释线程的用户的标识。
| participants     | [identitySet][] 集合 | 参与此注释线程的用户的标识。

[identitySet]: identityset.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->

