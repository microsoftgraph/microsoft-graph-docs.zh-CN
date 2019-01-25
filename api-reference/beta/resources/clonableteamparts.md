---
title: clonableTeamParts 枚举类型
description: '描述应克隆的工作组的一部分。 '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511462"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述应克隆的[工作组](../resources/team.md)的一部分。 

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|$1|将复制已安装的应用程序的列表。|
|标签|-2|将复制通道中的选项卡。|
|settings|-4|将复制的团队，以及关键组设置中的所有设置。|
|channels|-8|将复制的通道结构 （但不是在进入频道的消息）。|
|members|1.6|将复制的成员和所有者的团队。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
