---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c1485bbc43588b8144cbe1cc7cb189f9b8c9fdc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863776"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings 资源类型



用于配置成员是否可以在[团队](team.md)中执行某些操作（例如，创建频道和添加 bot）的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowCreatePrivateChannels|Boolean|如果设置为 true，则成员可以添加和更新专用通道。|
|allowCreateUpdateChannels|Boolean|如果设置为 true，则成员可以添加和更新频道。|
|allowDeleteChannels|Boolean|如果设置为 true，则成员可以删除频道。|
|allowAddRemoveApps|Boolean|如果设置为 true，则成员可以添加和删除应用。|
|allowCreateUpdateRemoveTabs|Boolean|如果设置为 true，则成员可以添加、更新和删除选项卡。 |
|allowCreateUpdateRemoveConnectors|Boolean|如果设置为 true，则成员可以添加、更新和删除连接器。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreatePrivateChannels": true,
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
