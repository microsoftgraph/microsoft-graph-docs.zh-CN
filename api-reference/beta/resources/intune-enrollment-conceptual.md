---
title: 使用Intune注册公司设备 - Microsoft 图形 API
description: 列出为租户组织注册设备 (REST) Intune终结点的 Microsoft 图形 API。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
ms.openlocfilehash: 68bf3e2f220be640434be73a6dcb87a953870198
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210743"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>使用 Intune 注册企业拥有的设备

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。 你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。

以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：

- [Active Directory Windows Autopilot Deployment 配置文件](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Apple 注册配置文件分配](intune-enrollment-appleenrollmentprofileassignment.md)
- [Apple 所有者类型注册类型](intune-enrollment-appleownertypeenrollmenttype.md)
- [Apple 用户发起的注册配置文件](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [Apple 用户发起的注册类型](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [Azure AD Windows AutoPilot Deployment 配置文件](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [DEP 注册基准配置文件](intune-enrollment-depenrollmentbaseprofile.md)
- [DEP 注册配置文件](intune-enrollment-depenrollmentprofile.md)
- [DEP iOS 注册配置文件](intune-enrollment-depiosenrollmentprofile.md)
- [DEP macOS 注册配置文件](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP 载入设置](intune-enrollment-deponboardingsetting.md)
- [DEP 令牌类型](intune-enrollment-deptokentype.md)
- [设备平台类型](intune-enrollment-deviceplatformtype.md)
- [发现源](intune-enrollment-discoverysource.md)
- [注册配置文件](intune-enrollment-enrollmentprofile.md)
- [已导入的 Apple 设备标识](intune-enrollment-importedappledeviceidentity.md)
- [已导入的 Apple 设备标识结果](intune-enrollment-importedappledeviceidentityresult.md)
- [已导入的设备标识](intune-enrollment-importeddeviceidentity.md)
- [已导入的设备标识结果](intune-enrollment-importeddeviceidentityresult.md)
- [已导入的设备标识类型](intune-enrollment-importeddeviceidentitytype.md)
- [已导入的 Windows Autopilot 设备标识](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [已导入的 Windows Autopilot 设备标识导入状态](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [已导入的 Windows Autopilot 设备标识状态](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [已导入的 Windows Autopilot 设备标识上载状态](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes 配对模式](intune-enrollment-itunespairingmode.md)
- [带指纹的管理证书](intune-enrollment-managementcertificatewiththumbprint.md)
- [开箱即用体验设置](intune-enrollment-outofboxexperiencesettings.md)
- [平台](intune-enrollment-platform.md)
- [建议的注册限制](intune-enrollment-suggestedenrollmentlimit.md)
- [Windows Autopilot Deployment 配置文件分配](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Windows Autopilot 设备标识](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows autopilot 设备修正状态](intune-enrollment-windowsautopilotdeviceremediationstate.md)
- [Windows Autopilot 设备类型](intune-enrollment-windowsautopilotdevicetype.md)
- [Windows Autopilot 配置文件分配详细状态](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Windows Autopilot 配置文件分配状态](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows Autopilot 设置](intune-enrollment-windowsautopilotsettings.md)
- [Windows Autopilot 同步状态](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows 设备使用类型](intune-enrollment-windowsdeviceusagetype.md)
- [Windows 注册状态屏幕设置](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows 用户类型](intune-enrollment-windowsusertype.md)
