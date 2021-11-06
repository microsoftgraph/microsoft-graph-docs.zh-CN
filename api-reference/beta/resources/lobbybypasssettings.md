---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议厅。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5fa0fac27d8dfaacb27572476ab49e80cb3832e
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805556"
---
# <a name="lobbybypasssettings-resource-type"></a>lobbyBypassSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定哪些参与者可以绕过会议厅。

## <a name="properties"></a>属性

| 属性              | 类型    | Description                                                         |
| --------------------- | ------- | ------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | 指定自动获准加入会议、绕过会议厅的参与者类型。 可选。|
| isDialInBypassEnabled | Boolean | 指定是否始终允许拨入呼叫者绕过大厅。 可选。 |

### <a name="lobbybypassscope-values"></a>lobbyBypassScope 值

| 值                    | Description     |
| ------------------------ | --------------------------------------------------- |
| 组织者 | 只有组织者才能参加会议并绕过会议厅。 所有其他参与者都放置在会议厅中。 |
| 组织 | 只有来自同一公司的参与者和 **来宾** 才能参加会议并绕过会议厅。 所有其他参与者都放置在会议厅中。 |
| organizationAndFederated | 只有来自同一公司或受信任组织的参与者和来宾才能参加会议并绕过会议厅。 所有其他参与者都放置在会议厅中。 |
| everyone | 每个人都可以参加会议。 会议厅中不放置任何参与者。 |
| invited | 只有组织者邀请的人才能参加会议并绕过会议厅。 所有其他参与者都放置在会议厅中。 |
| organizationExcludingGuests |  只有来自同一公司的参与者才能参加会议并绕过会议厅。 所有其他参与者都放置在会议厅中。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
