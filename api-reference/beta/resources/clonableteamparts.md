---
title: clonableTeamParts 枚举类型
description: '介绍应克隆的团队部分。 '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: nkramer
ms.openlocfilehash: 666dc3cc60490a9a30a5e2bab0b0642c34fb5009
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034076"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍应克隆的 [团队](../resources/team.md) 部分。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|1 |复制已安装应用程序的列表。|
|选项卡|2 |复制通道中的选项卡。|
|settings|4 |复制团队中的所有设置以及关键组设置。|
|channels|8 |将通道结构 (，但不会复制频道) 中的邮件。|
|members|16 |复制团队的成员和所有者。|


