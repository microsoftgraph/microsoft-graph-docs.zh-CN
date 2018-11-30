---
title: deviceThreatProtectionLevel 枚举类型
description: 设备的设备威胁保护 API 的威胁保护级别。
ms.openlocfilehash: 900ae43f962e0a7d122588fa35db6827d4accfc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043911"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





