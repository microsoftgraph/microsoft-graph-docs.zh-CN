---
title: Microsoft Intune 中的共享资源 - Microsoft Graph API
description: 列出适用于 Intune 终结点的 Microsoft Graph API (REST) 为租户组织支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 07f408cfc4157dd4ad415a71b19367ce0ce6ddfa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156733"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="bf4cf-103">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="bf4cf-103">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="bf4cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf4cf-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf4cf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf4cf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf4cf-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf4cf-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf4cf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf4cf-108">这些终结点在多个适用于 Intune 工作流的 Microsoft Graph API 中使用。</span><span class="sxs-lookup"><span data-stu-id="bf4cf-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="bf4cf-109">使用给定资源所需的意图、目的和权限因基础调用的特定工作流和上下文而异。</span><span class="sxs-lookup"><span data-stu-id="bf4cf-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="bf4cf-110">此外，某些方法、属性和操作仅受特定工作流支持。</span><span class="sxs-lookup"><span data-stu-id="bf4cf-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="bf4cf-111">以下 Graph 资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="bf4cf-111">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="bf4cf-112">操作状态</span><span class="sxs-lookup"><span data-stu-id="bf4cf-112">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="bf4cf-113">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="bf4cf-113">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="bf4cf-114">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="bf4cf-114">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="bf4cf-115">Android 企业始终使用 VPN 程序包类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-115">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="bf4cf-116">Android 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="bf4cf-116">Android managed app protection</span></span>](intune-shared-androidmanagedappprotection.md)
- [<span data-ttu-id="bf4cf-117">Android 托管应用商店应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-117">Android managed store app assignment settings</span></span>](intune-shared-androidmanagedstoreappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-118">证书目标存储</span><span class="sxs-lookup"><span data-stu-id="bf4cf-118">Certificate destination store</span></span>](intune-shared-certificatedestinationstore.md)
- [<span data-ttu-id="bf4cf-119">证书存储</span><span class="sxs-lookup"><span data-stu-id="bf4cf-119">Certificate store</span></span>](intune-shared-certificatestore.md)
- [<span data-ttu-id="bf4cf-120">证书有效期范围</span><span class="sxs-lookup"><span data-stu-id="bf4cf-120">Certificate validity period scale</span></span>](intune-shared-certificatevalidityperiodscale.md)
- [<span data-ttu-id="bf4cf-121">公司门户操作</span><span class="sxs-lookup"><span data-stu-id="bf4cf-121">Company portal action</span></span>](intune-shared-companyportalaction.md)
- [<span data-ttu-id="bf4cf-122">公司门户阻止的操作</span><span class="sxs-lookup"><span data-stu-id="bf4cf-122">Company portal blocked action</span></span>](intune-shared-companyportalblockedaction.md)
- [<span data-ttu-id="bf4cf-123">符合性状态</span><span class="sxs-lookup"><span data-stu-id="bf4cf-123">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="bf4cf-124">配置管理器集合分配目标</span><span class="sxs-lookup"><span data-stu-id="bf4cf-124">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="bf4cf-125">设备和应用管理分配筛选器类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-125">Device and app management assignment filter type</span></span>](intune-shared-deviceandappmanagementassignmentfiltertype.md)
- [<span data-ttu-id="bf4cf-126">设备和应用管理分配源</span><span class="sxs-lookup"><span data-stu-id="bf4cf-126">Device and app management assignment source</span></span>](intune-shared-deviceandappmanagementassignmentsource.md)
- [<span data-ttu-id="bf4cf-127">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="bf4cf-127">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="bf4cf-128">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="bf4cf-128">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="bf4cf-129">设备类别</span><span class="sxs-lookup"><span data-stu-id="bf4cf-129">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="bf4cf-130">设备合规性策略</span><span class="sxs-lookup"><span data-stu-id="bf4cf-130">Device compliance policy</span></span>](intune-shared-devicecompliancepolicy.md)
- [<span data-ttu-id="bf4cf-131">设备配置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-131">Device configuration</span></span>](intune-shared-deviceconfiguration.md)
- [<span data-ttu-id="bf4cf-132">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-132">Device enrollment configuration</span></span>](intune-shared-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="bf4cf-133">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-133">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="bf4cf-134">设备管理</span><span class="sxs-lookup"><span data-stu-id="bf4cf-134">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="bf4cf-135">设备管理派生的凭据设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-135">Device management derived credential settings</span></span>](intune-shared-devicemanagementderivedcredentialsettings.md)
- [<span data-ttu-id="bf4cf-136">设备管理报告</span><span class="sxs-lookup"><span data-stu-id="bf4cf-136">Device management reports</span></span>](intune-shared-devicemanagementreports.md)
- [<span data-ttu-id="bf4cf-137">设备管理脚本</span><span class="sxs-lookup"><span data-stu-id="bf4cf-137">Device management script</span></span>](intune-shared-devicemanagementscript.md)
- [<span data-ttu-id="bf4cf-138">设备平台类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-138">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="bf4cf-139">设备类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-139">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="bf4cf-140">支持</span><span class="sxs-lookup"><span data-stu-id="bf4cf-140">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="bf4cf-141">注册可用性选项</span><span class="sxs-lookup"><span data-stu-id="bf4cf-141">Enrollment availability options</span></span>](intune-shared-enrollmentavailabilityoptions.md)
- [<span data-ttu-id="bf4cf-142">注册状态</span><span class="sxs-lookup"><span data-stu-id="bf4cf-142">Enrollment state</span></span>](intune-shared-enrollmentstate.md)
- [<span data-ttu-id="bf4cf-143">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="bf4cf-143">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="bf4cf-144">扩展密钥用法</span><span class="sxs-lookup"><span data-stu-id="bf4cf-144">Extended key usage</span></span>](intune-shared-extendedkeyusage.md)
- [<span data-ttu-id="bf4cf-145">组分配目标</span><span class="sxs-lookup"><span data-stu-id="bf4cf-145">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="bf4cf-146">哈希算法</span><span class="sxs-lookup"><span data-stu-id="bf4cf-146">Hash algorithms</span></span>](intune-shared-hashalgorithms.md)
- [<span data-ttu-id="bf4cf-147">安装意图</span><span class="sxs-lookup"><span data-stu-id="bf4cf-147">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="bf4cf-148">iOS LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-148">iOS LOB app assignment settings</span></span>](intune-shared-ioslobappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-149">iOS LOB 应用预配配置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-149">iOS LOB app provisioning configuration</span></span>](intune-shared-ioslobappprovisioningconfiguration.md)
- [<span data-ttu-id="bf4cf-150">iOS 管理的应用保护</span><span class="sxs-lookup"><span data-stu-id="bf4cf-150">iOS managed app protection</span></span>](intune-shared-iosmanagedappprotection.md)
- [<span data-ttu-id="bf4cf-151">iOS 应用商店应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-151">iOS store app assignment settings</span></span>](intune-shared-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-152">iOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-152">iOS VPP app assignment settings</span></span>](intune-shared-iosvppappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-153">IP 范围</span><span class="sxs-lookup"><span data-stu-id="bf4cf-153">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="bf4cf-154">IPv4 范围</span><span class="sxs-lookup"><span data-stu-id="bf4cf-154">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="bf4cf-155">IPv6 范围</span><span class="sxs-lookup"><span data-stu-id="bf4cf-155">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="bf4cf-156">密钥大小</span><span class="sxs-lookup"><span data-stu-id="bf4cf-156">Key size</span></span>](intune-shared-keysize.md)
- [<span data-ttu-id="bf4cf-157">密钥存储提供程序选项</span><span class="sxs-lookup"><span data-stu-id="bf4cf-157">Key storage provider option</span></span>](intune-shared-keystorageprovideroption.md)
- [<span data-ttu-id="bf4cf-158">密钥使用情况</span><span class="sxs-lookup"><span data-stu-id="bf4cf-158">Key usages</span></span>](intune-shared-keyusages.md)
- [<span data-ttu-id="bf4cf-159">键/值对</span><span class="sxs-lookup"><span data-stu-id="bf4cf-159">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="bf4cf-160">macOS LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-160">macOS LOB app assignment settings</span></span>](intune-shared-macoslobappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-161">macOS VPP 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-161">macOS VPP app assignment settings</span></span>](intune-shared-macosvppappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-162">托管设备</span><span class="sxs-lookup"><span data-stu-id="bf4cf-162">Managed device</span></span>](intune-shared-manageddevice.md)
- [<span data-ttu-id="bf4cf-163">托管的设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-163">Managed device owner type</span></span>](intune-shared-manageddeviceownertype.md)
- [<span data-ttu-id="bf4cf-164">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-164">Management agent type</span></span>](intune-shared-managementagenttype.md)
- [<span data-ttu-id="bf4cf-165">MDM Windows 信息保护策略</span><span class="sxs-lookup"><span data-stu-id="bf4cf-165">MDM windows information protection policy</span></span>](intune-shared-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="bf4cf-166">适用于企业的 Microsoft 应用商店分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-166">Microsoft store for business app assignment settings</span></span>](intune-shared-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-167">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="bf4cf-167">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="bf4cf-168">移动应用</span><span class="sxs-lookup"><span data-stu-id="bf4cf-168">Mobile app</span></span>](intune-shared-mobileapp.md)
- [<span data-ttu-id="bf4cf-169">移动应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-169">Mobile app assignment settings</span></span>](intune-shared-mobileappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-170">移动应用安装时间设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-170">Mobile app install time settings</span></span>](intune-shared-mobileappinstalltimesettings.md)
- [<span data-ttu-id="bf4cf-171">移动应用疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="bf4cf-171">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="bf4cf-172">所有者类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-172">Owner type</span></span>](intune-shared-ownertype.md)
- [<span data-ttu-id="bf4cf-173">策略平台类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-173">Policy platform type</span></span>](intune-shared-policyplatformtype.md)
- [<span data-ttu-id="bf4cf-174">代理域</span><span class="sxs-lookup"><span data-stu-id="bf4cf-174">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="bf4cf-175">Report</span><span class="sxs-lookup"><span data-stu-id="bf4cf-175">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="bf4cf-176">报表根目录</span><span class="sxs-lookup"><span data-stu-id="bf4cf-176">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="bf4cf-177">生成的应用状态</span><span class="sxs-lookup"><span data-stu-id="bf4cf-177">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="bf4cf-178">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="bf4cf-178">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="bf4cf-179">按帐户类型运行</span><span class="sxs-lookup"><span data-stu-id="bf4cf-179">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="bf4cf-180">运行状态</span><span class="sxs-lookup"><span data-stu-id="bf4cf-180">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="bf4cf-181">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="bf4cf-181">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="bf4cf-182">设置源类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-182">Setting source type</span></span>](intune-shared-settingsourcetype.md)
- [<span data-ttu-id="bf4cf-183">使用者可选名称类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-183">Subject alternative name type</span></span>](intune-shared-subjectalternativenametype.md)
- [<span data-ttu-id="bf4cf-184">目标托管应用配置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-184">Targeted managed app configuration</span></span>](intune-shared-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="bf4cf-185">URI</span><span class="sxs-lookup"><span data-stu-id="bf4cf-185">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="bf4cf-186">"用户"</span><span class="sxs-lookup"><span data-stu-id="bf4cf-186">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="bf4cf-187">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="bf4cf-187">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="bf4cf-188">VPP 令牌操作失败原因</span><span class="sxs-lookup"><span data-stu-id="bf4cf-188">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="bf4cf-189">Win32 LOB 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-189">Win32 LOB app assignment settings</span></span>](intune-shared-win32lobappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-190">Win32 LOB 应用传递优化优先级</span><span class="sxs-lookup"><span data-stu-id="bf4cf-190">Win32 LOB app delivery optimization priority</span></span>](intune-shared-win32lobappdeliveryoptimizationpriority.md)
- [<span data-ttu-id="bf4cf-191">Win32 LOB 应用通知</span><span class="sxs-lookup"><span data-stu-id="bf4cf-191">Win32 LOB app notification</span></span>](intune-shared-win32lobappnotification.md)
- [<span data-ttu-id="bf4cf-192">Win32 LOB 应用重启设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-192">Win32 LOB app restart settings</span></span>](intune-shared-win32lobapprestartsettings.md)
- [<span data-ttu-id="bf4cf-193">Windows AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-193">Windows AppX app assignment settings</span></span>](intune-shared-windowsappxappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-194">Windows Autopilot Deployment 配置文件</span><span class="sxs-lookup"><span data-stu-id="bf4cf-194">Windows autopilot deployment profile</span></span>](intune-shared-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="bf4cf-195">Windows 域加入配置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-195">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
- [<span data-ttu-id="bf4cf-196">Windows Universal AppX 应用分配设置</span><span class="sxs-lookup"><span data-stu-id="bf4cf-196">Windows universal AppX app assignment settings</span></span>](intune-shared-windowsuniversalappxappassignmentsettings.md)
- [<span data-ttu-id="bf4cf-197">Windows 更新状态</span><span class="sxs-lookup"><span data-stu-id="bf4cf-197">Windows update state</span></span>](intune-shared-windowsupdatestate.md)