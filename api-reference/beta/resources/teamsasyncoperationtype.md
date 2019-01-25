---
title: teamsAsyncOperationType 枚举类型
description: TeamsAsyncOperation 的类型。 将要添加的成员此处为多个异步支持操作。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516565"
---
# <a name="teamsasyncoperationtype-enum-type"></a>teamsAsyncOperationType 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsAsyncOperation](teamsasyncoperation.md)的类型。 将要添加的成员此处为多个异步支持操作。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|Invalid|0%|值无效|
|cloneTeam|$1|要克隆团队的操作。|
|archiveTeam|-2|若要存档团队的操作。|
|unarchiveTeam|-3|若要还原的存档的团队的操作。|
|createTeam|-3|若要从头开始创建团队的操作。|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
