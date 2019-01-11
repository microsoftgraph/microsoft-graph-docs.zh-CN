---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b755d213d39beb228afe603b2066b55416f14c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857321"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备注册状态。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notRegistered|0|未注册设备。|
|注册|2|已注册设备。|
|吊销|3|已阻止、 擦除或停用该设备。|
|keyConflict|4|设备具有键冲突。|
|approvalPending|5|设备是待审批状态。|
|certificateReset|6|设备证书已被重置。|
|notRegisteredPendingEnrollment|7|未注册设备以及待处理的注册。|
|unknown|8|未知设备注册状态。|



