---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件必需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5e89c96d08fa1c265647692b3edb831fd308b7f7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730677"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 工作配置文件必需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|lowSecurityBiometric|1|要求低安全基于生物特征的密码。|
|必需|双面|必需。|
|atLeastNumeric|第三章|至少需要数字密码。|
|numericComplex|4 |需要数字复杂密码。|
|atLeastAlphabetic|5 |至少需要字母密码。|
|atLeastAlphanumeric|6 |至少需要字母数字密码。|
|alphanumericWithSymbols|7 |至少需要带符号的字母数字密码。|





