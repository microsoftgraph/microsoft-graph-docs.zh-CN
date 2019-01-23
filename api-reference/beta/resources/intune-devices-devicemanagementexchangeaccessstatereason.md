---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态的原因。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7a076239e49c59cb95cd1c1f644bc9a2f1f906e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395858"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备 Exchange 访问状态的原因。

## <a name="members"></a>成员
|成员|值|说明|
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




