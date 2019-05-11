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
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="ae0c0-103">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="ae0c0-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="ae0c0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae0c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae0c0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae0c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae0c0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ae0c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ae0c0-107">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="ae0c0-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="ae0c0-108">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="ae0c0-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="ae0c0-109">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="ae0c0-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="ae0c0-110">Active Directory Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ae0c0-111">Azure AD Windows AutoPilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ae0c0-112">DEP 注册基准配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="ae0c0-113">DEP 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="ae0c0-114">DEP iOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="ae0c0-115">DEP macOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="ae0c0-116">DEP 载入设置</span><span class="sxs-lookup"><span data-stu-id="ae0c0-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="ae0c0-117">DEP 令牌类型</span><span class="sxs-lookup"><span data-stu-id="ae0c0-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="ae0c0-118">发现源</span><span class="sxs-lookup"><span data-stu-id="ae0c0-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="ae0c0-119">注册配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="ae0c0-120">注册状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="ae0c0-121">已导入的 Apple 设备标识</span><span class="sxs-lookup"><span data-stu-id="ae0c0-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="ae0c0-122">已导入的 Apple 设备标识结果</span><span class="sxs-lookup"><span data-stu-id="ae0c0-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="ae0c0-123">已导入的设备标识</span><span class="sxs-lookup"><span data-stu-id="ae0c0-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="ae0c0-124">已导入的设备标识结果</span><span class="sxs-lookup"><span data-stu-id="ae0c0-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="ae0c0-125">已导入的设备标识类型</span><span class="sxs-lookup"><span data-stu-id="ae0c0-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="ae0c0-126">已导入的 Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="ae0c0-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="ae0c0-127">已导入的 Windows Autopilot 设备标识导入状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="ae0c0-128">已导入的 Windows Autopilot 设备标识状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="ae0c0-129">已导入的 Windows Autopilot 设备标识上载</span><span class="sxs-lookup"><span data-stu-id="ae0c0-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="ae0c0-130">已导入的 Windows Autopilot 设备标识上载状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="ae0c0-131">iTunes 配对模式</span><span class="sxs-lookup"><span data-stu-id="ae0c0-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="ae0c0-132">带指纹的管理证书</span><span class="sxs-lookup"><span data-stu-id="ae0c0-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="ae0c0-133">开箱即用体验设置</span><span class="sxs-lookup"><span data-stu-id="ae0c0-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="ae0c0-134">平台</span><span class="sxs-lookup"><span data-stu-id="ae0c0-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="ae0c0-135">Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="ae0c0-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="ae0c0-136">Windows Autopilot Deployment 配置文件分配</span><span class="sxs-lookup"><span data-stu-id="ae0c0-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="ae0c0-137">Windows Autopilot 设备标识</span><span class="sxs-lookup"><span data-stu-id="ae0c0-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="ae0c0-138">Windows Autopilot 设备类型</span><span class="sxs-lookup"><span data-stu-id="ae0c0-138">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="ae0c0-139">Windows Autopilot 配置文件分配详细状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-139">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="ae0c0-140">Windows Autopilot 配置文件分配状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-140">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="ae0c0-141">Windows Autopilot 设置</span><span class="sxs-lookup"><span data-stu-id="ae0c0-141">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="ae0c0-142">Windows Autopilot 同步状态</span><span class="sxs-lookup"><span data-stu-id="ae0c0-142">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="ae0c0-143">Windows 设备使用类型</span><span class="sxs-lookup"><span data-stu-id="ae0c0-143">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="ae0c0-144">Windows 注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="ae0c0-144">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="ae0c0-145">Windows 用户类型</span><span class="sxs-lookup"><span data-stu-id="ae0c0-145">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
