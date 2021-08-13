---
author: daspek
title: shareAction 资源类型
description: shareAction 对象提供有关共享操作中项目共享对象的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b9d252df884e90d7351edb9544a354d88fbc78baebcc5926686b016c38e58f37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251776"
---
# <a name="shareaction-resource-type"></a>shareAction 资源类型

命名空间：microsoft.graph

**shareAction** 资源提供有关 [共享项的活动][activity]的信息。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型                       | 说明
|:--------------|:---------------------------|:-----------------------------
| recipients    | [identitySet][] 集合 | 项在此操作中共享的标识。

[identitySet]: identityset.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->

