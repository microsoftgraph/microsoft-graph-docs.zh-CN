---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e64bc6465e190e4e5da3629b6d638dc82813a2bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359381"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备威胁防护 API 的设备威胁保护级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|才|0|默认值。 请勿使用。|
|加密|1|设备威胁级别要求：安全。 这是最安全的级别，表示在设备上未发现任何威胁。|
|降低|双面|设备威胁保护级别要求：低。 Low 表示对设备或设备数据带来最小风险的威胁的严重程度。|
|中等|第三章|设备威胁保护级别要求：中。 中型代表设备或设备数据面临中等风险的威胁的严重程度。|
|高效|4|设备威胁保护级别要求：高。 High 表示对设备或设备数据带来严重风险的威胁的严重程度。|
|notSet|10 |设备威胁保护级别要求：未设置。 未设置表示设备不需要满足威胁保护级别。|




