---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d5fdb65510bcd287494b3966ca00bbe7f25b0a2fd5720338030bc1bcf8c11a64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183217"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者策略所需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意图。|
|必需|1 |必须设置密码，但对类型没有限制。|
|numeric|2 |至少为数字。|
|numericComplex|3 |至少为无重复序列或顺序序列的数值。|
|字母|4 |至少字母密码。|
|alphanumeric|5 |至少为字母数字密码|
|alphanumericWithSymbols|6 |至少为带符号的字母数字。|
|lowSecurityBiometric|7 |需要低安全生物识别密码。|
|customPassword|8 |管理员设置的自定义密码。|




