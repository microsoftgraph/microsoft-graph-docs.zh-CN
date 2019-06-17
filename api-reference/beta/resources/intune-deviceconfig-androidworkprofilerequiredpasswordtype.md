---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1ebbbb51390d5d96afcfe0e2d4805e0ba9a3007
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993772"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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





