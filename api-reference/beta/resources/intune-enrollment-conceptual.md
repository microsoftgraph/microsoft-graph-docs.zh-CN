---
title: 使用 Intune 注册企业拥有的设备
description: " (BYOD) 方案。"
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07623c878ac3df9d8a171d7850868f2d7b84e56c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843937"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>使用 Intune 注册企业拥有的设备

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。 你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。

以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：

- [Active directory 的 windows 自动执行某些操作部署配置文件](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Azure AD windows 自动执行某些操作部署配置文件](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [DEP 注册基本配置文件](intune-enrollment-depenrollmentbaseprofile.md)
- [DEP 注册配置文件](intune-enrollment-depenrollmentprofile.md)
- [DEP iOS 注册配置文件](intune-enrollment-depiosenrollmentprofile.md)
- [DEP macOS 注册配置文件](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP 了员工就职状态设置](intune-enrollment-deponboardingsetting.md)
- [DEP 标记类型](intune-enrollment-deptokentype.md)
- [发现源](intune-enrollment-discoverysource.md)
- [注册配置文件](intune-enrollment-enrollmentprofile.md)
- [注册状态](intune-enrollment-enrollmentstate.md)
- [导入的 Apple 设备标识](intune-enrollment-importedappledeviceidentity.md)
- [导入 Apple 设备标识结果](intune-enrollment-importedappledeviceidentityresult.md)
- [导入的设备标识](intune-enrollment-importeddeviceidentity.md)
- [导入设备标识结果](intune-enrollment-importeddeviceidentityresult.md)
- [导入设备的标识类型](intune-enrollment-importeddeviceidentitytype.md)
- [导入的 windows 自动执行某些操作设备标识](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [导入的 windows 自动执行某些操作设备标识导入状态](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [导入的 windows 自动执行某些操作设备标识状态](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [导入的 windows 自动执行某些操作设备标识上载](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [导入的 windows 自动执行某些操作设备标识上载状态](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes 配对模式](intune-enrollment-itunespairingmode.md)
- [管理证书与指纹](intune-enrollment-managementcertificatewiththumbprint.md)
- [即开体验设置](intune-enrollment-outofboxexperiencesettings.md)
- [平台](intune-enrollment-platform.md)
- [Windows 自动执行某些操作部署配置文件](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Windows 自动执行某些操作部署配置文件分配](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [自动执行某些操作设备的 Windows 标识](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows 自动执行某些操作配置文件分配详细状态](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Windows 自动执行某些操作配置文件的工作分配状态](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows 自动执行某些操作设置](intune-enrollment-windowsautopilotsettings.md)
- [Windows 自动执行某些操作同步状态](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows 设备使用类型](intune-enrollment-windowsdeviceusagetype.md)
- [Windows 注册状态屏幕设置](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows 用户类型](intune-enrollment-windowsusertype.md)
