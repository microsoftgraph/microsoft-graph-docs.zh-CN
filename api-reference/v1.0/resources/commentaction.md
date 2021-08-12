---
author: daspek
title: commentAction 资源类型
description: commentAction 对象提供有关对项目进行注释的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bd146a400e83692754e1ca920dcba97339c1634f8fe81cc37374a6e37a30a872
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135279"
---
# <a name="commentaction-resource-type"></a>commentAction 资源类型

命名空间：microsoft.graph

**commentAction** 资源提供有关对项目 [进行注释活动][]的信息。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

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
  "@type&quot;: &quot;microsoft.graph.commentAction"
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

