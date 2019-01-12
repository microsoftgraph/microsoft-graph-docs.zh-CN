---
title: androidDeviceOwnerRequiredPasswordType 枚举类型
description: Android 设备所有者策略要求密码类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1208de597baff9dd05a48663435a3a928f3dae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938039"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





