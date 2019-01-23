---
title: deviceThreatProtectionLevel 枚举类型
description: 设备的设备威胁保护 API 的威胁保护级别。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411230"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备的设备威胁保护 API 的威胁保护级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|不可用|0|默认值。 请勿使用。|
|保护|1|设备威胁级别要求： 安全。 这是最安全的级别，表示在设备上未发现任何威胁。|
|低|2|设备威胁保护级别要求： 低。 低代表严重性为会带来风险降至最低到设备或设备数据的威胁。|
|中等|3|设备威胁保护级别要求： 中等。 中等代表严重性为威胁带来中等风险到的设备或设备数据。|
|高|4|设备威胁保护级别要求： 高。 高代表严重性为会造成严重到设备或设备数据风险的威胁。|
|notSet|10|设备威胁保护级别要求： 未设置。 不是设备，以满足了威胁保护级别不要求集代表。|




