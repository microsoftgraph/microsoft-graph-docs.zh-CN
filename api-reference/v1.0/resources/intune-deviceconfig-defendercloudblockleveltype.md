---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 658a484a29ebed8cb111ded81ef439a560c87ac0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366627"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

云块级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险|
|高效|1|High 适用于强级别的检测。|
|highPlus|双面|高级别 + 使用高级别，并应用附加保护措施|
|zeroTolerance|第三章|零耐受性阻止所有未知可执行文件|




