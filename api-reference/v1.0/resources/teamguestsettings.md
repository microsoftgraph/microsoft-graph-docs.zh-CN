---
title: teamGuestSettings 资源类型
description: 要配置的是否来宾可以创建、 更新或删除通道团队中的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924368"
---
# <a name="teamguestsettings-resource-type"></a>teamGuestSettings 资源类型



要配置的是否来宾可以创建、 更新或删除通道[团队](team.md)中的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|布尔|如果设置为 true，则来宾可以添加和更新通道。|
|allowDeleteChannels|布尔|如果设置为 true，则来宾可以删除通道。|

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
