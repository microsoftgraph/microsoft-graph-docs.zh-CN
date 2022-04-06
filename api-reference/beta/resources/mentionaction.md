---
author: daspek
description: MentionAction 资源提供了有关提到人员的活动的信息。
ms.date: 09/14/2017
title: MentionAction
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4675a732738741dc5bb201f97753dca2be42a17d
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723484"
---
# <a name="mentionaction-resource-type"></a>MentionAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**MentionAction** 资源提供了有关提到人员的 [活动][]的信息。

[活动]: itemactivity.md

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

## <a name="properties"></a>属性

| 属性   | 类型                       | 说明                                           |
| :--------- | :------------------------- | :---------------------------------------------------- |
| mentionees | [identitySet][] 集合 | 此操作提及的用户的标识。 |

[identitySet]: identityset.md

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

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
