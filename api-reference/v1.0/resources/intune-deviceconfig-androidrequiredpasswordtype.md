---
title: androidRequiredPasswordType 枚举类型
description: Android 必需的密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e1ac4e27243adc47b087aa6453ff316d9b2e2fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530963"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 必需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|字母|1 |要求字母密码。|
|字母数字|2 |需要字母数字密码。|
|alphanumericWithSymbols|3 |需要带符号的字母数字密码。|
|lowSecurityBiometric|4 |要求低安全基于生物特征的密码。|
|位数|5 |需要数字密码。|
|numericComplex|6 |需要数字复杂密码。|
|任意|7 |需要密码或模式，可以接受。|




