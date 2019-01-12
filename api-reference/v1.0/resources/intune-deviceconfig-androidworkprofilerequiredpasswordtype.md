---
title: androidWorkProfileRequiredPasswordType 枚举类型
description: Android 工作模板所需密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbe1eb1482e979d236c1f8bf92f687077fb189f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986276"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>androidWorkProfileRequiredPasswordType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 工作模板所需密码类型。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|lowSecurityBiometric|1|低安全性生物基于所需的密码。|
|必需|2|必填。|
|atLeastNumeric|3|所需的密码至少数值。|
|numericComplex|4|所需的数字复杂密码。|
|atLeastAlphabetic|5|所需的密码至少字母。|
|atLeastAlphanumeric|6|所需的至少字母数字密码。|
|alphanumericWithSymbols|7|使用所需的符号密码至少字母数字。|



