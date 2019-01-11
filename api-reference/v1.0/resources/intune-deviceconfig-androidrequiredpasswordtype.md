---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 06a89256920f143af923e6a3949e61843fa7aa00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814418"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 所需的密码类型。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|字母|1|所需的密码字母。|
|字母数字|2|所需的字母数字密码。|
|alphanumericWithSymbols|3|所需的符号密码全角字母数字。|
|lowSecurityBiometric|4|低安全性生物基于所需的密码。|
|数值|5|所需的数字密码。|
|numericComplex|6|所需的数字复杂密码。|
|任意|7|Password 或模式是必需的且任何可接受。|



