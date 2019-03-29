---
title: 更新 windows81GeneralConfiguration
description: 更新 windows81GeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc1ef5d0935290a8056c06dfcd4df6281417827e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984581"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="b9574-103">更新 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9574-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="b9574-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9574-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9574-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9574-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9574-106">更新 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9574-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9574-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9574-107">Prerequisites</span></span>
<span data-ttu-id="b9574-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9574-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9574-110">Permission type</span></span>|<span data-ttu-id="b9574-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9574-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9574-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9574-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9574-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9574-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9574-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9574-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9574-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9574-115">Not supported.</span></span>|
|<span data-ttu-id="b9574-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9574-116">Application</span></span>|<span data-ttu-id="b9574-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9574-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9574-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9574-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b9574-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9574-119">Request headers</span></span>
|<span data-ttu-id="b9574-120">标头</span><span class="sxs-lookup"><span data-stu-id="b9574-120">Header</span></span>|<span data-ttu-id="b9574-121">值</span><span class="sxs-lookup"><span data-stu-id="b9574-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9574-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9574-122">Authorization</span></span>|<span data-ttu-id="b9574-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9574-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9574-124">接受</span><span class="sxs-lookup"><span data-stu-id="b9574-124">Accept</span></span>|<span data-ttu-id="b9574-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9574-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9574-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9574-126">Request body</span></span>
<span data-ttu-id="b9574-127">在请求正文中，提供 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9574-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="b9574-128">下表显示了创建 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b9574-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="b9574-129">属性</span><span class="sxs-lookup"><span data-stu-id="b9574-129">Property</span></span>|<span data-ttu-id="b9574-130">类型</span><span class="sxs-lookup"><span data-stu-id="b9574-130">Type</span></span>|<span data-ttu-id="b9574-131">说明</span><span class="sxs-lookup"><span data-stu-id="b9574-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9574-132">id</span><span class="sxs-lookup"><span data-stu-id="b9574-132">id</span></span>|<span data-ttu-id="b9574-133">String</span><span class="sxs-lookup"><span data-stu-id="b9574-133">String</span></span>|<span data-ttu-id="b9574-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b9574-134">Key of the entity.</span></span> <span data-ttu-id="b9574-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9574-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b9574-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9574-137">DateTimeOffset</span></span>|<span data-ttu-id="b9574-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b9574-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b9574-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9574-140">roleScopeTagIds</span></span>|<span data-ttu-id="b9574-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9574-141">String collection</span></span>|<span data-ttu-id="b9574-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b9574-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9574-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9574-144">supportsScopeTags</span></span>|<span data-ttu-id="b9574-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-145">Boolean</span></span>|<span data-ttu-id="b9574-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b9574-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b9574-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b9574-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b9574-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b9574-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b9574-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b9574-149">This property is read-only.</span></span> <span data-ttu-id="b9574-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9574-151">createdDateTime</span></span>|<span data-ttu-id="b9574-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9574-152">DateTimeOffset</span></span>|<span data-ttu-id="b9574-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b9574-153">DateTime the object was created.</span></span> <span data-ttu-id="b9574-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-155">description</span><span class="sxs-lookup"><span data-stu-id="b9574-155">description</span></span>|<span data-ttu-id="b9574-156">String</span><span class="sxs-lookup"><span data-stu-id="b9574-156">String</span></span>|<span data-ttu-id="b9574-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b9574-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9574-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b9574-159">displayName</span></span>|<span data-ttu-id="b9574-160">String</span><span class="sxs-lookup"><span data-stu-id="b9574-160">String</span></span>|<span data-ttu-id="b9574-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b9574-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9574-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-163">version</span><span class="sxs-lookup"><span data-stu-id="b9574-163">version</span></span>|<span data-ttu-id="b9574-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-164">Int32</span></span>|<span data-ttu-id="b9574-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b9574-165">Version of the device configuration.</span></span> <span data-ttu-id="b9574-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9574-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9574-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b9574-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b9574-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-168">Boolean</span></span>|<span data-ttu-id="b9574-169">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="b9574-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b9574-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b9574-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="b9574-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-171">Boolean</span></span>|<span data-ttu-id="b9574-172">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="b9574-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b9574-173">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b9574-173">This property is read-only.</span></span>|
|<span data-ttu-id="b9574-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b9574-174">browserBlockAutofill</span></span>|<span data-ttu-id="b9574-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-175">Boolean</span></span>|<span data-ttu-id="b9574-176">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="b9574-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b9574-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b9574-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="b9574-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-178">Boolean</span></span>|<span data-ttu-id="b9574-179">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="b9574-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="b9574-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="b9574-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="b9574-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-181">Boolean</span></span>|<span data-ttu-id="b9574-182">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="b9574-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="b9574-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b9574-183">browserBlockJavaScript</span></span>|<span data-ttu-id="b9574-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-184">Boolean</span></span>|<span data-ttu-id="b9574-185">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="b9574-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b9574-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="b9574-186">browserBlockPlugins</span></span>|<span data-ttu-id="b9574-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-187">Boolean</span></span>|<span data-ttu-id="b9574-188">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="b9574-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="b9574-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b9574-189">browserBlockPopups</span></span>|<span data-ttu-id="b9574-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-190">Boolean</span></span>|<span data-ttu-id="b9574-191">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b9574-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b9574-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b9574-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b9574-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-193">Boolean</span></span>|<span data-ttu-id="b9574-194">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="b9574-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b9574-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b9574-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="b9574-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-196">Boolean</span></span>|<span data-ttu-id="b9574-197">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="b9574-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="b9574-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b9574-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="b9574-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-199">Boolean</span></span>|<span data-ttu-id="b9574-200">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="b9574-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b9574-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b9574-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b9574-202">String</span><span class="sxs-lookup"><span data-stu-id="b9574-202">String</span></span>|<span data-ttu-id="b9574-203">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="b9574-203">The enterprise mode site list location.</span></span> <span data-ttu-id="b9574-204">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b9574-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b9574-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9574-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="b9574-206">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9574-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="b9574-207">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="b9574-207">The internet security level.</span></span> <span data-ttu-id="b9574-208">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="b9574-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b9574-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9574-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="b9574-210">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9574-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b9574-211">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="b9574-211">The Intranet security level.</span></span> <span data-ttu-id="b9574-212">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="b9574-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b9574-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="b9574-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="b9574-214">String</span><span class="sxs-lookup"><span data-stu-id="b9574-214">String</span></span>|<span data-ttu-id="b9574-215">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="b9574-215">The logging report location.</span></span>|
|<span data-ttu-id="b9574-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="b9574-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="b9574-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-217">Boolean</span></span>|<span data-ttu-id="b9574-218">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="b9574-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="b9574-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="b9574-219">browserRequireFirewall</span></span>|<span data-ttu-id="b9574-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-220">Boolean</span></span>|<span data-ttu-id="b9574-221">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="b9574-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="b9574-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b9574-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="b9574-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-223">Boolean</span></span>|<span data-ttu-id="b9574-224">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="b9574-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="b9574-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9574-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="b9574-226">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9574-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b9574-227">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="b9574-227">The trusted sites security level.</span></span> <span data-ttu-id="b9574-228">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="b9574-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b9574-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b9574-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b9574-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-230">Boolean</span></span>|<span data-ttu-id="b9574-231">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="b9574-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b9574-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="b9574-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="b9574-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-233">Boolean</span></span>|<span data-ttu-id="b9574-234">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="b9574-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b9574-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="b9574-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="b9574-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-236">Boolean</span></span>|<span data-ttu-id="b9574-237">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="b9574-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="b9574-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b9574-238">passwordExpirationDays</span></span>|<span data-ttu-id="b9574-239">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-239">Int32</span></span>|<span data-ttu-id="b9574-240">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="b9574-240">Password expiration in days.</span></span>|
|<span data-ttu-id="b9574-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b9574-241">passwordMinimumLength</span></span>|<span data-ttu-id="b9574-242">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-242">Int32</span></span>|<span data-ttu-id="b9574-243">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="b9574-243">The minimum password length.</span></span>|
|<span data-ttu-id="b9574-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b9574-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b9574-245">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-245">Int32</span></span>|<span data-ttu-id="b9574-246">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b9574-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b9574-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b9574-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b9574-248">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-248">Int32</span></span>|<span data-ttu-id="b9574-249">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b9574-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b9574-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b9574-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b9574-251">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-251">Int32</span></span>|<span data-ttu-id="b9574-252">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b9574-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b9574-253">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="b9574-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b9574-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b9574-254">passwordRequiredType</span></span>|[<span data-ttu-id="b9574-255">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b9574-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b9574-256">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b9574-256">The required password type.</span></span> <span data-ttu-id="b9574-257">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b9574-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b9574-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b9574-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b9574-259">Int32</span><span class="sxs-lookup"><span data-stu-id="b9574-259">Int32</span></span>|<span data-ttu-id="b9574-260">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="b9574-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="b9574-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b9574-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="b9574-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-262">Boolean</span></span>|<span data-ttu-id="b9574-263">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="b9574-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b9574-264">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="b9574-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="b9574-265">updateClassification</span><span class="sxs-lookup"><span data-stu-id="b9574-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="b9574-266">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="b9574-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="b9574-267">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b9574-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="b9574-268">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="b9574-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="b9574-269">updateClassification</span><span class="sxs-lookup"><span data-stu-id="b9574-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="b9574-270">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="b9574-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="b9574-271">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b9574-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="b9574-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="b9574-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="b9574-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9574-273">Boolean</span></span>|<span data-ttu-id="b9574-274">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="b9574-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="b9574-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b9574-275">userAccountControlSettings</span></span>|[<span data-ttu-id="b9574-276">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b9574-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="b9574-277">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="b9574-277">The user account control settings.</span></span> <span data-ttu-id="b9574-278">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="b9574-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="b9574-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="b9574-279">workFoldersUrl</span></span>|<span data-ttu-id="b9574-280">String</span><span class="sxs-lookup"><span data-stu-id="b9574-280">String</span></span>|<span data-ttu-id="b9574-281">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="b9574-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="b9574-282">响应</span><span class="sxs-lookup"><span data-stu-id="b9574-282">Response</span></span>
<span data-ttu-id="b9574-283">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9574-283">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9574-284">示例</span><span class="sxs-lookup"><span data-stu-id="b9574-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9574-285">请求</span><span class="sxs-lookup"><span data-stu-id="b9574-285">Request</span></span>
<span data-ttu-id="b9574-286">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9574-286">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="b9574-287">响应</span><span class="sxs-lookup"><span data-stu-id="b9574-287">Response</span></span>
<span data-ttu-id="b9574-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9574-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




