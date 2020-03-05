---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f77bc80a5723e3e00675aeaab05f2dd7ea180f76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519937"
---
# <a name="teammembersettings-resource-type"></a>teamMemberSettings 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于配置成员是否可以在[团队](team.md)中执行某些操作（例如，创建频道和添加 bot）的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|布尔|如果设置为 true，则成员可以添加和更新任何频道。|
|allowCreatePrivateChannels|布尔|如果设置为 true，则成员可以添加和更新专用通道。|
|allowDeleteChannels|布尔|如果设置为 true，则成员可以删除频道。|
|allowAddRemoveApps|布尔|如果设置为 true，则成员可以添加和删除应用。|
|allowCreateUpdateRemoveTabs|布尔|如果设置为 true，则成员可以添加、更新和删除选项卡。 |
|allowCreateUpdateRemoveConnectors|布尔|如果设置为 true，则成员可以添加、更新和删除连接器。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowCreatePrivateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
