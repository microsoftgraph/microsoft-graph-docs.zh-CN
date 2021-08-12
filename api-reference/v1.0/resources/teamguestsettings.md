---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b8c0a47135af606d2bfb83d190bd88d6af4ad65356c99096563f76053f9a9ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146354"
---
# <a name="teamguestsettings-resource-type"></a>teamGuestSettings 资源类型

命名空间：microsoft.graph



设置配置来宾是否可以在团队中创建、更新或删除[频道](team.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|如果设置为 true，则来宾可以添加和更新频道。|
|allowDeleteChannels|Boolean|如果设置为 true，则来宾可以删除频道。|

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

