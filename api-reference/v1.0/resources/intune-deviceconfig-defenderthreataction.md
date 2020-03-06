---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4c9edcd596d6dcd40b2cfe873b660651f74bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530856"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对检测到的恶意软件威胁执行的 Defender 的默认操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|根据更新定义应用操作。|
|清理|1 |清理检测到的威胁。|
|隔离|2 |隔离检测到的威胁。|
|删除|3 |删除检测到的威胁。|
|允许|4 |允许检测到的威胁。|
|定制|5 |允许用户确定要对检测到的威胁采取的操作。|
|数据|6 |阻止检测到的威胁。|




