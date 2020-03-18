---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6d783f8bdf5faeed2d3e10a9286a897c8d85783
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796984"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者策略需要密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|必需|1|必须设置密码，但类型没有限制。|
|位数|双面|至少为数值。|
|numericComplex|第三章|至少不带重复或有序序列的数字。|
|字母|4 |至少为字母密码。|
|字母数字|5 |至少为字母数字密码|
|alphanumericWithSymbols|6 |至少带有符号的字母数字。|
|lowSecurityBiometric|7 |要求低安全基于生物特征的密码。|
|customPassword|8 |由管理员设置的自定义密码。|



