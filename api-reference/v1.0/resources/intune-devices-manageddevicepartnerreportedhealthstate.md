---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c8a9401e55529aa3a9062f21ecb01772b142eea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533244"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备运行状况 API 的可用运行状况状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|尚未报告设备运行状况状态|
|已|1 |设备已由移动威胁防护合作伙伴激活，但尚未报告运行状况。|
|失效|2 |设备已被移动威胁防护合作伙伴停用。 设备运行状况未知。|
|加密|3 |移动威胁防护合作伙伴认为设备受安全保护。|
|lowSeverity|4 |移动威胁防护合作伙伴将设备视为低威胁。|
|mediumSeverity|5 |移动威胁防护合作伙伴认为设备是中型威胁。|
|highSeverity|6 |移动威胁防护合作伙伴将设备视为高威胁。|
|无|7 |移动威胁防护合作伙伴认为设备无响应。 设备运行状况未知。|
|威胁|8 |威胁防御合作伙伴认为设备受到威胁。 这意味着该设备具有活跃的威胁或风险，最终用户无法轻松修正该设备，并且用户应联系其 IT 管理员。|
|配置错误|9 |将设备视为与威胁防护合作伙伴配置不正确。 这意味着设备缺少必需的配置文件或配置以使威胁防护合作伙伴正常运行，因此威胁或风险分析无法完成。|




