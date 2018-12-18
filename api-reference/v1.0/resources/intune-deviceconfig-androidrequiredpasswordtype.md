---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: tfitzmac
ms.openlocfilehash: e9b757dc86bf71462f7f987cedfcd9e04497880e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349215"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 所需的密码类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|字母|1|所需的密码字母。|
|字母数字|2|所需的字母数字密码。|
|alphanumericWithSymbols|3|所需的符号密码全角字母数字。|
|lowSecurityBiometric|4|低安全性生物基于所需的密码。|
|数值|5|所需的数字密码。|
|numericComplex|6|所需的数字复杂密码。|
|任意|7|Password 或模式是必需的且任何可接受。|



