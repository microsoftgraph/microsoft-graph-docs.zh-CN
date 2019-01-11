---
title: 更新 windows81GeneralConfiguration
description: 更新 windows81GeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af7efc0a6c623599ad691c3fd40d71a8bbc88469
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846739"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="ddeae-103">更新 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddeae-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="ddeae-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddeae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddeae-105">更新 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ddeae-105">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddeae-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddeae-106">Prerequisites</span></span>
<span data-ttu-id="ddeae-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ddeae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddeae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddeae-109">Permission type</span></span>|<span data-ttu-id="ddeae-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddeae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddeae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddeae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddeae-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddeae-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddeae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddeae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddeae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddeae-114">Not supported.</span></span>|
|<span data-ttu-id="ddeae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddeae-115">Application</span></span>|<span data-ttu-id="ddeae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddeae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddeae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddeae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ddeae-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddeae-118">Request headers</span></span>
|<span data-ttu-id="ddeae-119">标头</span><span class="sxs-lookup"><span data-stu-id="ddeae-119">Header</span></span>|<span data-ttu-id="ddeae-120">值</span><span class="sxs-lookup"><span data-stu-id="ddeae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddeae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddeae-121">Authorization</span></span>|<span data-ttu-id="ddeae-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddeae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddeae-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ddeae-123">Accept</span></span>|<span data-ttu-id="ddeae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ddeae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddeae-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddeae-125">Request body</span></span>
<span data-ttu-id="ddeae-126">在请求正文中，提供 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddeae-126">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="ddeae-127">下表显示了创建 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddeae-127">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="ddeae-128">属性</span><span class="sxs-lookup"><span data-stu-id="ddeae-128">Property</span></span>|<span data-ttu-id="ddeae-129">类型</span><span class="sxs-lookup"><span data-stu-id="ddeae-129">Type</span></span>|<span data-ttu-id="ddeae-130">说明</span><span class="sxs-lookup"><span data-stu-id="ddeae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddeae-131">id</span><span class="sxs-lookup"><span data-stu-id="ddeae-131">id</span></span>|<span data-ttu-id="ddeae-132">String</span><span class="sxs-lookup"><span data-stu-id="ddeae-132">String</span></span>|<span data-ttu-id="ddeae-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddeae-133">Key of the entity.</span></span> <span data-ttu-id="ddeae-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddeae-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddeae-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddeae-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ddeae-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddeae-136">DateTimeOffset</span></span>|<span data-ttu-id="ddeae-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddeae-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ddeae-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddeae-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddeae-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddeae-139">createdDateTime</span></span>|<span data-ttu-id="ddeae-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddeae-140">DateTimeOffset</span></span>|<span data-ttu-id="ddeae-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddeae-141">DateTime the object was created.</span></span> <span data-ttu-id="ddeae-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddeae-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddeae-143">description</span><span class="sxs-lookup"><span data-stu-id="ddeae-143">description</span></span>|<span data-ttu-id="ddeae-144">String</span><span class="sxs-lookup"><span data-stu-id="ddeae-144">String</span></span>|<span data-ttu-id="ddeae-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddeae-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddeae-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddeae-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddeae-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ddeae-147">displayName</span></span>|<span data-ttu-id="ddeae-148">String</span><span class="sxs-lookup"><span data-stu-id="ddeae-148">String</span></span>|<span data-ttu-id="ddeae-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddeae-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddeae-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddeae-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddeae-151">version</span><span class="sxs-lookup"><span data-stu-id="ddeae-151">version</span></span>|<span data-ttu-id="ddeae-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-152">Int32</span></span>|<span data-ttu-id="ddeae-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddeae-153">Version of the device configuration.</span></span> <span data-ttu-id="ddeae-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddeae-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddeae-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="ddeae-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="ddeae-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-156">Boolean</span></span>|<span data-ttu-id="ddeae-157">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="ddeae-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="ddeae-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ddeae-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="ddeae-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-159">Boolean</span></span>|<span data-ttu-id="ddeae-160">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="ddeae-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ddeae-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ddeae-161">This property is read-only.</span></span>|
|<span data-ttu-id="ddeae-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ddeae-162">browserBlockAutofill</span></span>|<span data-ttu-id="ddeae-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-163">Boolean</span></span>|<span data-ttu-id="ddeae-164">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="ddeae-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="ddeae-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ddeae-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="ddeae-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-166">Boolean</span></span>|<span data-ttu-id="ddeae-167">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="ddeae-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="ddeae-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="ddeae-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="ddeae-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-169">Boolean</span></span>|<span data-ttu-id="ddeae-170">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="ddeae-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="ddeae-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ddeae-171">browserBlockJavaScript</span></span>|<span data-ttu-id="ddeae-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-172">Boolean</span></span>|<span data-ttu-id="ddeae-173">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="ddeae-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="ddeae-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="ddeae-174">browserBlockPlugins</span></span>|<span data-ttu-id="ddeae-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-175">Boolean</span></span>|<span data-ttu-id="ddeae-176">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="ddeae-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="ddeae-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ddeae-177">browserBlockPopups</span></span>|<span data-ttu-id="ddeae-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-178">Boolean</span></span>|<span data-ttu-id="ddeae-179">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="ddeae-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="ddeae-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="ddeae-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="ddeae-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-181">Boolean</span></span>|<span data-ttu-id="ddeae-182">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="ddeae-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="ddeae-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ddeae-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="ddeae-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-184">Boolean</span></span>|<span data-ttu-id="ddeae-185">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="ddeae-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="ddeae-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="ddeae-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="ddeae-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-187">Boolean</span></span>|<span data-ttu-id="ddeae-188">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="ddeae-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="ddeae-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="ddeae-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="ddeae-190">String</span><span class="sxs-lookup"><span data-stu-id="ddeae-190">String</span></span>|<span data-ttu-id="ddeae-191">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="ddeae-191">The enterprise mode site list location.</span></span> <span data-ttu-id="ddeae-192">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="ddeae-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="ddeae-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddeae-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="ddeae-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddeae-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="ddeae-195">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="ddeae-195">The internet security level.</span></span> <span data-ttu-id="ddeae-196">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ddeae-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ddeae-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddeae-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="ddeae-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddeae-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ddeae-199">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="ddeae-199">The Intranet security level.</span></span> <span data-ttu-id="ddeae-200">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ddeae-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ddeae-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="ddeae-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="ddeae-202">String</span><span class="sxs-lookup"><span data-stu-id="ddeae-202">String</span></span>|<span data-ttu-id="ddeae-203">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="ddeae-203">The logging report location.</span></span>|
|<span data-ttu-id="ddeae-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="ddeae-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="ddeae-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-205">Boolean</span></span>|<span data-ttu-id="ddeae-206">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="ddeae-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="ddeae-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="ddeae-207">browserRequireFirewall</span></span>|<span data-ttu-id="ddeae-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-208">Boolean</span></span>|<span data-ttu-id="ddeae-209">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="ddeae-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="ddeae-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ddeae-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="ddeae-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-211">Boolean</span></span>|<span data-ttu-id="ddeae-212">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="ddeae-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="ddeae-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddeae-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="ddeae-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ddeae-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ddeae-215">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="ddeae-215">The trusted sites security level.</span></span> <span data-ttu-id="ddeae-216">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ddeae-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ddeae-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ddeae-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ddeae-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-218">Boolean</span></span>|<span data-ttu-id="ddeae-219">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="ddeae-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ddeae-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="ddeae-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="ddeae-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-221">Boolean</span></span>|<span data-ttu-id="ddeae-222">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="ddeae-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ddeae-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="ddeae-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="ddeae-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-224">Boolean</span></span>|<span data-ttu-id="ddeae-225">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="ddeae-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="ddeae-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ddeae-226">passwordExpirationDays</span></span>|<span data-ttu-id="ddeae-227">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-227">Int32</span></span>|<span data-ttu-id="ddeae-228">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="ddeae-228">Password expiration in days.</span></span>|
|<span data-ttu-id="ddeae-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ddeae-229">passwordMinimumLength</span></span>|<span data-ttu-id="ddeae-230">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-230">Int32</span></span>|<span data-ttu-id="ddeae-231">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="ddeae-231">The minimum password length.</span></span>|
|<span data-ttu-id="ddeae-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ddeae-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ddeae-233">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-233">Int32</span></span>|<span data-ttu-id="ddeae-234">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="ddeae-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ddeae-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ddeae-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ddeae-236">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-236">Int32</span></span>|<span data-ttu-id="ddeae-237">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="ddeae-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ddeae-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ddeae-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ddeae-239">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-239">Int32</span></span>|<span data-ttu-id="ddeae-240">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="ddeae-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="ddeae-241">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="ddeae-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ddeae-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ddeae-242">passwordRequiredType</span></span>|[<span data-ttu-id="ddeae-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ddeae-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ddeae-244">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="ddeae-244">The required password type.</span></span> <span data-ttu-id="ddeae-245">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="ddeae-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ddeae-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ddeae-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ddeae-247">Int32</span><span class="sxs-lookup"><span data-stu-id="ddeae-247">Int32</span></span>|<span data-ttu-id="ddeae-248">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="ddeae-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="ddeae-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="ddeae-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="ddeae-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-250">Boolean</span></span>|<span data-ttu-id="ddeae-251">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="ddeae-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="ddeae-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="ddeae-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="ddeae-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddeae-253">Boolean</span></span>|<span data-ttu-id="ddeae-254">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="ddeae-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="ddeae-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ddeae-255">userAccountControlSettings</span></span>|[<span data-ttu-id="ddeae-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ddeae-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="ddeae-257">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="ddeae-257">The user account control settings.</span></span> <span data-ttu-id="ddeae-258">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="ddeae-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="ddeae-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="ddeae-259">workFoldersUrl</span></span>|<span data-ttu-id="ddeae-260">String</span><span class="sxs-lookup"><span data-stu-id="ddeae-260">String</span></span>|<span data-ttu-id="ddeae-261">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="ddeae-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="ddeae-262">响应</span><span class="sxs-lookup"><span data-stu-id="ddeae-262">Response</span></span>
<span data-ttu-id="ddeae-263">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddeae-263">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddeae-264">示例</span><span class="sxs-lookup"><span data-stu-id="ddeae-264">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddeae-265">请求</span><span class="sxs-lookup"><span data-stu-id="ddeae-265">Request</span></span>
<span data-ttu-id="ddeae-266">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddeae-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ddeae-267">响应</span><span class="sxs-lookup"><span data-stu-id="ddeae-267">Response</span></span>
<span data-ttu-id="ddeae-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddeae-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



