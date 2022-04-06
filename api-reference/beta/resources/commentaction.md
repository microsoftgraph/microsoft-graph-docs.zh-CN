---
author: daspek
description: CommentAction 资源提供有关对某个项所做的注释活动的信息。
ms.date: 09/14/2017
title: CommentAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 32532bf0771da739db86915091cdc8b79aa942c2
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722755"
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
