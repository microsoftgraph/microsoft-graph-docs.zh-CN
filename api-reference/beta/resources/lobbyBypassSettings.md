---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议厅。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fbf6aada6f4a748a615f660e4a3ec62322116bdc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962096"
---
# <a name="lobbybypasssettings-resource-type"></a>lobbyBypassSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定哪些参与者可以绕过会议厅。

## <a name="properties"></a>属性

| 属性              | 类型    | 说明                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | 指定自动获准加入会议、绕过会议厅的参与者类型。 下表列出了可能的值。 可选。|
| isDialInBypassEnabled | Boolean | 指定是否始终允许拨入呼叫者绕过大厅。 可选。 | 

### <a name="lobbybypassscope-values"></a>lobbyBypassScope 值

| 值                    | 说明                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer － 组织者                | 仅组织者可以进入会议，绕过会议厅。 所有其他参与者都放置在会议厅中。                                                                                                         |
| 组织             | 只有来自同一公司的参与者可以绕过会议厅参加会议。 所有其他参与者都放置在会议厅中。                                                                              |
| organizationAndFederated | 只有来自同一公司或受信任组织的参与者可以绕过会议厅参加会议。 所有其他参与者都放置在会议厅中。 |
| everyone                 | 每个人都可以参加会议。 会议厅中不放置任何参与者。                                                                                                                   |
| unknownFutureValue       | 不知情未来值。                                                                                                                                     |

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
