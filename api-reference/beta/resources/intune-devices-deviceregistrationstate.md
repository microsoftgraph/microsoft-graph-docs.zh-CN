---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794013"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备注册状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notRegistered|0|设备未注册。|
|注册|双面|设备已注册。|
|吊销|第三章|设备已被阻止、已擦除或已停用。|
|keyConflict|4|设备有键冲突。|
|approvalPending|5|设备正在等待审批。|
|certificateReset|型|设备证书已重置。|
|notRegisteredPendingEnrollment|步|设备未注册且未完成注册。|
|unknown|utf-8|设备注册状态未知。|





