---
author: daspek
description: ShareAction 资源提供了有关共享项的活动的信息。
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 10eb5b870a5ecd80f4a064d1dca496f216bf241d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965164"
---
# <a name="shareaction-resource-type"></a>ShareAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ShareAction** 资源提供了有关共享项的[活动][activity]的信息。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型                       | 说明
|:--------------|:---------------------------|:-----------------------------
| recipients    | [identitySet][] 集合 | 项在此操作中共享的标识。

[identitySet]: identityset.md

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->
