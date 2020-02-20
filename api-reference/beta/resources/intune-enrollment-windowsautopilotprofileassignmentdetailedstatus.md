---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 418670dd5f334b169d43022a9908c2a39f279b60
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163897"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a>windowsAutopilotProfileAssignmentDetailedStatus 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无分配详细状态|
|hardwareRequirementsNotMet|1|不满足硬件要求。 如果将自部署 AutoPilot 配置文件分配给不安装 TPM 2.0 的设备，则可能会发生这种情况。|
|surfaceHubProfileNotSupported|双面|如果 SurfaceHub AutoPilot 配置文件分配给不是 SurfaceHub 的设备，则可能会发生这种情况。|
|holoLensProfileNotSupported|第三章|如果将 HoloLens AutoPilot 配置文件分配给非 HoloLens 的设备，则可能会发生这种情况。|
|windowsPcProfileNotSupported|4|如果 WindowsPc AutoPilot 配置文件分配给不是 WindowsPc 的设备，则可能会发生这种情况。|



