---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7c5cc116567b0ee2db1b2dd5e28c4749d7c6772c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033864"
---
# <a name="teamguestsettings-resource-type"></a>teamGuestSettings 资源类型



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
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
