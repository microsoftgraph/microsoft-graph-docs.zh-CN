---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备交换访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6cc10fd962a43ed87179299f22e48d84c7c13ba
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736067"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备交换访问状态原因。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未从 Exchange 发现访问状态原因|
|unknown|1|未知的访问状态原因|
|exchangeGlobalRule|2|由 Exchange 全局规则确定的访问状态|
|exchangeIndividualRule|3|由 Exchange 单个规则确定的访问状态|
|exchangeDeviceRule|4|由 Exchange 设备规则确定的访问状态|
|exchangeUpgrade|5|Exchange 升级导致的访问状态|
|exchangeMailboxPolicy|6 |Exchange 邮箱策略确定的访问状态|
|其他|7 |Exchange 确定的访问状态|
|兼容|8 |合规性质询授予的访问状态|
|notCompliant|9 |合规性质询撤销的访问状态|
|notEnrolled|10|管理质询撤销的访问状态|
|unknownLocation|12 |由于位置未知而导致的访问状态|
|mfaRequired|13|由于 MFA 质询而导致的访问状态|
|azureADBlockDueToAccessPolicy|14|AAD 访问策略撤销的访问状态|
|compromisedPassword|15|被泄露的密码吊销的访问状态|
|deviceNotKnownWithManagedApp|16|托管应用程序质询撤销的访问状态|





