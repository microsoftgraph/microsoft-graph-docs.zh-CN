---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备Exchange访问状态原因。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7aa61e8ecdf88663123a486cb9bccb033aeecbb5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754572"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备Exchange访问状态原因。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|未从用户发现任何访问Exchange|
|unknown|1|未知访问状态原因|
|exchangeGlobalRule|2|由全局规则Exchange的访问状态|
|exchangeIndividualRule|3|由单个规则Exchange的访问状态|
|exchangeDeviceRule|4 |由设备规则Exchange的访问状态|
|exchangeUpgrade|5 |由于升级Exchange访问状态|
|exchangeMailboxPolicy|6 |由邮箱策略Exchange的访问状态|
|other|7 |访问状态由用户Exchange|
|compliant|8 |合规性质询授予的访问状态|
|notCompliant|9 |合规性质询撤销的访问状态|
|notEnrolled|10  |管理质询撤销的访问状态|
|unknownLocation|12 |由于位置未知而进入访问状态|
|mfaRequired|13|MFA 质询导致的访问状态|
|azureADBlockDueToAccessPolicy|14 |AAD 访问策略吊销的访问状态|
|compromisedPassword|15|通过泄露的密码吊销的访问状态|
|deviceNotKnownWithManagedApp|16 |托管应用程序质询吊销的访问状态|




