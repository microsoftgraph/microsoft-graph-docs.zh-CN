---
title: defenderThreatAction 枚举类型
description: Defender 对检测到的恶意软件威胁采取的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a14e8f638460b16763183501ea38b361e4307f0b95654f0712ce38d8a7557780
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184772"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 对检测到的恶意软件威胁采取的默认操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|根据更新定义应用操作。|
|clean|1|清理检测到的威胁。|
|隔离|2|隔离检测到的威胁。|
|remove|3|删除检测到的威胁。|
|allow|4 |允许检测到的威胁。|
|userDefined|5 |允许用户确定对检测到的威胁要采取的操作。|
|block|6 |阻止检测到的威胁。|




