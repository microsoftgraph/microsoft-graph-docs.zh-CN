---
title: 使用 Intune 注册企业设备-Microsoft Graph API
description: 列出为租户组织注册设备的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d456863ec39479d113299d741470c48323aa4616
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941595"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>使用 Intune 注册企业拥有的设备

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。 你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。

以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：

- [Active Directory Windows Autopilot Deployment 配置文件](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Azure AD Windows AutoPilot Deployment 配置文件](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [DEP 注册基准配置文件](intune-enrollment-depenrollmentbaseprofile.md)
- [DEP 注册配置文件](intune-enrollment-depenrollmentprofile.md)
- [DEP iOS 注册配置文件](intune-enrollment-depiosenrollmentprofile.md)
- [DEP macOS 注册配置文件](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP 载入设置](intune-enrollment-deponboardingsetting.md)
- [DEP 令牌类型](intune-enrollment-deptokentype.md)
- [发现源](intune-enrollment-discoverysource.md)
- [注册配置文件](intune-enrollment-enrollmentprofile.md)
- [注册状态](intune-enrollment-enrollmentstate.md)
- [已导入的 Apple 设备标识](intune-enrollment-importedappledeviceidentity.md)
- [已导入的 Apple 设备标识结果](intune-enrollment-importedappledeviceidentityresult.md)
- [已导入的设备标识](intune-enrollment-importeddeviceidentity.md)
- [已导入的设备标识结果](intune-enrollment-importeddeviceidentityresult.md)
- [已导入的设备标识类型](intune-enrollment-importeddeviceidentitytype.md)
- [已导入的 Windows Autopilot 设备标识](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [已导入的 Windows Autopilot 设备标识导入状态](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [已导入的 Windows Autopilot 设备标识状态](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [已导入的 Windows Autopilot 设备标识上载](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [已导入的 Windows Autopilot 设备标识上载状态](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes 配对模式](intune-enrollment-itunespairingmode.md)
- [带指纹的管理证书](intune-enrollment-managementcertificatewiththumbprint.md)
- [开箱即用体验设置](intune-enrollment-outofboxexperiencesettings.md)
- [平台](intune-enrollment-platform.md)
- [Windows Autopilot Deployment 配置文件](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Windows Autopilot Deployment 配置文件分配](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Windows Autopilot 设备标识](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows Autopilot 设备类型](intune-enrollment-windowsautopilotdevicetype.md)
- [Windows Autopilot 配置文件分配详细状态](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Windows Autopilot 配置文件分配状态](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows Autopilot 设置](intune-enrollment-windowsautopilotsettings.md)
- [Windows Autopilot 同步状态](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows 设备使用类型](intune-enrollment-windowsdeviceusagetype.md)
- [Windows 注册状态屏幕设置](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows 用户类型](intune-enrollment-windowsusertype.md)
