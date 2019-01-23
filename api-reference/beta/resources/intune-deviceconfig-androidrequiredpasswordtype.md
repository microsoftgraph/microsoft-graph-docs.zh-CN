---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eebc6b0ad6eed346927fd48a2dc1f82b5e529b28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392911"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




