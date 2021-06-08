---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d179666a4de9256e98c704bccd9e512d4aebd0ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760284"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 所需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意图。|
|字母|1|需要字母密码。|
|alphanumeric|2|需要字母数字密码。|
|alphanumericWithSymbols|3|需要符号密码的字母数字。|
|lowSecurityBiometric|4 |需要低安全生物识别密码。|
|numeric|5 |需要数字密码。|
|numericComplex|6 |需要数字复杂密码。|
|任意|7 |密码或模式是必需的，任何密码或模式都是可接受的。|




