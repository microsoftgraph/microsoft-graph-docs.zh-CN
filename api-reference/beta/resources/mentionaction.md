---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.openlocfilehash: 7843feebd8ebca2022b276007d21a89b754217a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804968"
---
# <a name="mentionaction-resource-type"></a>MentionAction 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**MentionAction** 资源提供了有关提到人员的[活动][]的信息。

[活动]: itemactivity.md

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

## <a name="properties"></a>属性

| 属性名称 | 类型                       | 说明
|:--------------|:---------------------------|:-----------------------------
| mentionees    | [identitySet][] 集合 | 此操作提及的用户的标识。

[identitySet]: identityset.md

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
