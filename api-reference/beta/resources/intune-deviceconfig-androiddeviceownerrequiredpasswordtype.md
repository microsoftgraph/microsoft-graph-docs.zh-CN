---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc6d81a71fe01addb6111252b28aee01072fe0dd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949064"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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




