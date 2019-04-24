---
title: 成员
description: 描述 teamsApp 的当前安装状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462247"
---
#<a name="teamsappinstalledstate-enum-type"></a>teamsAppInstalledState 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述[teamsApp](teamsapp.md)的当前安装状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|notInstalled|0|未将应用安装到团队。|
|了|1|应用程序以正常方式安装。|
|installedAndHidden|2 |已安装应用程序, 但已在视图中隐藏。|
|installedAndPermanent|3 |应用程序永久安装且不可能删除。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
