---
title: 创建 windows81GeneralConfiguration
description: 创建新的 windows81GeneralConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c56d80d1ec1a5d222ba87c0eacc548daab4d19d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957736"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="55899-103">创建 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="55899-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="55899-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55899-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55899-105">创建新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55899-105">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55899-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="55899-106">Prerequisites</span></span>
<span data-ttu-id="55899-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55899-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55899-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="55899-109">Permission type</span></span>|<span data-ttu-id="55899-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="55899-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55899-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55899-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55899-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55899-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55899-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55899-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55899-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="55899-114">Not supported.</span></span>|
|<span data-ttu-id="55899-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="55899-115">Application</span></span>|<span data-ttu-id="55899-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55899-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55899-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55899-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="55899-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="55899-118">Request headers</span></span>
|<span data-ttu-id="55899-119">标头</span><span class="sxs-lookup"><span data-stu-id="55899-119">Header</span></span>|<span data-ttu-id="55899-120">值</span><span class="sxs-lookup"><span data-stu-id="55899-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55899-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="55899-121">Authorization</span></span>|<span data-ttu-id="55899-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55899-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55899-123">接受</span><span class="sxs-lookup"><span data-stu-id="55899-123">Accept</span></span>|<span data-ttu-id="55899-124">application/json</span><span class="sxs-lookup"><span data-stu-id="55899-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55899-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="55899-125">Request body</span></span>
<span data-ttu-id="55899-126">在请求正文中，提供 windows81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55899-126">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="55899-127">下表显示了创建 windows81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="55899-127">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="55899-128">属性</span><span class="sxs-lookup"><span data-stu-id="55899-128">Property</span></span>|<span data-ttu-id="55899-129">类型</span><span class="sxs-lookup"><span data-stu-id="55899-129">Type</span></span>|<span data-ttu-id="55899-130">说明</span><span class="sxs-lookup"><span data-stu-id="55899-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55899-131">id</span><span class="sxs-lookup"><span data-stu-id="55899-131">id</span></span>|<span data-ttu-id="55899-132">String</span><span class="sxs-lookup"><span data-stu-id="55899-132">String</span></span>|<span data-ttu-id="55899-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="55899-133">Key of the entity.</span></span> <span data-ttu-id="55899-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55899-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55899-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55899-135">lastModifiedDateTime</span></span>|<span data-ttu-id="55899-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55899-136">DateTimeOffset</span></span>|<span data-ttu-id="55899-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55899-137">DateTime the object was last modified.</span></span> <span data-ttu-id="55899-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55899-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55899-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55899-139">createdDateTime</span></span>|<span data-ttu-id="55899-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55899-140">DateTimeOffset</span></span>|<span data-ttu-id="55899-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55899-141">DateTime the object was created.</span></span> <span data-ttu-id="55899-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55899-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55899-143">description</span><span class="sxs-lookup"><span data-stu-id="55899-143">description</span></span>|<span data-ttu-id="55899-144">String</span><span class="sxs-lookup"><span data-stu-id="55899-144">String</span></span>|<span data-ttu-id="55899-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="55899-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="55899-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55899-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55899-147">displayName</span><span class="sxs-lookup"><span data-stu-id="55899-147">displayName</span></span>|<span data-ttu-id="55899-148">String</span><span class="sxs-lookup"><span data-stu-id="55899-148">String</span></span>|<span data-ttu-id="55899-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="55899-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="55899-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55899-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55899-151">version</span><span class="sxs-lookup"><span data-stu-id="55899-151">version</span></span>|<span data-ttu-id="55899-152">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-152">Int32</span></span>|<span data-ttu-id="55899-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="55899-153">Version of the device configuration.</span></span> <span data-ttu-id="55899-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55899-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55899-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="55899-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="55899-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-156">Boolean</span></span>|<span data-ttu-id="55899-157">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="55899-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="55899-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="55899-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="55899-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-159">Boolean</span></span>|<span data-ttu-id="55899-160">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="55899-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="55899-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="55899-161">This property is read-only.</span></span>|
|<span data-ttu-id="55899-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="55899-162">browserBlockAutofill</span></span>|<span data-ttu-id="55899-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-163">Boolean</span></span>|<span data-ttu-id="55899-164">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="55899-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="55899-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="55899-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="55899-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-166">Boolean</span></span>|<span data-ttu-id="55899-167">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="55899-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="55899-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="55899-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="55899-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-169">Boolean</span></span>|<span data-ttu-id="55899-170">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="55899-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="55899-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="55899-171">browserBlockJavaScript</span></span>|<span data-ttu-id="55899-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-172">Boolean</span></span>|<span data-ttu-id="55899-173">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="55899-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="55899-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="55899-174">browserBlockPlugins</span></span>|<span data-ttu-id="55899-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-175">Boolean</span></span>|<span data-ttu-id="55899-176">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="55899-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="55899-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="55899-177">browserBlockPopups</span></span>|<span data-ttu-id="55899-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-178">Boolean</span></span>|<span data-ttu-id="55899-179">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="55899-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="55899-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="55899-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="55899-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-181">Boolean</span></span>|<span data-ttu-id="55899-182">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="55899-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="55899-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="55899-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="55899-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-184">Boolean</span></span>|<span data-ttu-id="55899-185">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="55899-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="55899-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="55899-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="55899-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-187">Boolean</span></span>|<span data-ttu-id="55899-188">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="55899-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="55899-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="55899-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="55899-190">String</span><span class="sxs-lookup"><span data-stu-id="55899-190">String</span></span>|<span data-ttu-id="55899-191">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="55899-191">The enterprise mode site list location.</span></span> <span data-ttu-id="55899-192">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="55899-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="55899-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55899-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="55899-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55899-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="55899-195">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="55899-195">The internet security level.</span></span> <span data-ttu-id="55899-196">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="55899-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="55899-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55899-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="55899-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55899-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="55899-199">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="55899-199">The Intranet security level.</span></span> <span data-ttu-id="55899-200">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="55899-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="55899-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="55899-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="55899-202">String</span><span class="sxs-lookup"><span data-stu-id="55899-202">String</span></span>|<span data-ttu-id="55899-203">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="55899-203">The logging report location.</span></span>|
|<span data-ttu-id="55899-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="55899-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="55899-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-205">Boolean</span></span>|<span data-ttu-id="55899-206">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="55899-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="55899-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="55899-207">browserRequireFirewall</span></span>|<span data-ttu-id="55899-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-208">Boolean</span></span>|<span data-ttu-id="55899-209">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="55899-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="55899-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="55899-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="55899-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-211">Boolean</span></span>|<span data-ttu-id="55899-212">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="55899-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="55899-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55899-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="55899-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55899-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="55899-215">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="55899-215">The trusted sites security level.</span></span> <span data-ttu-id="55899-216">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="55899-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="55899-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="55899-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="55899-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-218">Boolean</span></span>|<span data-ttu-id="55899-219">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="55899-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="55899-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="55899-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="55899-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-221">Boolean</span></span>|<span data-ttu-id="55899-222">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="55899-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="55899-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="55899-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="55899-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-224">Boolean</span></span>|<span data-ttu-id="55899-225">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="55899-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="55899-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="55899-226">passwordExpirationDays</span></span>|<span data-ttu-id="55899-227">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-227">Int32</span></span>|<span data-ttu-id="55899-228">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="55899-228">Password expiration in days.</span></span>|
|<span data-ttu-id="55899-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="55899-229">passwordMinimumLength</span></span>|<span data-ttu-id="55899-230">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-230">Int32</span></span>|<span data-ttu-id="55899-231">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="55899-231">The minimum password length.</span></span>|
|<span data-ttu-id="55899-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="55899-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="55899-233">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-233">Int32</span></span>|<span data-ttu-id="55899-234">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="55899-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="55899-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="55899-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="55899-236">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-236">Int32</span></span>|<span data-ttu-id="55899-237">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="55899-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="55899-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="55899-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="55899-239">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-239">Int32</span></span>|<span data-ttu-id="55899-240">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="55899-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="55899-241">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="55899-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="55899-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="55899-242">passwordRequiredType</span></span>|[<span data-ttu-id="55899-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="55899-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="55899-244">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="55899-244">The required password type.</span></span> <span data-ttu-id="55899-245">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="55899-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="55899-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="55899-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="55899-247">Int32</span><span class="sxs-lookup"><span data-stu-id="55899-247">Int32</span></span>|<span data-ttu-id="55899-248">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="55899-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="55899-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="55899-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="55899-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-250">Boolean</span></span>|<span data-ttu-id="55899-251">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="55899-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="55899-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="55899-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="55899-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="55899-253">Boolean</span></span>|<span data-ttu-id="55899-254">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="55899-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="55899-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="55899-255">userAccountControlSettings</span></span>|[<span data-ttu-id="55899-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="55899-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="55899-257">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="55899-257">The user account control settings.</span></span> <span data-ttu-id="55899-258">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="55899-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="55899-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="55899-259">workFoldersUrl</span></span>|<span data-ttu-id="55899-260">String</span><span class="sxs-lookup"><span data-stu-id="55899-260">String</span></span>|<span data-ttu-id="55899-261">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="55899-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="55899-262">响应</span><span class="sxs-lookup"><span data-stu-id="55899-262">Response</span></span>
<span data-ttu-id="55899-263">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55899-263">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55899-264">示例</span><span class="sxs-lookup"><span data-stu-id="55899-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="55899-265">请求</span><span class="sxs-lookup"><span data-stu-id="55899-265">Request</span></span>
<span data-ttu-id="55899-266">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55899-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55899-267">响应</span><span class="sxs-lookup"><span data-stu-id="55899-267">Response</span></span>
<span data-ttu-id="55899-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55899-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



