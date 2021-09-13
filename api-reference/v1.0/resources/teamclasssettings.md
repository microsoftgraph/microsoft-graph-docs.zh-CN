---
title: teamClassSettings 资源类型
description: 表示特定于类类型的团队的设置。
ms.localizationpriority: medium
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fd7a3163abd23d7c009ef3a03c668335eeb1e453
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134358"
---
# <a name="teamclasssettings-resource-type"></a>teamClassSettings 资源类型

命名空间：microsoft.graph

表示团队的特定于类 [的属性](team.md)。 仅当团队代表班级时可用。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|布尔值|如果设置为 ，则允许向家长/监护人发送每周作业摘要电子邮件，但租户管理员已全局启用 `true` 该设置。|

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

