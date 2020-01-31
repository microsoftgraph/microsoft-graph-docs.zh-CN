---
title: Microsoft Intune 中的共享资源-Microsoft Graph API
description: 列出支持租户组织的多个工作流的 Intune 终结点（REST）的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: e1b613dc9140e597dc9eb0c74448f227cf940ba5
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636824"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="bd153-103">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="bd153-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="bd153-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd153-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd153-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd153-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd153-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd153-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd153-107">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="bd153-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="bd153-108">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="bd153-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="bd153-109">此外，特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="bd153-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="bd153-110">以下关系图资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="bd153-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="bd153-111">操作状态</span><span class="sxs-lookup"><span data-stu-id="bd153-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="bd153-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="bd153-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="bd153-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="bd153-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="bd153-114">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="bd153-114">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="bd153-115">BitLocker 恢复密码旋转类型</span><span class="sxs-lookup"><span data-stu-id="bd153-115">BitLocker recovery password rotation type</span></span>](intune-shared-bitlockerrecoverypasswordrotationtype.md)
- [<span data-ttu-id="bd153-116">公司门户操作</span><span class="sxs-lookup"><span data-stu-id="bd153-116">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="bd153-117">公司门户阻止的操作</span><span class="sxs-lookup"><span data-stu-id="bd153-117">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="bd153-118">符合性状态</span><span class="sxs-lookup"><span data-stu-id="bd153-118">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="bd153-119">设备和应用程序管理分配源</span><span class="sxs-lookup"><span data-stu-id="bd153-119">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="bd153-120">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="bd153-120">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="bd153-121">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="bd153-121">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="bd153-122">设备类别</span><span class="sxs-lookup"><span data-stu-id="bd153-122">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="bd153-123">设备合规性策略</span><span class="sxs-lookup"><span data-stu-id="bd153-123">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="bd153-124">设备配置</span><span class="sxs-lookup"><span data-stu-id="bd153-124">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="bd153-125">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="bd153-125">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="bd153-126">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="bd153-126">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="bd153-127">设备管理</span><span class="sxs-lookup"><span data-stu-id="bd153-127">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="bd153-128">设备管理派生的凭据颁发者</span><span class="sxs-lookup"><span data-stu-id="bd153-128">Device management derived credential issuer</span></span>](intune-shared-devicemanagementderivedcredentialissuer.md)
- [<span data-ttu-id="bd153-129">设备管理派生凭据通知类型</span><span class="sxs-lookup"><span data-stu-id="bd153-129">Device management derived credential notification type</span></span>](intune-shared-devicemanagementderivedcredentialnotificationtype.md)
- [<span data-ttu-id="bd153-130">设备管理派生的凭据设置</span><span class="sxs-lookup"><span data-stu-id="bd153-130">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="bd153-131">设备管理脚本</span><span class="sxs-lookup"><span data-stu-id="bd153-131">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="bd153-132">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="bd153-132">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="bd153-133">设备类型</span><span class="sxs-lookup"><span data-stu-id="bd153-133">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="bd153-134">支持</span><span class="sxs-lookup"><span data-stu-id="bd153-134">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="bd153-135">注册状态</span><span class="sxs-lookup"><span data-stu-id="bd153-135">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="bd153-136">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="bd153-136">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="bd153-137">组分配目标</span><span class="sxs-lookup"><span data-stu-id="bd153-137">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="bd153-138">安装意图</span><span class="sxs-lookup"><span data-stu-id="bd153-138">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="bd153-139">iOS LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-139">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="bd153-140">iOS LOB 应用预配配置</span><span class="sxs-lookup"><span data-stu-id="bd153-140">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="bd153-141">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="bd153-141">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="bd153-142">iOS 应用商店应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-142">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="bd153-143">iOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-143">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="bd153-144">IP 范围</span><span class="sxs-lookup"><span data-stu-id="bd153-144">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="bd153-145">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="bd153-145">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="bd153-146">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="bd153-146">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="bd153-147">关键字布尔值对</span><span class="sxs-lookup"><span data-stu-id="bd153-147">Key boolean value pair</span></span>](intune-shared-keybooleanvaluepair.md)
- [<span data-ttu-id="bd153-148">键整数值对</span><span class="sxs-lookup"><span data-stu-id="bd153-148">Key integer value pair</span></span>](intune-shared-keyintegervaluepair.md)
- [<span data-ttu-id="bd153-149">关键实数值对</span><span class="sxs-lookup"><span data-stu-id="bd153-149">Key real value pair</span></span>](intune-shared-keyrealvaluepair.md)
- [<span data-ttu-id="bd153-150">键字符串值对</span><span class="sxs-lookup"><span data-stu-id="bd153-150">Key string value pair</span></span>](intune-shared-keystringvaluepair.md)
- [<span data-ttu-id="bd153-151">键类型值对</span><span class="sxs-lookup"><span data-stu-id="bd153-151">Key typed value pair</span></span>](intune-shared-keytypedvaluepair.md)
- [<span data-ttu-id="bd153-152">键/值对</span><span class="sxs-lookup"><span data-stu-id="bd153-152">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="bd153-153">macOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-153">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="bd153-154">托管的设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="bd153-154">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="bd153-155">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="bd153-155">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="bd153-156">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="bd153-156">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="bd153-157">适用于企业的 Microsoft 应用商店分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-157">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="bd153-158">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="bd153-158">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="bd153-159">移动应用</span><span class="sxs-lookup"><span data-stu-id="bd153-159">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="bd153-160">移动应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-160">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="bd153-161">移动应用安装时间设置</span><span class="sxs-lookup"><span data-stu-id="bd153-161">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="bd153-162">移动应用疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="bd153-162">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="bd153-163">所有者类型</span><span class="sxs-lookup"><span data-stu-id="bd153-163">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="bd153-164">策略平台类型</span><span class="sxs-lookup"><span data-stu-id="bd153-164">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="bd153-165">代理域</span><span class="sxs-lookup"><span data-stu-id="bd153-165">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="bd153-166">Report</span><span class="sxs-lookup"><span data-stu-id="bd153-166">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="bd153-167">报表根目录</span><span class="sxs-lookup"><span data-stu-id="bd153-167">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="bd153-168">生成的应用状态</span><span class="sxs-lookup"><span data-stu-id="bd153-168">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="bd153-169">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="bd153-169">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="bd153-170">按帐户类型运行</span><span class="sxs-lookup"><span data-stu-id="bd153-170">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="bd153-171">运行状态</span><span class="sxs-lookup"><span data-stu-id="bd153-171">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="bd153-172">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="bd153-172">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="bd153-173">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="bd153-173">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="bd153-174">URI</span><span class="sxs-lookup"><span data-stu-id="bd153-174">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="bd153-175">用户</span><span class="sxs-lookup"><span data-stu-id="bd153-175">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="bd153-176">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="bd153-176">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="bd153-177">VPP 令牌操作失败原因</span><span class="sxs-lookup"><span data-stu-id="bd153-177">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="bd153-178">Win32 LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-178">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="bd153-179">Win32 LOB 应用通知</span><span class="sxs-lookup"><span data-stu-id="bd153-179">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="bd153-180">Win32 LOB 应用重启设置</span><span class="sxs-lookup"><span data-stu-id="bd153-180">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="bd153-181">Windows AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-181">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="bd153-182">Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="bd153-182">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="bd153-183">Windows 域加入配置</span><span class="sxs-lookup"><span data-stu-id="bd153-183">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="bd153-184">Windows Universal AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bd153-184">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="bd153-185">Windows 更新状态</span><span class="sxs-lookup"><span data-stu-id="bd153-185">Windows update state</span></span>](intune-shared-windowsupdatestate.md)
- [<span data-ttu-id="bd153-186">Windows 更新状态</span><span class="sxs-lookup"><span data-stu-id="bd153-186">Windows update status</span></span>](intune-shared-windowsupdatestatus.md)

