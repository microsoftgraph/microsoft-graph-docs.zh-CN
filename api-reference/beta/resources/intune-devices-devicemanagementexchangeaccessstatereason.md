---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备 Exchange 访问状态的原因。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 25d5ac8a5624352b9c474caf4088709ca1453387
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981845"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





