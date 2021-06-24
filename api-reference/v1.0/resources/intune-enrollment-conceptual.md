---
title: 使用 Intune 注册公司设备 - Microsoft Graph API
description: 列出为租户Graph注册设备的适用于 Intune (REST) 的 Microsoft Graph API。
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daefbf23d8aa70cdd3f81fdcb4afb69dd2590ba7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108935"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>使用 Intune 注册企业拥有的设备

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。 你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。

以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：

- [设备管理](intune-enrollment-devicemanagement.md)
- [注册状态](intune-enrollment-enrollmentstate.md)
- [已导入的 Windows Autopilot 设备标识](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [已导入的 Windows Autopilot 设备标识导入状态](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [已导入的 Windows Autopilot 设备标识状态](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [已导入的 Windows Autopilot 设备标识上载状态](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [Windows Autopilot 设备标识](intune-enrollment-windowsautopilotdeviceidentity.md)