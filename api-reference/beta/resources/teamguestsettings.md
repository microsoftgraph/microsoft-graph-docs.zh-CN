---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b195590b696002d2ece9828ad8b65fb5b607765f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341702"
---
# <a name="teamguestsettings-resource-type"></a>teamGuestSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于配置来宾是否可以在[团队](team.md)中创建、更新或删除频道的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|如果设置为 true, 则来宾可以添加和更新频道。|
|allowDeleteChannels|Boolean|如果设置为 true, 则来宾可以删除频道。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
