---
title: clonableTeamParts 枚举类型
description: '描述应克隆团队的哪一部分。 '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 371f026b671f750ef67ec796d154fa3e399ac8967664466bdcb2bc498a11124c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252058"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

命名空间：microsoft.graph



描述应克隆 [团队](../resources/team.md) 的哪一部分。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|1|复制已安装应用的列表。|
|选项卡|2|在频道内复制选项卡。|
|settings|4 |复制团队内的所有设置以及关键组设置。|
|channels|8 |复制频道结构 (，但不复制频道中) 。|
|members|16 |复制团队的成员和所有者。|

