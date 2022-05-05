---
title: windowsAutopilotDeviceRemediationState 枚举类型
description: 设备修正状态，指示是否已更改已注册 Autopilot 的设备的硬件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a6220236194bdb2bfbe655359cfc1d7291d90436
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210932"
---
# <a name="windowsautopilotdeviceremediationstate-enum-type"></a>windowsAutopilotDeviceRemediationState 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备修正状态，指示是否已更改已注册 Autopilot 的设备的硬件。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知状态。|
|noRemediationRequired|1|未检测到硬件更改。|
|automaticRemediationRequired|2|客户端上检测到硬件更改。 需要其他修正。|
|manualRemediationRequired|3|客户端上检测到无法自动解析的硬件更改。 需要其他修正。|
|unknownFutureValue|4|标记已知枚举值的末尾，并允许将来使用其他值。|




