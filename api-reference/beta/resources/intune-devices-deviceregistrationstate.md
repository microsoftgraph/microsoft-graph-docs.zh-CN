---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb7e522159df19040fcc4da3870e76b7971c95c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470676"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备注册状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notRegistered|0|设备未注册。|
|注册|双面|设备已注册。|
|吊销|第三章|设备已被阻止、已擦除或已停用。|
|keyConflict|4 |设备有键冲突。|
|approvalPending|5 |设备正在等待审批。|
|certificateReset|6 |设备证书已重置。|
|notRegisteredPendingEnrollment|7 |设备未注册且未完成注册。|
|unknown|8 |设备注册状态未知。|



