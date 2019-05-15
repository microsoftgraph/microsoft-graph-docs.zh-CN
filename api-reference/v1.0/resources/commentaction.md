---
author: daspek
ms.author: dspektor
title: commentAction 资源类型
description: CommentAction 对象提供有关对项目所做的注释的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 12e6cd68d5809b8e4c1765234eeb77b40b30a78e
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970629"
---
# <a name="commentaction-resource-type"></a>commentAction 资源类型

**CommentAction**资源提供有关对项目进行的注释[活动][]的信息。

>**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

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
