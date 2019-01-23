---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cdf8c03dab6642cf6859ca822001a71b041c0e54
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399897"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 工作模板所需密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|lowSecurityBiometric|1|低安全性生物基于所需的密码。|
|必需|2|必需项。|
|atLeastNumeric|3|所需的密码至少数值。|
|numericComplex|4|所需的数字复杂密码。|
|atLeastAlphabetic|5|所需的密码至少字母。|
|atLeastAlphanumeric|6|所需的至少字母数字密码。|
|alphanumericWithSymbols|7|使用所需的符号密码至少字母数字。|




