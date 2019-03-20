---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 376e33edac921f6771d76a45622a58bca3076c5c
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572332"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者策略需要密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值, 无意向。|
|必需|1|必须设置密码, 但类型没有限制。|
|位数|双面|至少为数值。|
|numericComplex|第三章|至少不带重复或有序序列的数字。|
|字母|4|至少为字母密码。|
|字母数字|5|至少为字母数字密码|
|alphanumericWithSymbols|型|至少带有符号的字母数字。|
|lowSecurityBiometric|步|要求低安全基于生物特征的密码。|




