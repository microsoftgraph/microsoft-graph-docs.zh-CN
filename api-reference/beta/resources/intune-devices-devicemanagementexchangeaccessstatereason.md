---
title: deviceManagementExchangeAccessStateReason 枚举类型
description: 设备Exchange访问状态原因。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5f6b1dd60e9a8880502bd04e77efc3a0dc53f82b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125979"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备Exchange访问状态原因。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未从用户发现任何访问Exchange|
|unknown|1|未知访问状态原因|
|exchangeGlobalRule|2|由全局规则Exchange的访问状态|
|exchangeIndividualRule|3|由单个规则Exchange的访问状态|
|exchangeDeviceRule|4 |由设备规则Exchange的访问状态|
|exchangeUpgrade|5 |由于升级Exchange访问状态|
|exchangeMailboxPolicy|6 |由邮箱策略Exchange的访问状态|
|other|7 |由用户确定的访问Exchange|
|compliant|8 |合规性质询授予的访问状态|
|notCompliant|9 |合规性质询撤销的访问状态|
|notEnrolled|10 |管理质询吊销的访问状态|
|unknownLocation|12 |由于位置未知而进入访问状态|
|mfaRequired|13|MFA 质询导致的访问状态|
|azureADBlockDueToAccessPolicy|14 |AAD 访问策略吊销的访问状态|
|compromisedPassword|15 |通过泄露的密码吊销的访问状态|
|deviceNotKnownWithManagedApp|16 |托管应用程序质询吊销的访问状态|



