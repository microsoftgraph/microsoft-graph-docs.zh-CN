---
title: 创建 windows81GeneralConfiguration
description: 创建新的 windows81GeneralConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21f2406c5953d7aa8a46c22a7782a016a62a56b9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42737377"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="85e07-103">创建 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="85e07-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="85e07-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85e07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e07-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85e07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e07-106">创建新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85e07-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85e07-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="85e07-107">Prerequisites</span></span>
<span data-ttu-id="85e07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="85e07-110">Permission type</span></span>|<span data-ttu-id="85e07-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85e07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85e07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85e07-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e07-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85e07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85e07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="85e07-115">Not supported.</span></span>|
|<span data-ttu-id="85e07-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="85e07-116">Application</span></span>|<span data-ttu-id="85e07-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e07-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e07-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85e07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85e07-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="85e07-119">Request headers</span></span>
|<span data-ttu-id="85e07-120">标头</span><span class="sxs-lookup"><span data-stu-id="85e07-120">Header</span></span>|<span data-ttu-id="85e07-121">值</span><span class="sxs-lookup"><span data-stu-id="85e07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85e07-122">Authorization</span></span>|<span data-ttu-id="85e07-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85e07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e07-124">接受</span><span class="sxs-lookup"><span data-stu-id="85e07-124">Accept</span></span>|<span data-ttu-id="85e07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85e07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e07-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="85e07-126">Request body</span></span>
<span data-ttu-id="85e07-127">在请求正文中，提供 windows81GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85e07-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="85e07-128">下表显示了创建 windows81GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85e07-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="85e07-129">属性</span><span class="sxs-lookup"><span data-stu-id="85e07-129">Property</span></span>|<span data-ttu-id="85e07-130">类型</span><span class="sxs-lookup"><span data-stu-id="85e07-130">Type</span></span>|<span data-ttu-id="85e07-131">说明</span><span class="sxs-lookup"><span data-stu-id="85e07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e07-132">id</span><span class="sxs-lookup"><span data-stu-id="85e07-132">id</span></span>|<span data-ttu-id="85e07-133">字符串</span><span class="sxs-lookup"><span data-stu-id="85e07-133">String</span></span>|<span data-ttu-id="85e07-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="85e07-134">Key of the entity.</span></span> <span data-ttu-id="85e07-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85e07-136">lastModifiedDateTime</span></span>|<span data-ttu-id="85e07-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e07-137">DateTimeOffset</span></span>|<span data-ttu-id="85e07-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="85e07-138">DateTime the object was last modified.</span></span> <span data-ttu-id="85e07-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85e07-140">roleScopeTagIds</span></span>|<span data-ttu-id="85e07-141">String collection</span><span class="sxs-lookup"><span data-stu-id="85e07-141">String collection</span></span>|<span data-ttu-id="85e07-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="85e07-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85e07-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="85e07-144">supportsScopeTags</span></span>|<span data-ttu-id="85e07-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-145">Boolean</span></span>|<span data-ttu-id="85e07-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="85e07-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85e07-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="85e07-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85e07-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="85e07-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85e07-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="85e07-149">This property is read-only.</span></span> <span data-ttu-id="85e07-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85e07-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="85e07-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85e07-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="85e07-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="85e07-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="85e07-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85e07-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="85e07-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85e07-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="85e07-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="85e07-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="85e07-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85e07-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="85e07-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85e07-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="85e07-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="85e07-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="85e07-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85e07-163">createdDateTime</span></span>|<span data-ttu-id="85e07-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e07-164">DateTimeOffset</span></span>|<span data-ttu-id="85e07-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="85e07-165">DateTime the object was created.</span></span> <span data-ttu-id="85e07-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-167">说明</span><span class="sxs-lookup"><span data-stu-id="85e07-167">description</span></span>|<span data-ttu-id="85e07-168">String</span><span class="sxs-lookup"><span data-stu-id="85e07-168">String</span></span>|<span data-ttu-id="85e07-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="85e07-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85e07-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-171">displayName</span><span class="sxs-lookup"><span data-stu-id="85e07-171">displayName</span></span>|<span data-ttu-id="85e07-172">字符串</span><span class="sxs-lookup"><span data-stu-id="85e07-172">String</span></span>|<span data-ttu-id="85e07-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="85e07-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85e07-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-175">version</span><span class="sxs-lookup"><span data-stu-id="85e07-175">version</span></span>|<span data-ttu-id="85e07-176">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-176">Int32</span></span>|<span data-ttu-id="85e07-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="85e07-177">Version of the device configuration.</span></span> <span data-ttu-id="85e07-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e07-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e07-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="85e07-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="85e07-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-180">Boolean</span></span>|<span data-ttu-id="85e07-181">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="85e07-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="85e07-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="85e07-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="85e07-183">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-183">Boolean</span></span>|<span data-ttu-id="85e07-184">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="85e07-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="85e07-185">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="85e07-185">This property is read-only.</span></span>|
|<span data-ttu-id="85e07-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="85e07-186">browserBlockAutofill</span></span>|<span data-ttu-id="85e07-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-187">Boolean</span></span>|<span data-ttu-id="85e07-188">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="85e07-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="85e07-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="85e07-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="85e07-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-190">Boolean</span></span>|<span data-ttu-id="85e07-191">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="85e07-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="85e07-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="85e07-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="85e07-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-193">Boolean</span></span>|<span data-ttu-id="85e07-194">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="85e07-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="85e07-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="85e07-195">browserBlockJavaScript</span></span>|<span data-ttu-id="85e07-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-196">Boolean</span></span>|<span data-ttu-id="85e07-197">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="85e07-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="85e07-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="85e07-198">browserBlockPlugins</span></span>|<span data-ttu-id="85e07-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-199">Boolean</span></span>|<span data-ttu-id="85e07-200">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="85e07-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="85e07-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="85e07-201">browserBlockPopups</span></span>|<span data-ttu-id="85e07-202">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-202">Boolean</span></span>|<span data-ttu-id="85e07-203">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="85e07-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="85e07-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="85e07-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="85e07-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-205">Boolean</span></span>|<span data-ttu-id="85e07-206">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="85e07-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="85e07-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="85e07-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="85e07-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-208">Boolean</span></span>|<span data-ttu-id="85e07-209">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="85e07-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="85e07-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="85e07-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="85e07-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e07-211">Boolean</span></span>|<span data-ttu-id="85e07-212">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="85e07-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="85e07-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="85e07-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="85e07-214">String</span><span class="sxs-lookup"><span data-stu-id="85e07-214">String</span></span>|<span data-ttu-id="85e07-215">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="85e07-215">The enterprise mode site list location.</span></span> <span data-ttu-id="85e07-216">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="85e07-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="85e07-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85e07-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="85e07-218">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85e07-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="85e07-219">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="85e07-219">The internet security level.</span></span> <span data-ttu-id="85e07-220">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="85e07-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="85e07-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85e07-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="85e07-222">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85e07-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="85e07-223">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="85e07-223">The Intranet security level.</span></span> <span data-ttu-id="85e07-224">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="85e07-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="85e07-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="85e07-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="85e07-226">String</span><span class="sxs-lookup"><span data-stu-id="85e07-226">String</span></span>|<span data-ttu-id="85e07-227">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="85e07-227">The logging report location.</span></span>|
|<span data-ttu-id="85e07-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="85e07-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="85e07-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-229">Boolean</span></span>|<span data-ttu-id="85e07-230">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="85e07-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="85e07-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="85e07-231">browserRequireFirewall</span></span>|<span data-ttu-id="85e07-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-232">Boolean</span></span>|<span data-ttu-id="85e07-233">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="85e07-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="85e07-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="85e07-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="85e07-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-235">Boolean</span></span>|<span data-ttu-id="85e07-236">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="85e07-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="85e07-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85e07-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="85e07-238">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85e07-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="85e07-239">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="85e07-239">The trusted sites security level.</span></span> <span data-ttu-id="85e07-240">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="85e07-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="85e07-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="85e07-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="85e07-242">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-242">Boolean</span></span>|<span data-ttu-id="85e07-243">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="85e07-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="85e07-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="85e07-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="85e07-245">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-245">Boolean</span></span>|<span data-ttu-id="85e07-246">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="85e07-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="85e07-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="85e07-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="85e07-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-248">Boolean</span></span>|<span data-ttu-id="85e07-249">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="85e07-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="85e07-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="85e07-250">passwordExpirationDays</span></span>|<span data-ttu-id="85e07-251">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-251">Int32</span></span>|<span data-ttu-id="85e07-252">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="85e07-252">Password expiration in days.</span></span>|
|<span data-ttu-id="85e07-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="85e07-253">passwordMinimumLength</span></span>|<span data-ttu-id="85e07-254">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-254">Int32</span></span>|<span data-ttu-id="85e07-255">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="85e07-255">The minimum password length.</span></span>|
|<span data-ttu-id="85e07-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="85e07-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="85e07-257">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-257">Int32</span></span>|<span data-ttu-id="85e07-258">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="85e07-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="85e07-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="85e07-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="85e07-260">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-260">Int32</span></span>|<span data-ttu-id="85e07-261">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="85e07-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="85e07-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="85e07-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="85e07-263">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-263">Int32</span></span>|<span data-ttu-id="85e07-264">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="85e07-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="85e07-265">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="85e07-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="85e07-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="85e07-266">passwordRequiredType</span></span>|[<span data-ttu-id="85e07-267">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="85e07-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="85e07-268">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="85e07-268">The required password type.</span></span> <span data-ttu-id="85e07-269">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="85e07-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="85e07-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="85e07-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="85e07-271">Int32</span><span class="sxs-lookup"><span data-stu-id="85e07-271">Int32</span></span>|<span data-ttu-id="85e07-272">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="85e07-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="85e07-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="85e07-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="85e07-274">布尔值</span><span class="sxs-lookup"><span data-stu-id="85e07-274">Boolean</span></span>|<span data-ttu-id="85e07-275">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="85e07-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="85e07-276">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="85e07-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="85e07-277">updateClassification</span><span class="sxs-lookup"><span data-stu-id="85e07-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="85e07-278">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="85e07-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="85e07-279">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="85e07-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="85e07-280">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="85e07-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="85e07-281">updateClassification</span><span class="sxs-lookup"><span data-stu-id="85e07-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="85e07-282">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="85e07-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="85e07-283">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="85e07-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="85e07-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="85e07-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="85e07-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e07-285">Boolean</span></span>|<span data-ttu-id="85e07-286">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="85e07-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="85e07-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="85e07-287">userAccountControlSettings</span></span>|[<span data-ttu-id="85e07-288">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="85e07-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="85e07-289">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="85e07-289">The user account control settings.</span></span> <span data-ttu-id="85e07-290">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="85e07-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="85e07-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="85e07-291">workFoldersUrl</span></span>|<span data-ttu-id="85e07-292">String</span><span class="sxs-lookup"><span data-stu-id="85e07-292">String</span></span>|<span data-ttu-id="85e07-293">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="85e07-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="85e07-294">响应</span><span class="sxs-lookup"><span data-stu-id="85e07-294">Response</span></span>
<span data-ttu-id="85e07-295">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85e07-295">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e07-296">示例</span><span class="sxs-lookup"><span data-stu-id="85e07-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="85e07-297">请求</span><span class="sxs-lookup"><span data-stu-id="85e07-297">Request</span></span>
<span data-ttu-id="85e07-298">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85e07-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2697

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="85e07-299">响应</span><span class="sxs-lookup"><span data-stu-id="85e07-299">Response</span></span>
<span data-ttu-id="85e07-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85e07-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2869

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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




