---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
ms.openlocfilehash: 8dee8332155cd3d0ba94424090df94d07f214d18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047155"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

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





