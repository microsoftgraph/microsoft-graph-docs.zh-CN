---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2543f1a7d874a8443424fa1161187e7ccd771f7b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356917"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




