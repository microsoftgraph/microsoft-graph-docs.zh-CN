---
author: daspek
description: CommentAction 资源提供有关对某个项所做的注释活动的信息。
ms.date: 09/14/2017
title: CommentAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 984e9777c31fb1ce6b6b748b9ffb0cdfe9b6446a
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944145"
---
# <a name="commentaction-resource-type"></a>CommentAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**CommentAction** 资源提供有关对某个项所做的注释 [活动][]的信息。

[活动]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>属性

| 属性     | 类型                       | 说明                                                       |
| :----------- | :------------------------- | :---------------------------------------------------------------- |
| isReply      | boolean                    | 如果为 true，此活动是对现有注释线程的回复。 |
| parentAuthor | [identitySet][]            | 启动注释线程的用户的标识。          |
| participants | [identitySet][] 集合 | 参与此注释线程的用户的标识。 |

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
