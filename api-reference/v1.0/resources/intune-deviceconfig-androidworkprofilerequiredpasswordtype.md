---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作配置文件需要密码类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 08c878b764e658c8272054b71262ae5607e2585f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736480"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 工作配置文件需要密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|lowSecurityBiometric|1|所需的基于生物识别的低安全性密码。|
|必需|2|必需。|
|atLeastNumeric|3|至少需要数值密码。|
|numericComplex|4|所需的数值复杂密码。|
|atLeastAlphabetic|5|至少需要字母密码。|
|atLeastAlphanumeric|6 |至少需要字母数字密码。|
|alphanumericWithSymbols|7 |至少具有所需符号密码的字母数字。|





