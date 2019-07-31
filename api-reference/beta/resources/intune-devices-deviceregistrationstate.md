---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e153ac5c1bfbd09540fd55b5df23eab095e2a002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968384"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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





