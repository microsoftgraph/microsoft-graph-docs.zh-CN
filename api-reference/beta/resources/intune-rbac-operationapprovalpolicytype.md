---
title: operationApprovalPolicyType 枚举类型
description: 操作审批策略类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a7bf4c90ea38235ab674307a580382c50676ec5f
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60490260"
---
# <a name="operationapprovalpolicytype-enum-type"></a>operationApprovalPolicyType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作审批策略类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceActions|1|设备操作|
|deviceWipe|2|设备擦除操作|
|deviceRetire|3|设备停用操作|
|deviceRetireNonCompliant|4 |停用不兼容的设备操作|
|deviceDelete|5|设备删除操作|
|deviceLock|6 |设备锁定操作|
|deviceErase|7 |设备擦除操作|
|deviceDisableActivationLock|8 |设备禁用激活锁定操作|
|windowsEnrollment|9 |Windows注册|
|compliancePolicies|10 |合规性策略|
|configurationPolicies|11|配置策略|
|appProtectionPolicies|12 |应用保护策略|
|policySets|13|策略集|
|filters|14 |筛选器|
|endpointSecurity|15 |终结点安全性|
|apps|16|应用程序|
|脚本|17 |脚本|
|角色|18 |角色|
|unknownFutureValue|99|将来操作审批策略类型的占位符|



