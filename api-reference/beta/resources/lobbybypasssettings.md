---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议大厅。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: db525d4d3a4f2999dd637745532789043b4f68df
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884165"
---
# <a name="lobbybypasssettings-resource-type"></a>lobbyBypassSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定哪些参与者可以绕过会议大厅。

## <a name="properties"></a>属性

| 属性              | 类型    | 说明                                                         |
| --------------------- | ------- | ------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | 指定绕过大厅自动进入会议的参与者类型。 可选。|
| isDialInBypassEnabled | 布尔 | 指定是否始终让拨入呼叫者绕过大厅。 可选。 |

### <a name="lobbybypassscope-values"></a>lobbyBypassScope 值

下表列出了 [可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)的成员。 必须使用`Prefer: include-unknown-enum-members`请求标头获取此可旋转枚举中的以下值： `invited``organizationExcludingGuests`

| 值                    | 说明     |
| ------------------------ | --------------------------------------------------- |
| 组织者 | 只有组织者可以进入会议并绕过大厅。 所有其他参与者都放置在会议大厅中。 |
| 组织 | 只有来自同一家公司的参与者 **和客人** 才能参加会议，并绕过大厅。 所有其他参与者都放置在会议大厅中。 |
| organizationAndFederated | 只有来自同一公司或受信任组织和来宾的参与者才能参加会议并绕过大厅。 所有其他参与者都放置在会议大厅中。 |
| 每个人 都 | 每个人都可以参加会议。 会议大厅中没有参与者。 |
| 邀请 | 只有组织者邀请的人员才能进入会议并绕过大厅。 所有其他参与者都放置在会议大厅中。 |
| organizationExcludingGuests |  只有来自同一公司的参与者才能参加会议，并绕过大厅。 所有其他参与者都放置在会议大厅中。 |
| unknownFutureValue | 可变枚举 sentinel 值。 请勿使用。 |

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
