---
title: clonableTeamParts 枚举类型
description: '介绍应克隆的团队部分。 '
localization_priority: Normal
author: nkramer
ms.prod: ''
doc_type: enumPageType
ms.openlocfilehash: 5d9121d7cbaa10260b1a7a7ce180ed7c9f37a565
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086807"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

命名空间：microsoft.graph



介绍应克隆的 [团队](../resources/team.md) 部分。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|1 |复制已安装应用程序的列表。|
|选项卡|2 |复制通道中的选项卡。|
|settings|4 |复制团队中的所有设置以及关键组设置。|
|channels|8 |将通道结构 (，但不会复制频道) 中的邮件。|
|members|16 |复制团队的成员和所有者。|

