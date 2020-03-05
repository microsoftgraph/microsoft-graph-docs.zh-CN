---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略需要密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fda5f4ee9e8565180100ca96b227727b20efa2eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486365"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者策略需要密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|必需|1 |必须设置密码，但类型没有限制。|
|位数|2 |至少为数值。|
|numericComplex|3 |至少不带重复或有序序列的数字。|
|字母|4 |至少为字母密码。|
|字母数字|5 |至少为字母数字密码|
|alphanumericWithSymbols|6 |至少带有符号的字母数字。|
|lowSecurityBiometric|7 |要求低安全基于生物特征的密码。|
|customPassword|8 |由管理员设置的自定义密码。|



