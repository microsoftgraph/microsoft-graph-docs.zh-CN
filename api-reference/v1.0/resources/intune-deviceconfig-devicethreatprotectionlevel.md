---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁防护级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3765e3cbdd8ea1ae40183d621a7ff0fb352ba19fcfa58b27201b5eb62b4e20ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163780"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备威胁防护 API 的设备威胁防护级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|不可用|0|默认值。 请勿使用。|
|secured|1|设备威胁级别要求：安全。 这是最安全级别，表示未在设备上发现任何威胁。|
|low|2|设备威胁防护级别要求：低。 低表示威胁的严重性，对设备或设备数据带来的风险最小。|
|中等|3|设备威胁防护级别要求：中等。 中等表示威胁的严重性，对设备或设备数据带来中等风险。|
|high|4 |设备威胁防护级别要求：高。 高表示威胁的严重性，对设备或设备数据带来高风险。|
|notSet|10 |设备威胁防护级别要求：未设置。 未设置表示设备无需满足威胁防护级别。|




