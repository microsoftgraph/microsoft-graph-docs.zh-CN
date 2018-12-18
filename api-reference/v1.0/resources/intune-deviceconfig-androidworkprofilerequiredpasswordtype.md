---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
author: tfitzmac
ms.openlocfilehash: 64b5dfcd5b919a428ef6823856dbf67102a316c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331659"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 工作模板所需密码类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|lowSecurityBiometric|1|低安全性生物基于所需的密码。|
|必需|2|必需。|
|atLeastNumeric|3|所需的密码至少数值。|
|numericComplex|4|所需的数字复杂密码。|
|atLeastAlphabetic|5|所需的密码至少字母。|
|atLeastAlphanumeric|6|所需的至少字母数字密码。|
|alphanumericWithSymbols|7|使用所需的符号密码至少字母数字。|



