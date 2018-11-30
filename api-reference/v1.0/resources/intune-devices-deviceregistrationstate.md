---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
ms.openlocfilehash: 9f9ee23d385ce4a7fca73e2d296c3f34063fc218
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008007"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备注册状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notRegistered|0|未注册设备。|
|注册|2|已注册设备。|
|吊销|3|已阻止、 擦除或停用该设备。|
|keyConflict|4|设备具有键冲突。|
|approvalPending|5|设备是待审批状态。|
|certificateReset|6|设备证书已被重置。|
|notRegisteredPendingEnrollment|7|未注册设备以及待处理的注册。|
|unknown|8|未知设备注册状态。|



