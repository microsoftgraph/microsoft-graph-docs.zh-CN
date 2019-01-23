---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 可用的运行状况状态的设备运行状况 API
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb5b13ceceab27e1e88a69310a3198159f5e24c1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418825"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

可用的运行状况状态的设备运行状况 API

## <a name="members"></a>成员
|成员|值|说明|
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




