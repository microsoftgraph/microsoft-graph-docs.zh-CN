---
title: clonableTeamParts 枚举类型
description: '描述应克隆的工作组的一部分。 '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860555"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

描述应克隆的[工作组](../resources/team.md)的一部分。 

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|apps|1|将复制已安装的应用程序的列表。|
|选项卡|2|将复制通道中的选项卡。|
|settings|4|将复制的团队，以及关键组设置中的所有设置。|
|通道|8|将复制的通道结构 （但不是在进入频道的消息）。|
|members|16|将复制的成员和所有者的团队。|
