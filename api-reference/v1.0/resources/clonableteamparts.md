---
title: clonableTeamParts 枚举类型
description: '描述应克隆团队的哪一部分。 '
ms.localizationpriority: medium
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 29ed2da8079d00576d19e94d792da0b1af423781
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109281"
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
|channels|8 |将通道结构 (，但不复制频道中的) 。|
|members|16 |复制团队的成员和所有者。|

