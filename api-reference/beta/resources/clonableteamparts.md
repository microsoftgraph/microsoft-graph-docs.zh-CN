---
title: clonableTeamParts 枚举类型
description: '描述应克隆团队的哪个部分。 '
ms.localizationpriority: medium
doc_type: enumPageType
ms.prod: teamwork
author: nkramer
ms.openlocfilehash: 99a50eb62af486b1d5eb84ae779627bbf8509cc1
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944143"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述应克隆 [团队](../resources/team.md) 的哪个部分。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|1|复制已安装应用的列表。|
|选项卡|2|复制通道中的选项卡。|
|settings|4|复制团队中的所有设置以及关键组设置。|
|channels|8 |复制通道结构 (但不复制通道) 中的消息。|
|members|16|复制团队的成员和所有者。|


