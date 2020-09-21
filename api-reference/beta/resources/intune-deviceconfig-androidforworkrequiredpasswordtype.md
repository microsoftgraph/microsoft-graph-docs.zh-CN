---
title: androidForWorkRequiredPasswordType 枚举类型
description: 适用于工作所需密码类型的 Android。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20c7e330d060346557717e9eea0924b275c60d04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968491"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a>androidForWorkRequiredPasswordType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于工作所需密码类型的 Android。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，无意向。|
|lowSecurityBiometric|1 |要求低安全基于生物特征的密码。|
|必需|2 |必需。|
|atLeastNumeric|第三章|至少需要数字密码。|
|numericComplex|4 |需要数字复杂密码。|
|atLeastAlphabetic|5 |至少需要字母密码。|
|atLeastAlphanumeric|6 |至少需要字母数字密码。|
|alphanumericWithSymbols|7 |至少需要带符号的字母数字密码。|






