---
title: 创建 windows81GeneralConfiguration
description: 创建新的 windows81GeneralConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ec8ebea9beab335bb8d3ef6364e61564befd256
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153310"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="e7bc9-103">创建 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7bc9-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="e7bc9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7bc9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7bc9-106">创建新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7bc9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7bc9-107">Prerequisites</span></span>
<span data-ttu-id="e7bc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7bc9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7bc9-110">Permission type</span></span>|<span data-ttu-id="e7bc9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7bc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7bc9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7bc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7bc9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7bc9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7bc9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7bc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7bc9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-115">Not supported.</span></span>|
|<span data-ttu-id="e7bc9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7bc9-116">Application</span></span>|<span data-ttu-id="e7bc9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7bc9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7bc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7bc9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7bc9-119">Request headers</span></span>
|<span data-ttu-id="e7bc9-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7bc9-120">Header</span></span>|<span data-ttu-id="e7bc9-121">值</span><span class="sxs-lookup"><span data-stu-id="e7bc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7bc9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7bc9-122">Authorization</span></span>|<span data-ttu-id="e7bc9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7bc9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7bc9-124">Accept</span></span>|<span data-ttu-id="e7bc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7bc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7bc9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7bc9-126">Request body</span></span>
<span data-ttu-id="e7bc9-127">在请求正文中，提供 windows81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="e7bc9-128">下表显示了创建 windows81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="e7bc9-129">属性</span><span class="sxs-lookup"><span data-stu-id="e7bc9-129">Property</span></span>|<span data-ttu-id="e7bc9-130">类型</span><span class="sxs-lookup"><span data-stu-id="e7bc9-130">Type</span></span>|<span data-ttu-id="e7bc9-131">说明</span><span class="sxs-lookup"><span data-stu-id="e7bc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7bc9-132">id</span><span class="sxs-lookup"><span data-stu-id="e7bc9-132">id</span></span>|<span data-ttu-id="e7bc9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e7bc9-133">String</span></span>|<span data-ttu-id="e7bc9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-134">Key of the entity.</span></span> <span data-ttu-id="e7bc9-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7bc9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7bc9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bc9-137">DateTimeOffset</span></span>|<span data-ttu-id="e7bc9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7bc9-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7bc9-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7bc9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e7bc9-141">String collection</span></span>|<span data-ttu-id="e7bc9-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7bc9-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7bc9-144">supportsScopeTags</span></span>|<span data-ttu-id="e7bc9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-145">Boolean</span></span>|<span data-ttu-id="e7bc9-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7bc9-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7bc9-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7bc9-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-149">This property is read-only.</span></span> <span data-ttu-id="e7bc9-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7bc9-151">createdDateTime</span></span>|<span data-ttu-id="e7bc9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bc9-152">DateTimeOffset</span></span>|<span data-ttu-id="e7bc9-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-153">DateTime the object was created.</span></span> <span data-ttu-id="e7bc9-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-155">description</span><span class="sxs-lookup"><span data-stu-id="e7bc9-155">description</span></span>|<span data-ttu-id="e7bc9-156">字符串</span><span class="sxs-lookup"><span data-stu-id="e7bc9-156">String</span></span>|<span data-ttu-id="e7bc9-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7bc9-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e7bc9-159">displayName</span></span>|<span data-ttu-id="e7bc9-160">String</span><span class="sxs-lookup"><span data-stu-id="e7bc9-160">String</span></span>|<span data-ttu-id="e7bc9-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7bc9-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-163">version</span><span class="sxs-lookup"><span data-stu-id="e7bc9-163">version</span></span>|<span data-ttu-id="e7bc9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-164">Int32</span></span>|<span data-ttu-id="e7bc9-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-165">Version of the device configuration.</span></span> <span data-ttu-id="e7bc9-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7bc9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7bc9-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="e7bc9-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="e7bc9-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-168">Boolean</span></span>|<span data-ttu-id="e7bc9-169">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="e7bc9-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="e7bc9-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="e7bc9-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-171">Boolean</span></span>|<span data-ttu-id="e7bc9-172">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="e7bc9-173">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-173">This property is read-only.</span></span>|
|<span data-ttu-id="e7bc9-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e7bc9-174">browserBlockAutofill</span></span>|<span data-ttu-id="e7bc9-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-175">Boolean</span></span>|<span data-ttu-id="e7bc9-176">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="e7bc9-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="e7bc9-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="e7bc9-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-178">Boolean</span></span>|<span data-ttu-id="e7bc9-179">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="e7bc9-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="e7bc9-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="e7bc9-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-181">Boolean</span></span>|<span data-ttu-id="e7bc9-182">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="e7bc9-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="e7bc9-183">browserBlockJavaScript</span></span>|<span data-ttu-id="e7bc9-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-184">Boolean</span></span>|<span data-ttu-id="e7bc9-185">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="e7bc9-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="e7bc9-186">browserBlockPlugins</span></span>|<span data-ttu-id="e7bc9-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-187">Boolean</span></span>|<span data-ttu-id="e7bc9-188">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="e7bc9-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="e7bc9-189">browserBlockPopups</span></span>|<span data-ttu-id="e7bc9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-190">Boolean</span></span>|<span data-ttu-id="e7bc9-191">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="e7bc9-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="e7bc9-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="e7bc9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-193">Boolean</span></span>|<span data-ttu-id="e7bc9-194">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="e7bc9-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="e7bc9-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="e7bc9-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-196">Boolean</span></span>|<span data-ttu-id="e7bc9-197">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="e7bc9-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="e7bc9-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="e7bc9-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-199">Boolean</span></span>|<span data-ttu-id="e7bc9-200">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="e7bc9-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="e7bc9-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="e7bc9-202">String</span><span class="sxs-lookup"><span data-stu-id="e7bc9-202">String</span></span>|<span data-ttu-id="e7bc9-203">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-203">The enterprise mode site list location.</span></span> <span data-ttu-id="e7bc9-204">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="e7bc9-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e7bc9-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="e7bc9-206">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e7bc9-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="e7bc9-207">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-207">The internet security level.</span></span> <span data-ttu-id="e7bc9-208">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="e7bc9-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e7bc9-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="e7bc9-210">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e7bc9-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="e7bc9-211">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-211">The Intranet security level.</span></span> <span data-ttu-id="e7bc9-212">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="e7bc9-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="e7bc9-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="e7bc9-214">String</span><span class="sxs-lookup"><span data-stu-id="e7bc9-214">String</span></span>|<span data-ttu-id="e7bc9-215">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-215">The logging report location.</span></span>|
|<span data-ttu-id="e7bc9-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="e7bc9-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="e7bc9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-217">Boolean</span></span>|<span data-ttu-id="e7bc9-218">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="e7bc9-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="e7bc9-219">browserRequireFirewall</span></span>|<span data-ttu-id="e7bc9-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-220">Boolean</span></span>|<span data-ttu-id="e7bc9-221">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="e7bc9-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="e7bc9-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="e7bc9-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-223">Boolean</span></span>|<span data-ttu-id="e7bc9-224">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="e7bc9-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e7bc9-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="e7bc9-226">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e7bc9-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="e7bc9-227">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-227">The trusted sites security level.</span></span> <span data-ttu-id="e7bc9-228">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="e7bc9-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="e7bc9-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="e7bc9-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-230">Boolean</span></span>|<span data-ttu-id="e7bc9-231">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="e7bc9-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="e7bc9-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="e7bc9-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-233">Boolean</span></span>|<span data-ttu-id="e7bc9-234">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="e7bc9-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="e7bc9-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="e7bc9-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-236">Boolean</span></span>|<span data-ttu-id="e7bc9-237">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="e7bc9-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e7bc9-238">passwordExpirationDays</span></span>|<span data-ttu-id="e7bc9-239">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-239">Int32</span></span>|<span data-ttu-id="e7bc9-240">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-240">Password expiration in days.</span></span>|
|<span data-ttu-id="e7bc9-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e7bc9-241">passwordMinimumLength</span></span>|<span data-ttu-id="e7bc9-242">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-242">Int32</span></span>|<span data-ttu-id="e7bc9-243">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-243">The minimum password length.</span></span>|
|<span data-ttu-id="e7bc9-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e7bc9-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e7bc9-245">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-245">Int32</span></span>|<span data-ttu-id="e7bc9-246">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e7bc9-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e7bc9-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e7bc9-248">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-248">Int32</span></span>|<span data-ttu-id="e7bc9-249">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e7bc9-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e7bc9-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e7bc9-251">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-251">Int32</span></span>|<span data-ttu-id="e7bc9-252">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="e7bc9-253">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e7bc9-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e7bc9-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e7bc9-254">passwordRequiredType</span></span>|[<span data-ttu-id="e7bc9-255">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e7bc9-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e7bc9-256">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-256">The required password type.</span></span> <span data-ttu-id="e7bc9-257">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e7bc9-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e7bc9-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e7bc9-259">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bc9-259">Int32</span></span>|<span data-ttu-id="e7bc9-260">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="e7bc9-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="e7bc9-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="e7bc9-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-262">Boolean</span></span>|<span data-ttu-id="e7bc9-263">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="e7bc9-264">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="e7bc9-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="e7bc9-265">updateClassification</span><span class="sxs-lookup"><span data-stu-id="e7bc9-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="e7bc9-266">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="e7bc9-267">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="e7bc9-268">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="e7bc9-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="e7bc9-269">updateClassification</span><span class="sxs-lookup"><span data-stu-id="e7bc9-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="e7bc9-270">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="e7bc9-271">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="e7bc9-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="e7bc9-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="e7bc9-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7bc9-273">Boolean</span></span>|<span data-ttu-id="e7bc9-274">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="e7bc9-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="e7bc9-275">userAccountControlSettings</span></span>|[<span data-ttu-id="e7bc9-276">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="e7bc9-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="e7bc9-277">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-277">The user account control settings.</span></span> <span data-ttu-id="e7bc9-278">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="e7bc9-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="e7bc9-279">workFoldersUrl</span></span>|<span data-ttu-id="e7bc9-280">String</span><span class="sxs-lookup"><span data-stu-id="e7bc9-280">String</span></span>|<span data-ttu-id="e7bc9-281">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="e7bc9-282">响应</span><span class="sxs-lookup"><span data-stu-id="e7bc9-282">Response</span></span>
<span data-ttu-id="e7bc9-283">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-283">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7bc9-284">示例</span><span class="sxs-lookup"><span data-stu-id="e7bc9-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7bc9-285">请求</span><span class="sxs-lookup"><span data-stu-id="e7bc9-285">Request</span></span>
<span data-ttu-id="e7bc9-286">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1924

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="e7bc9-287">响应</span><span class="sxs-lookup"><span data-stu-id="e7bc9-287">Response</span></span>
<span data-ttu-id="e7bc9-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7bc9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




