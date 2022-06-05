---
title: clonableTeamParts 枚举类型
description: '描述应克隆团队的哪个部分。 '
ms.localizationpriority: medium
author: nkramer
ms.prod: teamwork
doc_type: enumPageType
ms.openlocfilehash: cf317d3487cbd4a29bb860abda4510c2223aec24
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899440"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

命名空间：microsoft.graph



描述应克隆 [团队](../resources/team.md) 的哪个部分。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|1|复制已安装应用的列表。|
|选项卡|2|复制通道中的选项卡。|
|settings|4|复制团队中的所有设置以及关键组设置。|
|channels|8 |复制通道结构 (但不复制通道) 中的消息。|
|members|16|复制团队的成员和所有者。|

