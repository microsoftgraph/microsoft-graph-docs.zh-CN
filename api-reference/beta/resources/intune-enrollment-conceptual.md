---
title: 使用 Intune 注册公司设备 - Microsoft Graph API
description: 列出用于 Intune 终结点的 Microsoft Graph API (为) 组织注册设备的 REST 应用程序。
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a85db8c4397659789feafa395195a39542928f01
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131951"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="444c0-103">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="444c0-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="444c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="444c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="444c0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="444c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="444c0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="444c0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="444c0-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="444c0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="444c0-108">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="444c0-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="444c0-109">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="444c0-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="444c0-110">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="444c0-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="444c0-111">Active Directory Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-111">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="444c0-112">Apple 注册配置文件分配</span><span class="sxs-lookup"><span data-stu-id="444c0-112">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="444c0-113">Apple 所有者类型注册类型</span><span class="sxs-lookup"><span data-stu-id="444c0-113">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="444c0-114">Apple 用户启动的注册配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-114">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="444c0-115">Apple 用户启动的注册类型</span><span class="sxs-lookup"><span data-stu-id="444c0-115">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="444c0-116">Azure AD Windows AutoPilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-116">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="444c0-117">已删除的 Windows Autopilot 设备状态</span><span class="sxs-lookup"><span data-stu-id="444c0-117">Deleted windows autopilot device state</span></span>](intune-enrollment-deletedwindowsautopilotdevicestate.md)
- [<span data-ttu-id="444c0-118">DEP 注册基准配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-118">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="444c0-119">DEP 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-119">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="444c0-120">DEP iOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-120">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="444c0-121">DEP macOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-121">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="444c0-122">DEP 载入设置</span><span class="sxs-lookup"><span data-stu-id="444c0-122">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="444c0-123">DEP 令牌类型</span><span class="sxs-lookup"><span data-stu-id="444c0-123">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="444c0-124">发现源</span><span class="sxs-lookup"><span data-stu-id="444c0-124">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="444c0-125">注册配置文件</span><span class="sxs-lookup"><span data-stu-id="444c0-125">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="444c0-126">已导入的 Apple 设备标识</span><span class="sxs-lookup"><span data-stu-id="444c0-126">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="444c0-127">已导入的 Apple 设备标识结果</span><span class="sxs-lookup"><span data-stu-id="444c0-127">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="444c0-128">已导入的设备标识</span><span class="sxs-lookup"><span data-stu-id="444c0-128">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="444c0-129">已导入的设备标识结果</span><span class="sxs-lookup"><span data-stu-id="444c0-129">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="444c0-130">已导入的设备标识类型</span><span class="sxs-lookup"><span data-stu-id="444c0-130">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="444c0-131">已导入的 Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="444c0-131">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="444c0-132">已导入的 Windows Autopilot 设备标识导入状态</span><span class="sxs-lookup"><span data-stu-id="444c0-132">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="444c0-133">已导入的 Windows Autopilot 设备标识状态</span><span class="sxs-lookup"><span data-stu-id="444c0-133">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="444c0-134">已导入的 Windows Autopilot 设备标识上载状态</span><span class="sxs-lookup"><span data-stu-id="444c0-134">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="444c0-135">iTunes 配对模式</span><span class="sxs-lookup"><span data-stu-id="444c0-135">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="444c0-136">带指纹的管理证书</span><span class="sxs-lookup"><span data-stu-id="444c0-136">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="444c0-137">开箱即用体验设置</span><span class="sxs-lookup"><span data-stu-id="444c0-137">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="444c0-138">平台</span><span class="sxs-lookup"><span data-stu-id="444c0-138">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="444c0-139">建议的注册限制</span><span class="sxs-lookup"><span data-stu-id="444c0-139">Suggested enrollment limit</span></span>](intune-enrollment-suggestedenrollmentlimit.md)
- [<span data-ttu-id="444c0-140">Windows Autopilot Deployment 配置文件分配</span><span class="sxs-lookup"><span data-stu-id="444c0-140">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="444c0-141">Windows Autopilot 设备删除状态</span><span class="sxs-lookup"><span data-stu-id="444c0-141">Windows autopilot device deletion state</span></span>](intune-enrollment-windowsautopilotdevicedeletionstate.md)
- [<span data-ttu-id="444c0-142">Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="444c0-142">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="444c0-143">Windows Autopilot 设备类型</span><span class="sxs-lookup"><span data-stu-id="444c0-143">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="444c0-144">Windows Autopilot 配置文件分配详细状态</span><span class="sxs-lookup"><span data-stu-id="444c0-144">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="444c0-145">Windows Autopilot 配置文件分配状态</span><span class="sxs-lookup"><span data-stu-id="444c0-145">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="444c0-146">Windows Autopilot 设置</span><span class="sxs-lookup"><span data-stu-id="444c0-146">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="444c0-147">Windows Autopilot 同步状态</span><span class="sxs-lookup"><span data-stu-id="444c0-147">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="444c0-148">Windows 设备使用类型</span><span class="sxs-lookup"><span data-stu-id="444c0-148">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="444c0-149">Windows 注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="444c0-149">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="444c0-150">Windows 用户类型</span><span class="sxs-lookup"><span data-stu-id="444c0-150">Windows user type</span></span>](intune-enrollment-windowsusertype.md)