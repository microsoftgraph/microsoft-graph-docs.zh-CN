---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511707"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|Invalid|0%|值无效|
|NotStarted|$1|尚未开始此操作。|
|InProgress|-2|正在运行的操作。|
|succeeded|-3|操作成功。|
|failed|-4|操作失败。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
