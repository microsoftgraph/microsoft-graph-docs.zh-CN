---
title: teamClassSettings 资源类型
description: 表示特定于类型为 "类" 的团队的设置。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ec19534662f379be50ec778acc3037e32349f63
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865758"
---
# <a name="teamclasssettings-resource-type"></a>teamClassSettings 资源类型

表示[团队](team.md)的特定于类的属性。 仅当团队代表班级时可用。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Boolean|如果设置为`true`，则允许将每周分配摘要电子邮件发送给父/监护人，前提是租户管理员已启用全局设置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
