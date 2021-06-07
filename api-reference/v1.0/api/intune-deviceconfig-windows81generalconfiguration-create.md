---
title: 创建 windows81GeneralConfiguration
description: 创建新的 windows81GeneralConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2af1c27ac1097f7571aea1782cdd0dc4c99c2bb7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753809"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="f436a-103">创建 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="f436a-103">Create windows81GeneralConfiguration</span></span>

<span data-ttu-id="f436a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f436a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f436a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f436a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f436a-106">创建新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f436a-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f436a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f436a-107">Prerequisites</span></span>
<span data-ttu-id="f436a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f436a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f436a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f436a-110">Permission type</span></span>|<span data-ttu-id="f436a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f436a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f436a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f436a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f436a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f436a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f436a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f436a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f436a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f436a-115">Not supported.</span></span>|
|<span data-ttu-id="f436a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f436a-116">Application</span></span>|<span data-ttu-id="f436a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f436a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f436a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f436a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f436a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f436a-119">Request headers</span></span>
|<span data-ttu-id="f436a-120">标头</span><span class="sxs-lookup"><span data-stu-id="f436a-120">Header</span></span>|<span data-ttu-id="f436a-121">值</span><span class="sxs-lookup"><span data-stu-id="f436a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f436a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f436a-122">Authorization</span></span>|<span data-ttu-id="f436a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f436a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f436a-124">接受</span><span class="sxs-lookup"><span data-stu-id="f436a-124">Accept</span></span>|<span data-ttu-id="f436a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f436a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f436a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f436a-126">Request body</span></span>
<span data-ttu-id="f436a-127">在请求正文中，提供 windows81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f436a-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="f436a-128">下表显示了创建 windows81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f436a-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="f436a-129">属性</span><span class="sxs-lookup"><span data-stu-id="f436a-129">Property</span></span>|<span data-ttu-id="f436a-130">类型</span><span class="sxs-lookup"><span data-stu-id="f436a-130">Type</span></span>|<span data-ttu-id="f436a-131">说明</span><span class="sxs-lookup"><span data-stu-id="f436a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f436a-132">id</span><span class="sxs-lookup"><span data-stu-id="f436a-132">id</span></span>|<span data-ttu-id="f436a-133">String</span><span class="sxs-lookup"><span data-stu-id="f436a-133">String</span></span>|<span data-ttu-id="f436a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f436a-134">Key of the entity.</span></span> <span data-ttu-id="f436a-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f436a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f436a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f436a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f436a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f436a-137">DateTimeOffset</span></span>|<span data-ttu-id="f436a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f436a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f436a-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f436a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f436a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f436a-140">createdDateTime</span></span>|<span data-ttu-id="f436a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f436a-141">DateTimeOffset</span></span>|<span data-ttu-id="f436a-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f436a-142">DateTime the object was created.</span></span> <span data-ttu-id="f436a-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f436a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f436a-144">说明</span><span class="sxs-lookup"><span data-stu-id="f436a-144">description</span></span>|<span data-ttu-id="f436a-145">String</span><span class="sxs-lookup"><span data-stu-id="f436a-145">String</span></span>|<span data-ttu-id="f436a-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f436a-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f436a-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f436a-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f436a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f436a-148">displayName</span></span>|<span data-ttu-id="f436a-149">String</span><span class="sxs-lookup"><span data-stu-id="f436a-149">String</span></span>|<span data-ttu-id="f436a-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f436a-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f436a-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f436a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f436a-152">version</span><span class="sxs-lookup"><span data-stu-id="f436a-152">version</span></span>|<span data-ttu-id="f436a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-153">Int32</span></span>|<span data-ttu-id="f436a-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f436a-154">Version of the device configuration.</span></span> <span data-ttu-id="f436a-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f436a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f436a-156">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="f436a-156">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="f436a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-157">Boolean</span></span>|<span data-ttu-id="f436a-158">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="f436a-158">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="f436a-159">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="f436a-159">applyOnlyToWindows81</span></span>|<span data-ttu-id="f436a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-160">Boolean</span></span>|<span data-ttu-id="f436a-161">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="f436a-161">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="f436a-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f436a-162">This property is read-only.</span></span>|
|<span data-ttu-id="f436a-163">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f436a-163">browserBlockAutofill</span></span>|<span data-ttu-id="f436a-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-164">Boolean</span></span>|<span data-ttu-id="f436a-165">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="f436a-165">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="f436a-166">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="f436a-166">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="f436a-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-167">Boolean</span></span>|<span data-ttu-id="f436a-168">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="f436a-168">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="f436a-169">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="f436a-169">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="f436a-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-170">Boolean</span></span>|<span data-ttu-id="f436a-171">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="f436a-171">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="f436a-172">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="f436a-172">browserBlockJavaScript</span></span>|<span data-ttu-id="f436a-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-173">Boolean</span></span>|<span data-ttu-id="f436a-174">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="f436a-174">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="f436a-175">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="f436a-175">browserBlockPlugins</span></span>|<span data-ttu-id="f436a-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-176">Boolean</span></span>|<span data-ttu-id="f436a-177">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="f436a-177">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="f436a-178">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="f436a-178">browserBlockPopups</span></span>|<span data-ttu-id="f436a-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-179">Boolean</span></span>|<span data-ttu-id="f436a-180">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="f436a-180">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="f436a-181">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="f436a-181">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="f436a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-182">Boolean</span></span>|<span data-ttu-id="f436a-183">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="f436a-183">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="f436a-184">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="f436a-184">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="f436a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-185">Boolean</span></span>|<span data-ttu-id="f436a-186">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="f436a-186">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="f436a-187">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="f436a-187">browserRequireSmartScreen</span></span>|<span data-ttu-id="f436a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-188">Boolean</span></span>|<span data-ttu-id="f436a-189">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="f436a-189">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="f436a-190">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="f436a-190">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="f436a-191">String</span><span class="sxs-lookup"><span data-stu-id="f436a-191">String</span></span>|<span data-ttu-id="f436a-192">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="f436a-192">The enterprise mode site list location.</span></span> <span data-ttu-id="f436a-193">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="f436a-193">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="f436a-194">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f436a-194">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="f436a-195">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f436a-195">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="f436a-196">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="f436a-196">The internet security level.</span></span> <span data-ttu-id="f436a-197">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f436a-197">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="f436a-198">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f436a-198">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="f436a-199">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f436a-199">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="f436a-200">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="f436a-200">The Intranet security level.</span></span> <span data-ttu-id="f436a-201">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f436a-201">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="f436a-202">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="f436a-202">browserLoggingReportLocation</span></span>|<span data-ttu-id="f436a-203">String</span><span class="sxs-lookup"><span data-stu-id="f436a-203">String</span></span>|<span data-ttu-id="f436a-204">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="f436a-204">The logging report location.</span></span>|
|<span data-ttu-id="f436a-205">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="f436a-205">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="f436a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-206">Boolean</span></span>|<span data-ttu-id="f436a-207">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="f436a-207">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="f436a-208">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="f436a-208">browserRequireFirewall</span></span>|<span data-ttu-id="f436a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-209">Boolean</span></span>|<span data-ttu-id="f436a-210">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="f436a-210">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="f436a-211">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="f436a-211">browserRequireFraudWarning</span></span>|<span data-ttu-id="f436a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-212">Boolean</span></span>|<span data-ttu-id="f436a-213">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="f436a-213">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="f436a-214">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f436a-214">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="f436a-215">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f436a-215">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="f436a-216">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="f436a-216">The trusted sites security level.</span></span> <span data-ttu-id="f436a-217">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f436a-217">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="f436a-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="f436a-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="f436a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-219">Boolean</span></span>|<span data-ttu-id="f436a-220">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="f436a-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="f436a-221">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="f436a-221">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="f436a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-222">Boolean</span></span>|<span data-ttu-id="f436a-223">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="f436a-223">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f436a-224">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="f436a-224">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="f436a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-225">Boolean</span></span>|<span data-ttu-id="f436a-226">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="f436a-226">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="f436a-227">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f436a-227">passwordExpirationDays</span></span>|<span data-ttu-id="f436a-228">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-228">Int32</span></span>|<span data-ttu-id="f436a-229">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="f436a-229">Password expiration in days.</span></span>|
|<span data-ttu-id="f436a-230">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f436a-230">passwordMinimumLength</span></span>|<span data-ttu-id="f436a-231">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-231">Int32</span></span>|<span data-ttu-id="f436a-232">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="f436a-232">The minimum password length.</span></span>|
|<span data-ttu-id="f436a-233">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f436a-233">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f436a-234">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-234">Int32</span></span>|<span data-ttu-id="f436a-235">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="f436a-235">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f436a-236">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f436a-236">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f436a-237">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-237">Int32</span></span>|<span data-ttu-id="f436a-238">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f436a-238">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f436a-239">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f436a-239">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f436a-240">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-240">Int32</span></span>|<span data-ttu-id="f436a-241">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f436a-241">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="f436a-242">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="f436a-242">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f436a-243">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f436a-243">passwordRequiredType</span></span>|[<span data-ttu-id="f436a-244">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f436a-244">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f436a-245">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f436a-245">The required password type.</span></span> <span data-ttu-id="f436a-246">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f436a-246">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f436a-247">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f436a-247">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f436a-248">Int32</span><span class="sxs-lookup"><span data-stu-id="f436a-248">Int32</span></span>|<span data-ttu-id="f436a-249">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="f436a-249">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="f436a-250">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="f436a-250">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="f436a-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-251">Boolean</span></span>|<span data-ttu-id="f436a-252">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="f436a-252">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="f436a-253">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="f436a-253">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="f436a-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="f436a-254">Boolean</span></span>|<span data-ttu-id="f436a-255">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="f436a-255">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="f436a-256">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="f436a-256">userAccountControlSettings</span></span>|[<span data-ttu-id="f436a-257">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="f436a-257">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="f436a-258">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="f436a-258">The user account control settings.</span></span> <span data-ttu-id="f436a-259">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="f436a-259">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="f436a-260">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="f436a-260">workFoldersUrl</span></span>|<span data-ttu-id="f436a-261">String</span><span class="sxs-lookup"><span data-stu-id="f436a-261">String</span></span>|<span data-ttu-id="f436a-262">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="f436a-262">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="f436a-263">响应</span><span class="sxs-lookup"><span data-stu-id="f436a-263">Response</span></span>
<span data-ttu-id="f436a-264">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f436a-264">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f436a-265">示例</span><span class="sxs-lookup"><span data-stu-id="f436a-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="f436a-266">请求</span><span class="sxs-lookup"><span data-stu-id="f436a-266">Request</span></span>
<span data-ttu-id="f436a-267">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f436a-267">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="f436a-268">响应</span><span class="sxs-lookup"><span data-stu-id="f436a-268">Response</span></span>
<span data-ttu-id="f436a-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f436a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




