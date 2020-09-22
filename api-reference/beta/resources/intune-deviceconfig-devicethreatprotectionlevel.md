---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6169a6f7816a04b0e3a81065fc78869eadc3b7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040026"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备威胁防护 API 的设备威胁保护级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|才|0|默认值。 请勿使用。|
|加密|1 |设备威胁级别要求：安全。 这是最安全的级别，表示在设备上未发现任何威胁。|
|降低|2 |设备威胁保护级别要求：低。 Low 表示对设备或设备数据带来最小风险的威胁的严重程度。|
|中等|第三章|设备威胁保护级别要求：中。 中型代表设备或设备数据面临中等风险的威胁的严重程度。|
|高效|4 |设备威胁保护级别要求：高。 High 表示对设备或设备数据带来严重风险的威胁的严重程度。|
|notSet|10 |设备威胁保护级别要求：未设置。 未设置表示设备不需要满足威胁保护级别。|






