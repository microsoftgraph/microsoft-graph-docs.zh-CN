---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c788a08e09816683ed575898ee5f36cba241a8bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175260"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备 Exchange 访问状态原因。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未发现来自 Exchange 的访问状态原因|
|unknown|1|未知访问状态原因|
|exchangeGlobalRule|双面|由 Exchange 全局规则确定的访问状态|
|exchangeIndividualRule|第三章|由 Exchange 单个规则确定的访问状态|
|exchangeDeviceRule|4|由 Exchange 设备规则确定的访问状态|
|exchangeUpgrade|5|Exchange 升级导致的访问状态|
|exchangeMailboxPolicy|型|由 Exchange 邮箱策略确定的访问状态|
|相互|步|由 Exchange 确定的访问状态|
|合格|utf-8|合规性挑战授予的访问状态|
|notCompliant|第|由合规性挑战吊销的访问状态|
|notEnrolled|10|由管理质询吊销的访问状态|
|unknownLocation|12|由于未知位置导致的访问状态|
|mfaRequired|13|由于 MFA 质询而导致的访问状态|
|azureADBlockDueToAccessPolicy|日|由 AAD 访问策略吊销的访问状态|
|compromisedPassword|个|通过密码被破解的密码吊销的访问状态|
|deviceNotKnownWithManagedApp|位|由托管应用程序质询吊销的访问状态|




