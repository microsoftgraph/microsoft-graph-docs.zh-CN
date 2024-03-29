---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 215efff423e417d83f2416021b877c8d0c08897e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049492"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings 资源类型

命名空间：microsoft.graph



设置配置成员是否可以在团队中执行某些操作，例如，创建频道和添加[机器人](team.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowCreatePrivateChannels|布尔值|如果设置为 true，成员可以添加和更新私人频道。|
|allowCreateUpdateChannels|布尔值|如果设置为 true，成员可以添加和更新频道。|
|allowDeleteChannels|Boolean|如果设置为 true，成员可以删除频道。|
|allowAddRemoveApps|Boolean|如果设置为 true，成员可以添加和删除应用。|
|allowCreateUpdateRemoveTabs|Boolean|如果设置为 true，成员可以添加、更新和删除选项卡。 |
|allowCreateUpdateRemoveConnectors|Boolean|如果设置为 true，成员可以添加、更新和删除连接器。|

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

