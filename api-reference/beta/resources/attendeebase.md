---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
ms.openlocfilehash: bce1550c107f2114d02744091b5863360ab0bcea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535611"
---
# <a name="attendeebase-resource-type"></a>attendeeBase 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与会者类型。

由 [recipient](recipient.md) 派生。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|类型|String| 与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。|
|emailAddress|[emailAddress](emailaddress.md)|添加与会者姓名和 SMTP 地址。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
