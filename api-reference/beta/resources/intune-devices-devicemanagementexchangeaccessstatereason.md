---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态原因。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 00f9c44237052b4f15917763c6452c1a909543fc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784921"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备 Exchange 访问状态原因。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未发现来自 Exchange 的访问状态原因|
|unknown|1|未知访问状态原因|
|exchangeGlobalRule|双面|由 Exchange 全局规则确定的访问状态|
|exchangeIndividualRule|第三章|由 Exchange 单个规则确定的访问状态|
|exchangeDeviceRule|4 |由 Exchange 设备规则确定的访问状态|
|exchangeUpgrade|5 |Exchange 升级导致的访问状态|
|exchangeMailboxPolicy|6 |由 Exchange 邮箱策略确定的访问状态|
|相互|7 |由 Exchange 确定的访问状态|
|合格|8 |合规性挑战授予的访问状态|
|notCompliant|9 |由合规性挑战吊销的访问状态|
|notEnrolled|10 |由管理质询吊销的访问状态|
|unknownLocation|12 |由于未知位置导致的访问状态|
|mfaRequired|13 |由于 MFA 质询而导致的访问状态|
|azureADBlockDueToAccessPolicy|14 |由 AAD 访问策略吊销的访问状态|
|compromisedPassword|15 |通过密码被破解的密码吊销的访问状态|
|deviceNotKnownWithManagedApp|16 |由托管应用程序质询吊销的访问状态|



