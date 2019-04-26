---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: c472a0b1b992c91b60174859e4900ffcee04c007
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341456"
---
# <a name="commentaction-resource-type"></a>CommentAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**CommentAction** 资源提供有关对某个项所做的注释[活动][]的信息。

[活动]: itemactivity.md

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

## <a name="properties"></a>属性

| 属性名称    | 类型                       | 说明
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | 如果为 true，此活动是对现有注释线程的回复。
| parentAuthor     | [identitySet][]            | 启动注释线程的用户的标识。
| participants     | [identitySet][] 集合 | 参与此注释线程的用户的标识。

[identitySet]: identityset.md

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->
