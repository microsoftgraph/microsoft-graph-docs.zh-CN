---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态的原因。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 96bcc60daa0ec69788856413bf1d253d8b0cabfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834790"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备 Exchange 访问状态的原因。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|从 Exchange 发现没有访问状态理由|
|unknown|1|未知的访问状态的原因|
|exchangeGlobalRule|2|由 Exchange 全局规则的访问状态|
|exchangeIndividualRule|3|由 Exchange 单个规则的访问状态|
|exchangeDeviceRule|4|由 Exchange 设备规则的访问状态|
|exchangeUpgrade|5|由于 Exchange 升级的访问状态|
|exchangeMailboxPolicy|6|由 Exchange 邮箱策略的访问状态|
|其他|7|由 Exchange 的访问状态|
|符合标准|8|通过合规性质询授予的访问状态|
|notCompliant|9|合规性质询被吊销的访问状态|
|notEnrolled|10|管理质询被吊销的访问状态|
|unknownLocation|12|由于未知位置的访问状态|
|mfaRequired|13|由于 MFA 质询的访问状态|
|azureADBlockDueToAccessPolicy|14|由 AAD 访问策略吊销的访问状态|
|compromisedPassword|15|由受到攻击的密码吊销的访问状态|
|deviceNotKnownWithManagedApp|16|由托管应用程序质询吊销的访问状态|



