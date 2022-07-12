---
title: androidRequiredPasswordType 枚举类型
description: Android 所需的密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ae76d6e260dfdef8d269ab20448d38b7c751f0ec
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733876"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 所需的密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|字母|1|所需的字母密码。|
|字母|2|所需的字母数字密码。|
|alphanumericWithSymbols|3|具有所需的符号密码的字母数字。|
|lowSecurityBiometric|4|所需的基于生物识别的低安全性密码。|
|数字|5|所需的数值密码。|
|numericComplex|6 |所需的数值复杂密码。|
|任意|7 |需要密码或模式，任何密码或模式都是可接受的。|





