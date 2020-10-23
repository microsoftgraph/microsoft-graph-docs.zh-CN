---
title: 使用 Intune 注册企业设备-Microsoft Graph API
description: 列出为租户组织注册设备 (REST) 的适用于 Intune 终结点的 Microsoft Graph API。
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e8e1a03f5194b5790ba68c10dad8eae23a706945
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735237"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="07997-103">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="07997-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="07997-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07997-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07997-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="07997-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07997-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="07997-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07997-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07997-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07997-108">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="07997-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="07997-109">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="07997-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="07997-110">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="07997-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="07997-111">Active Directory Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-111">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="07997-112">Apple 注册配置文件分配</span><span class="sxs-lookup"><span data-stu-id="07997-112">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="07997-113">Apple 所有者类型注册类型</span><span class="sxs-lookup"><span data-stu-id="07997-113">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="07997-114">Apple 用户启动的注册配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-114">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="07997-115">Apple 用户启动的注册类型</span><span class="sxs-lookup"><span data-stu-id="07997-115">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="07997-116">Azure AD Windows AutoPilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-116">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="07997-117">DEP 注册基准配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-117">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="07997-118">DEP 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-118">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="07997-119">DEP iOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-119">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="07997-120">DEP macOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-120">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="07997-121">DEP 载入设置</span><span class="sxs-lookup"><span data-stu-id="07997-121">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="07997-122">DEP 令牌类型</span><span class="sxs-lookup"><span data-stu-id="07997-122">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="07997-123">发现源</span><span class="sxs-lookup"><span data-stu-id="07997-123">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="07997-124">注册配置文件</span><span class="sxs-lookup"><span data-stu-id="07997-124">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="07997-125">已导入的 Apple 设备标识</span><span class="sxs-lookup"><span data-stu-id="07997-125">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="07997-126">已导入的 Apple 设备标识结果</span><span class="sxs-lookup"><span data-stu-id="07997-126">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="07997-127">已导入的设备标识</span><span class="sxs-lookup"><span data-stu-id="07997-127">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="07997-128">已导入的设备标识结果</span><span class="sxs-lookup"><span data-stu-id="07997-128">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="07997-129">已导入的设备标识类型</span><span class="sxs-lookup"><span data-stu-id="07997-129">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="07997-130">已导入的 Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="07997-130">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="07997-131">已导入的 Windows Autopilot 设备标识导入状态</span><span class="sxs-lookup"><span data-stu-id="07997-131">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="07997-132">已导入的 Windows Autopilot 设备标识状态</span><span class="sxs-lookup"><span data-stu-id="07997-132">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="07997-133">已导入的 Windows Autopilot 设备标识上载状态</span><span class="sxs-lookup"><span data-stu-id="07997-133">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="07997-134">iTunes 配对模式</span><span class="sxs-lookup"><span data-stu-id="07997-134">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="07997-135">带指纹的管理证书</span><span class="sxs-lookup"><span data-stu-id="07997-135">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="07997-136">开箱即用体验设置</span><span class="sxs-lookup"><span data-stu-id="07997-136">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="07997-137">平台</span><span class="sxs-lookup"><span data-stu-id="07997-137">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="07997-138">建议的注册限制</span><span class="sxs-lookup"><span data-stu-id="07997-138">Suggested enrollment limit</span></span>](intune-enrollment-suggestedenrollmentlimit.md)
- [<span data-ttu-id="07997-139">Windows Autopilot Deployment 配置文件分配</span><span class="sxs-lookup"><span data-stu-id="07997-139">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="07997-140">Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="07997-140">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="07997-141">Windows Autopilot 设备类型</span><span class="sxs-lookup"><span data-stu-id="07997-141">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="07997-142">Windows Autopilot 配置文件分配详细状态</span><span class="sxs-lookup"><span data-stu-id="07997-142">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="07997-143">Windows Autopilot 配置文件分配状态</span><span class="sxs-lookup"><span data-stu-id="07997-143">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="07997-144">Windows Autopilot 设置</span><span class="sxs-lookup"><span data-stu-id="07997-144">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="07997-145">Windows Autopilot 同步状态</span><span class="sxs-lookup"><span data-stu-id="07997-145">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="07997-146">Windows 设备使用类型</span><span class="sxs-lookup"><span data-stu-id="07997-146">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="07997-147">Windows 注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="07997-147">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="07997-148">Windows 用户类型</span><span class="sxs-lookup"><span data-stu-id="07997-148">Windows user type</span></span>](intune-enrollment-windowsusertype.md)