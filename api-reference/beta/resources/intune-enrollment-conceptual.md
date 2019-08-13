---
title: 使用 Intune 注册企业设备-Microsoft Graph API
description: 列出为租户组织注册设备的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 506f85ae59330757f4c6f12cf80795c6678b125e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366369"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="ffb07-103">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="ffb07-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="ffb07-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ffb07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffb07-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ffb07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffb07-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffb07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb07-107">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="ffb07-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="ffb07-108">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="ffb07-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="ffb07-109">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="ffb07-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="ffb07-110">Active Directory Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ffb07-111">Azure AD Windows AutoPilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ffb07-112">DEP 注册基准配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="ffb07-113">DEP 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="ffb07-114">DEP iOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="ffb07-115">DEP macOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="ffb07-116">DEP 载入设置</span><span class="sxs-lookup"><span data-stu-id="ffb07-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="ffb07-117">DEP 令牌类型</span><span class="sxs-lookup"><span data-stu-id="ffb07-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="ffb07-118">发现源</span><span class="sxs-lookup"><span data-stu-id="ffb07-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="ffb07-119">注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="ffb07-120">注册状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="ffb07-121">已导入的 Apple 设备标识</span><span class="sxs-lookup"><span data-stu-id="ffb07-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="ffb07-122">已导入的 Apple 设备标识结果</span><span class="sxs-lookup"><span data-stu-id="ffb07-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="ffb07-123">已导入的设备标识</span><span class="sxs-lookup"><span data-stu-id="ffb07-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="ffb07-124">已导入的设备标识结果</span><span class="sxs-lookup"><span data-stu-id="ffb07-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="ffb07-125">已导入的设备标识类型</span><span class="sxs-lookup"><span data-stu-id="ffb07-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="ffb07-126">已导入的 Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="ffb07-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="ffb07-127">已导入的 Windows Autopilot 设备标识导入状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="ffb07-128">已导入的 Windows Autopilot 设备标识状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="ffb07-129">已导入的 Windows Autopilot 设备标识上载状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-129">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="ffb07-130">iTunes 配对模式</span><span class="sxs-lookup"><span data-stu-id="ffb07-130">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="ffb07-131">带指纹的管理证书</span><span class="sxs-lookup"><span data-stu-id="ffb07-131">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="ffb07-132">开箱即用体验设置</span><span class="sxs-lookup"><span data-stu-id="ffb07-132">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="ffb07-133">平台</span><span class="sxs-lookup"><span data-stu-id="ffb07-133">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="ffb07-134">Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="ffb07-134">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ffb07-135">Windows Autopilot Deployment 配置文件分配</span><span class="sxs-lookup"><span data-stu-id="ffb07-135">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="ffb07-136">Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="ffb07-136">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="ffb07-137">Windows Autopilot 设备类型</span><span class="sxs-lookup"><span data-stu-id="ffb07-137">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="ffb07-138">Windows Autopilot 配置文件分配详细状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="ffb07-139">Windows Autopilot 配置文件分配状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="ffb07-140">Windows Autopilot 设置</span><span class="sxs-lookup"><span data-stu-id="ffb07-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="ffb07-141">Windows Autopilot 同步状态</span><span class="sxs-lookup"><span data-stu-id="ffb07-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="ffb07-142">Windows 设备使用类型</span><span class="sxs-lookup"><span data-stu-id="ffb07-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="ffb07-143">Windows 注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="ffb07-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="ffb07-144">Windows 用户类型</span><span class="sxs-lookup"><span data-stu-id="ffb07-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
