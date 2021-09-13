---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 78bd301c77f6437b1382dec4d845186879e5e117
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040139"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备运行状况 API 的可用运行状况状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|尚未报告设备运行状况|
|activated|1|设备已由移动威胁防护合作伙伴激活，但尚未报告运行状况。|
|deactivated|2|设备已被移动威胁防护合作伙伴停用。 设备运行状况未知。|
|secured|3|设备被视为受移动威胁防护合作伙伴保护。|
|lowSeverity|4 |移动威胁防护合作伙伴将设备视为低威胁。|
|mediumSeverity|5 |移动威胁防护合作伙伴将设备视为中等威胁。|
|highSeverity|6 |移动威胁防护合作伙伴将设备视为高威胁。|
|unresponsive|7 |移动威胁防护合作伙伴认为设备无响应。 设备运行状况未知。|
|compromised|8 |威胁防护合作伙伴认为设备遭到入侵。 这意味着设备存在一个活动的"威胁或风险"，最终用户无法轻松修复此威胁或风险，并且用户应联系其 IT 管理员。|
|misconfigured|9 |设备被视为与威胁防护合作伙伴配置不当。 这意味着设备缺少所需配置文件或配置，威胁防护合作伙伴才能正常运行，因此无法完成威胁或风险分析。|



