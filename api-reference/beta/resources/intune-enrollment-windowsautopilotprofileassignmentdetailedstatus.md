---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 542f9191452077194092955f35b0e5fb332ae05d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728912"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a>windowsAutopilotProfileAssignmentDetailedStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无分配详细状态|
|hardwareRequirementsNotMet|1|不满足硬件要求。 如果将自部署 AutoPilot 配置文件分配给不安装 TPM 2.0 的设备，则可能会发生这种情况。|
|surfaceHubProfileNotSupported|双面|如果 SurfaceHub AutoPilot 配置文件分配给不是 SurfaceHub 的设备，则可能会发生这种情况。|
|holoLensProfileNotSupported|第三章|如果将 HoloLens AutoPilot 配置文件分配给非 HoloLens 的设备，则可能会发生这种情况。|
|windowsPcProfileNotSupported|4 |如果 WindowsPc AutoPilot 配置文件分配给不是 WindowsPc 的设备，则可能会发生这种情况。|





