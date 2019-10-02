---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 71533fa6d01c9c51980881429b4dc3e443f9c766
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359675"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对检测到的恶意软件威胁执行的 Defender 的默认操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|根据更新定义应用操作。|
|清理|1|清理检测到的威胁。|
|隔离|双面|隔离检测到的威胁。|
|删除|第三章|删除检测到的威胁。|
|允许|4|允许检测到的威胁。|
|定制|5|允许用户确定要对检测到的威胁采取的操作。|
|数据|型|阻止检测到的威胁。|




