---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁防护级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 55b2cc465f33312fe939f9c2c826846a94bce2eb
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735744"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备威胁防护 API 的设备威胁防护级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无法|0|默认值。 请勿使用。|
|担保|1|设备威胁级别要求：安全。 这是最安全的级别，表示设备上未发现任何威胁。|
|低|2|设备威胁防护级别要求：低。 低表示对设备或设备数据构成最小风险的威胁严重性。|
|中等|3|设备威胁防护级别要求：中等。 中等表示对设备或设备数据构成中等风险的威胁严重性。|
|高|4|设备威胁防护级别要求：高。 高表示威胁的严重性，对设备或设备数据构成严重风险。|
|notSet|10|设备威胁防护级别要求：未设置。 未设置表示设备无需满足威胁防护级别。|





