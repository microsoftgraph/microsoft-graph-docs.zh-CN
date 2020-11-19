---
title: Microsoft Intune 中的共享资源-Microsoft Graph API
description: 列出支持租户组织的多个工作流 (REST) 的适用于 Intune 终结点的 Microsoft Graph API。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 80528f0ad7ab587e6945543e03225d112d958604
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271931"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="4622f-103">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="4622f-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="4622f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4622f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4622f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4622f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4622f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4622f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4622f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4622f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4622f-108">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="4622f-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="4622f-109">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="4622f-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="4622f-110">此外，特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="4622f-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="4622f-111">以下关系图资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="4622f-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="4622f-112">操作状态</span><span class="sxs-lookup"><span data-stu-id="4622f-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="4622f-113">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="4622f-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="4622f-114">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="4622f-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="4622f-115">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="4622f-115">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="4622f-116">Android 托管存储应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-116">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="4622f-117">证书目标存储</span><span class="sxs-lookup"><span data-stu-id="4622f-117">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="4622f-118">证书存储</span><span class="sxs-lookup"><span data-stu-id="4622f-118">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="4622f-119">证书有效期范围</span><span class="sxs-lookup"><span data-stu-id="4622f-119">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="4622f-120">公司门户操作</span><span class="sxs-lookup"><span data-stu-id="4622f-120">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="4622f-121">公司门户阻止的操作</span><span class="sxs-lookup"><span data-stu-id="4622f-121">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="4622f-122">符合性状态</span><span class="sxs-lookup"><span data-stu-id="4622f-122">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="4622f-123">设备和应用程序管理分配筛选器类型</span><span class="sxs-lookup"><span data-stu-id="4622f-123">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="4622f-124">设备和应用程序管理分配源</span><span class="sxs-lookup"><span data-stu-id="4622f-124">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="4622f-125">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="4622f-125">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="4622f-126">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="4622f-126">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="4622f-127">设备类别</span><span class="sxs-lookup"><span data-stu-id="4622f-127">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="4622f-128">设备合规性策略</span><span class="sxs-lookup"><span data-stu-id="4622f-128">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="4622f-129">设备配置</span><span class="sxs-lookup"><span data-stu-id="4622f-129">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="4622f-130">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="4622f-130">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="4622f-131">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="4622f-131">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="4622f-132">设备管理</span><span class="sxs-lookup"><span data-stu-id="4622f-132">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="4622f-133">设备管理派生的凭据设置</span><span class="sxs-lookup"><span data-stu-id="4622f-133">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="4622f-134">设备管理报告</span><span class="sxs-lookup"><span data-stu-id="4622f-134">Device management reports</span></span>](intune-shared-devicemanagementreports.md)
- [<span data-ttu-id="4622f-135">设备管理脚本</span><span class="sxs-lookup"><span data-stu-id="4622f-135">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="4622f-136">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="4622f-136">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="4622f-137">设备类型</span><span class="sxs-lookup"><span data-stu-id="4622f-137">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="4622f-138">支持</span><span class="sxs-lookup"><span data-stu-id="4622f-138">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="4622f-139">注册可用性选项</span><span class="sxs-lookup"><span data-stu-id="4622f-139">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="4622f-140">注册状态</span><span class="sxs-lookup"><span data-stu-id="4622f-140">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="4622f-141">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="4622f-141">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="4622f-142">扩展密钥用法</span><span class="sxs-lookup"><span data-stu-id="4622f-142">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="4622f-143">组分配目标</span><span class="sxs-lookup"><span data-stu-id="4622f-143">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="4622f-144">哈希算法</span><span class="sxs-lookup"><span data-stu-id="4622f-144">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="4622f-145">安装意图</span><span class="sxs-lookup"><span data-stu-id="4622f-145">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="4622f-146">iOS LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-146">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="4622f-147">iOS LOB 应用预配配置</span><span class="sxs-lookup"><span data-stu-id="4622f-147">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="4622f-148">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="4622f-148">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="4622f-149">iOS 应用商店应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-149">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="4622f-150">iOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-150">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="4622f-151">IP 范围</span><span class="sxs-lookup"><span data-stu-id="4622f-151">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="4622f-152">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="4622f-152">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="4622f-153">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="4622f-153">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="4622f-154">密钥大小</span><span class="sxs-lookup"><span data-stu-id="4622f-154">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="4622f-155">密钥存储提供程序选项</span><span class="sxs-lookup"><span data-stu-id="4622f-155">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="4622f-156">密钥使用情况</span><span class="sxs-lookup"><span data-stu-id="4622f-156">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="4622f-157">键/值对</span><span class="sxs-lookup"><span data-stu-id="4622f-157">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="4622f-158">macOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-158">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="4622f-159">托管的设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="4622f-159">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="4622f-160">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="4622f-160">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="4622f-161">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="4622f-161">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="4622f-162">适用于企业的 Microsoft 应用商店分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-162">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="4622f-163">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="4622f-163">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="4622f-164">移动应用</span><span class="sxs-lookup"><span data-stu-id="4622f-164">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="4622f-165">移动应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-165">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="4622f-166">移动应用安装时间设置</span><span class="sxs-lookup"><span data-stu-id="4622f-166">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="4622f-167">移动应用疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="4622f-167">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="4622f-168">所有者类型</span><span class="sxs-lookup"><span data-stu-id="4622f-168">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="4622f-169">策略平台类型</span><span class="sxs-lookup"><span data-stu-id="4622f-169">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="4622f-170">代理域</span><span class="sxs-lookup"><span data-stu-id="4622f-170">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="4622f-171">Report</span><span class="sxs-lookup"><span data-stu-id="4622f-171">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="4622f-172">报表根目录</span><span class="sxs-lookup"><span data-stu-id="4622f-172">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="4622f-173">生成的应用状态</span><span class="sxs-lookup"><span data-stu-id="4622f-173">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="4622f-174">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="4622f-174">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="4622f-175">按帐户类型运行</span><span class="sxs-lookup"><span data-stu-id="4622f-175">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="4622f-176">运行状态</span><span class="sxs-lookup"><span data-stu-id="4622f-176">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="4622f-177">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="4622f-177">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="4622f-178">设置源类型</span><span class="sxs-lookup"><span data-stu-id="4622f-178">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="4622f-179">使用者可选名称类型</span><span class="sxs-lookup"><span data-stu-id="4622f-179">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="4622f-180">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="4622f-180">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="4622f-181">URI</span><span class="sxs-lookup"><span data-stu-id="4622f-181">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="4622f-182">用户</span><span class="sxs-lookup"><span data-stu-id="4622f-182">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="4622f-183">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="4622f-183">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="4622f-184">VPP 令牌操作失败原因</span><span class="sxs-lookup"><span data-stu-id="4622f-184">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="4622f-185">Win32 LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-185">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="4622f-186">Win32 LOB 应用传递优化优先级</span><span class="sxs-lookup"><span data-stu-id="4622f-186">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="4622f-187">Win32 LOB 应用通知</span><span class="sxs-lookup"><span data-stu-id="4622f-187">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="4622f-188">Win32 LOB 应用重启设置</span><span class="sxs-lookup"><span data-stu-id="4622f-188">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="4622f-189">Windows AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-189">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="4622f-190">Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="4622f-190">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="4622f-191">Windows 域加入配置</span><span class="sxs-lookup"><span data-stu-id="4622f-191">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="4622f-192">Windows Universal AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="4622f-192">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="4622f-193">Windows 更新状态</span><span class="sxs-lookup"><span data-stu-id="4622f-193">Windows update state</span></span>](intune-shared-windowsupdatestate.md)