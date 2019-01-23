---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略要求密码类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403537"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者策略要求密码类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|必需|1|必须有一密码，但没有任何限制类型。|
|数值|2|在至少数值。|
|numericComplex|3|在与没有重复或有序序列至少数值。|
|字母|4|至少字母数字密码。|
|字母数字|5|至少字母数字密码|
|alphanumericWithSymbols|6|替换为长划线至少字母数字。|




