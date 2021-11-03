---
title: windowsAutopilotProfileAssignmentDetailedStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd81c03006349bf3401c736c092dbab25e7ca0ac
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696306"
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
|hardwareRequirementsNotMet|1|不满足硬件要求。 如果将自部署 AutoPilot 配置文件分配给没有 TPM 2.0 的设备，则可能会发生这种情况。|
|surfaceHubProfileNotSupported|2|指示将Surface Hub AutoPilot 配置文件分配给未位于 Surface Hub (的设备) 。|
|holoLensProfileNotSupported|3|指示分配HoloLens AutoPilot 配置文件的设备HoloLens。|
|windowsPcProfileNotSupported|4 |指示将Windows电脑 AutoPilot 配置文件分配给不在电脑Windows的设备。|
|surfaceHub2SProfileNotSupported|5|指示 surface Hub 2S AutoPilot 配置文件已分配给非 surface Hub 2S 的设备。|
|unknownFutureValue|99|可发展枚举的占位符，但此枚举永远不会返回给调用方，因此没有必要。|



