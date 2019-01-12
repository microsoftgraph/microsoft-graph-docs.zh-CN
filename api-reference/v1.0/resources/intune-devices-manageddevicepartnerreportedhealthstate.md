---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 可用的运行状况状态的设备运行状况 API
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85d6731fc34bb3133fa7aed631d3d687a45a7dce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919048"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

可用的运行状况状态的设备运行状况 API
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|unknown|0|设备运行状况不尚未报告|
|激活|1|设备已激活通过移动的威胁防御合作伙伴，但不是报告运行状况。|
|停用|2|已由移动的威胁防御合作伙伴停用设备。 未知设备运行状况。|
|保护|3|设备被视为受移动的威胁防御合作伙伴。|
|lowSeverity|4|设备通过移动的威胁防御合作伙伴视为低威胁。|
|mediumSeverity|5|设备通过移动的威胁防御合作伙伴视为中型威胁。|
|highSeverity|6|设备通过移动的威胁防御合作伙伴视为高威胁。|
|未响应|7|移动的威胁防御合作伙伴被视为设备未响应。 未知设备运行状况。|
|威胁|8|设备被视为受到威胁防御合作伙伴。 这意味着设备具有活动的威胁或无法由最终用户轻松修正风险和用户应联系其 IT 管理员。|
|配置错误|9|设备被视为与威胁防御合作伙伴配置正确。 这意味着设备缺少必需的配置文件或配置威胁防御伙伴能够正常工作，因此威胁或不能完成风险分析。|



