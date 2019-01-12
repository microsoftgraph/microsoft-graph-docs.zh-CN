---
title: 使用 Intune 注册企业拥有的设备
description: " (BYOD) 方案。"
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9671eb7f66be78075209906a4f6f923256afef36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928022"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="fbd20-103">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="fbd20-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="fbd20-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fbd20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbd20-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fbd20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbd20-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbd20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="fbd20-107">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="fbd20-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="fbd20-108">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="fbd20-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="fbd20-109">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="fbd20-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="fbd20-110">Active directory 的 windows 自动执行某些操作部署配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="fbd20-111">Azure AD windows 自动执行某些操作部署配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="fbd20-112">DEP 注册基本配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="fbd20-113">DEP 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="fbd20-114">DEP iOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="fbd20-115">DEP macOS 注册配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="fbd20-116">DEP 了员工就职状态设置</span><span class="sxs-lookup"><span data-stu-id="fbd20-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="fbd20-117">DEP 标记类型</span><span class="sxs-lookup"><span data-stu-id="fbd20-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="fbd20-118">发现源</span><span class="sxs-lookup"><span data-stu-id="fbd20-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="fbd20-119">注册配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="fbd20-120">注册状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="fbd20-121">导入的 Apple 设备标识</span><span class="sxs-lookup"><span data-stu-id="fbd20-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="fbd20-122">导入 Apple 设备标识结果</span><span class="sxs-lookup"><span data-stu-id="fbd20-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="fbd20-123">导入的设备标识</span><span class="sxs-lookup"><span data-stu-id="fbd20-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="fbd20-124">导入设备标识结果</span><span class="sxs-lookup"><span data-stu-id="fbd20-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="fbd20-125">导入设备的标识类型</span><span class="sxs-lookup"><span data-stu-id="fbd20-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="fbd20-126">导入的 windows 自动执行某些操作设备标识</span><span class="sxs-lookup"><span data-stu-id="fbd20-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="fbd20-127">导入的 windows 自动执行某些操作设备标识导入状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="fbd20-128">导入的 windows 自动执行某些操作设备标识状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="fbd20-129">导入的 windows 自动执行某些操作设备标识上载</span><span class="sxs-lookup"><span data-stu-id="fbd20-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="fbd20-130">导入的 windows 自动执行某些操作设备标识上载状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="fbd20-131">iTunes 配对模式</span><span class="sxs-lookup"><span data-stu-id="fbd20-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="fbd20-132">管理证书与指纹</span><span class="sxs-lookup"><span data-stu-id="fbd20-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="fbd20-133">即开体验设置</span><span class="sxs-lookup"><span data-stu-id="fbd20-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="fbd20-134">平台</span><span class="sxs-lookup"><span data-stu-id="fbd20-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="fbd20-135">Windows 自动执行某些操作部署配置文件</span><span class="sxs-lookup"><span data-stu-id="fbd20-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="fbd20-136">Windows 自动执行某些操作部署配置文件分配</span><span class="sxs-lookup"><span data-stu-id="fbd20-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="fbd20-137">自动执行某些操作设备的 Windows 标识</span><span class="sxs-lookup"><span data-stu-id="fbd20-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="fbd20-138">Windows 自动执行某些操作配置文件分配详细状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="fbd20-139">Windows 自动执行某些操作配置文件的工作分配状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="fbd20-140">Windows 自动执行某些操作设置</span><span class="sxs-lookup"><span data-stu-id="fbd20-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="fbd20-141">Windows 自动执行某些操作同步状态</span><span class="sxs-lookup"><span data-stu-id="fbd20-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="fbd20-142">Windows 设备使用类型</span><span class="sxs-lookup"><span data-stu-id="fbd20-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="fbd20-143">Windows 注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="fbd20-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="fbd20-144">Windows 用户类型</span><span class="sxs-lookup"><span data-stu-id="fbd20-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
