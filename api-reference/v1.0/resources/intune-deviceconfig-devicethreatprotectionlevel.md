---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af0231e15cfa815d3fd2e154adf180f3e0c0c43
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566813"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备威胁防护 API 的设备威胁保护级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|才|0|默认值。 请勿使用。|
|加密|1|设备威胁级别要求: 安全。 这是最安全的级别, 表示在设备上未发现任何威胁。|
|降低|2 |设备威胁保护级别要求: 低。 Low 表示对设备或设备数据带来最小风险的威胁的严重程度。|
|中等|3 |设备威胁保护级别要求: 中。 中型代表设备或设备数据面临中等风险的威胁的严重程度。|
|高效|4 |设备威胁保护级别要求: 高。 High 表示对设备或设备数据带来严重风险的威胁的严重程度。|
|notSet|10 |设备威胁保护级别要求: 未设置。 未设置表示设备不需要满足威胁保护级别。|



