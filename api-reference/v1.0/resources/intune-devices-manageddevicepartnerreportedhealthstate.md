---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 775a8d6419b8370e7c962432780b5f0d2e3e0ae4
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729956"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备运行状况 API 的可用运行状况状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|尚未报告设备运行状况状态|
|激活|1|设备已由移动威胁防御合作伙伴激活，但尚未报告运行状况。|
|关闭|2|移动威胁防御合作伙伴已停用设备。 设备运行状况未知。|
|担保|3|设备由移动威胁防御合作伙伴视为受保护。|
|lowSeverity|4|移动威胁防御合作伙伴将设备视为低威胁。|
|mediumSeverity|5|移动威胁防御合作伙伴将设备视为中等威胁。|
|highSeverity|6 |移动威胁防御合作伙伴将设备视为高威胁。|
|反应 迟钝|7 |移动威胁防御合作伙伴认为设备无响应。 设备运行状况未知。|
|妥协|8 |威胁防御合作伙伴认为设备已泄露。 这意味着设备具有活动威胁或风险，最终用户无法轻松修正，用户应联系其 IT 管理员。|
|配置错误|9 |设备被视为与威胁防御合作伙伴配置错误。 这意味着设备缺少威胁防御合作伙伴正常运行所需的配置文件或配置，因此威胁或风险分析无法完成。|





