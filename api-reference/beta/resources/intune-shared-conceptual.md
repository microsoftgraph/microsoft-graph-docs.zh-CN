---
title: Microsoft Intune 中的共享资源-Microsoft Graph API
description: 列出支持租户组织的多个工作流的 Intune 终结点（REST）的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 007b118334c57397c2ec5b66e9d7acfc9cb42775
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088271"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="c3929-103">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="c3929-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="c3929-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c3929-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3929-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3929-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3929-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3929-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3929-107">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="c3929-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="c3929-108">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="c3929-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="c3929-109">此外，特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="c3929-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="c3929-110">以下关系图资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="c3929-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="c3929-111">操作状态</span><span class="sxs-lookup"><span data-stu-id="c3929-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="c3929-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="c3929-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="c3929-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="c3929-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="c3929-114">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="c3929-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="c3929-115">公司门户操作</span><span class="sxs-lookup"><span data-stu-id="c3929-115">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="c3929-116">公司门户阻止的操作</span><span class="sxs-lookup"><span data-stu-id="c3929-116">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="c3929-117">符合性状态</span><span class="sxs-lookup"><span data-stu-id="c3929-117">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="c3929-118">设备和应用程序管理分配源</span><span class="sxs-lookup"><span data-stu-id="c3929-118">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="c3929-119">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="c3929-119">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="c3929-120">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="c3929-120">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="c3929-121">设备类别</span><span class="sxs-lookup"><span data-stu-id="c3929-121">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="c3929-122">设备合规性策略</span><span class="sxs-lookup"><span data-stu-id="c3929-122">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="c3929-123">设备配置</span><span class="sxs-lookup"><span data-stu-id="c3929-123">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="c3929-124">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="c3929-124">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="c3929-125">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="c3929-125">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="c3929-126">设备管理</span><span class="sxs-lookup"><span data-stu-id="c3929-126">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="c3929-127">设备管理派生的凭据颁发者</span><span class="sxs-lookup"><span data-stu-id="c3929-127">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="c3929-128">设备管理派生凭据通知类型</span><span class="sxs-lookup"><span data-stu-id="c3929-128">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="c3929-129">设备管理派生的凭据设置</span><span class="sxs-lookup"><span data-stu-id="c3929-129">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="c3929-130">设备管理脚本</span><span class="sxs-lookup"><span data-stu-id="c3929-130">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="c3929-131">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="c3929-131">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="c3929-132">设备类型</span><span class="sxs-lookup"><span data-stu-id="c3929-132">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="c3929-133">支持</span><span class="sxs-lookup"><span data-stu-id="c3929-133">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="c3929-134">注册状态</span><span class="sxs-lookup"><span data-stu-id="c3929-134">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="c3929-135">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="c3929-135">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="c3929-136">组分配目标</span><span class="sxs-lookup"><span data-stu-id="c3929-136">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="c3929-137">安装意图</span><span class="sxs-lookup"><span data-stu-id="c3929-137">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="c3929-138">iOS LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-138">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="c3929-139">iOS LOB 应用预配配置</span><span class="sxs-lookup"><span data-stu-id="c3929-139">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="c3929-140">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="c3929-140">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="c3929-141">iOS 应用商店应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-141">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="c3929-142">iOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-142">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="c3929-143">IP 范围</span><span class="sxs-lookup"><span data-stu-id="c3929-143">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="c3929-144">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="c3929-144">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="c3929-145">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="c3929-145">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="c3929-146">键/值对</span><span class="sxs-lookup"><span data-stu-id="c3929-146">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="c3929-147">macOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-147">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="c3929-148">托管的设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="c3929-148">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="c3929-149">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="c3929-149">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="c3929-150">适用于企业的 Microsoft 应用商店分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-150">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="c3929-151">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="c3929-151">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="c3929-152">移动应用</span><span class="sxs-lookup"><span data-stu-id="c3929-152">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="c3929-153">移动应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-153">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="c3929-154">移动应用安装时间设置</span><span class="sxs-lookup"><span data-stu-id="c3929-154">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="c3929-155">移动应用疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="c3929-155">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="c3929-156">所有者类型</span><span class="sxs-lookup"><span data-stu-id="c3929-156">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="c3929-157">策略平台类型</span><span class="sxs-lookup"><span data-stu-id="c3929-157">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="c3929-158">代理域</span><span class="sxs-lookup"><span data-stu-id="c3929-158">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="c3929-159">Report</span><span class="sxs-lookup"><span data-stu-id="c3929-159">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="c3929-160">报表根目录</span><span class="sxs-lookup"><span data-stu-id="c3929-160">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="c3929-161">生成的应用状态</span><span class="sxs-lookup"><span data-stu-id="c3929-161">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="c3929-162">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="c3929-162">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="c3929-163">按帐户类型运行</span><span class="sxs-lookup"><span data-stu-id="c3929-163">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="c3929-164">运行状态</span><span class="sxs-lookup"><span data-stu-id="c3929-164">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="c3929-165">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="c3929-165">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="c3929-166">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="c3929-166">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="c3929-167">URI</span><span class="sxs-lookup"><span data-stu-id="c3929-167">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="c3929-168">用户</span><span class="sxs-lookup"><span data-stu-id="c3929-168">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="c3929-169">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="c3929-169">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="c3929-170">VPP 令牌操作失败原因</span><span class="sxs-lookup"><span data-stu-id="c3929-170">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="c3929-171">Win32 LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-171">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="c3929-172">Win32 LOB 应用通知</span><span class="sxs-lookup"><span data-stu-id="c3929-172">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="c3929-173">Win32 LOB 应用重启设置</span><span class="sxs-lookup"><span data-stu-id="c3929-173">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="c3929-174">Windows AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-174">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="c3929-175">Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="c3929-175">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="c3929-176">Windows 域加入配置</span><span class="sxs-lookup"><span data-stu-id="c3929-176">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="c3929-177">Windows Universal AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="c3929-177">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="c3929-178">Windows 更新状态</span><span class="sxs-lookup"><span data-stu-id="c3929-178">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="c3929-179">Windows 更新状态</span><span class="sxs-lookup"><span data-stu-id="c3929-179">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

