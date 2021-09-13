---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ceb929b2200c5f47b7aefd421feb1a7f19100228
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054266"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a>windowsAutopilotProfileAssignmentDetailedStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无工作分配详细状态|
|hardwareRequirementsNotMet|1|不满足硬件要求。 如果将自部署 AutoPilot 配置文件分配给没有 TPM 2.0 的设备，可能会发生这种情况。|
|surfaceHubProfileNotSupported|2|如果将 SurfaceHub AutoPilot 配置文件分配给非 SurfaceHub 的设备，可能会发生这种情况。|
|holoLensProfileNotSupported|3|如果将 AutoPilot 配置文件HoloLens分配给未分配该配置文件的设备，则可能会HoloLens。|
|windowsPcProfileNotSupported|4 |如果将 WindowsPc AutoPilot 配置文件分配给非 WindowsPc 的设备，则可能会发生这种情况。|



