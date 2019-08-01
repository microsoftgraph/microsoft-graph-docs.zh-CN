---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2e9c65138a6dee7082b85261fd62c0fe9a9fd5e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028675"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 工作配置文件必需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值, 无意向。|
|lowSecurityBiometric|1|要求低安全基于生物特征的密码。|
|必需|双面|必需。|
|atLeastNumeric|第三章|至少需要数字密码。|
|numericComplex|4|需要数字复杂密码。|
|atLeastAlphabetic|5|至少需要字母密码。|
|atLeastAlphanumeric|型|至少需要字母数字密码。|
|alphanumericWithSymbols|步|至少需要带符号的字母数字密码。|



