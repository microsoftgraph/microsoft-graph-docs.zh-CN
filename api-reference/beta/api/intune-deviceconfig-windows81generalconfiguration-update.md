---
title: 更新 windows81GeneralConfiguration
description: 更新 windows81GeneralConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a59e89f01723fe1555641c9a00678fbdfa0a0ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477194"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="4efb9-103">更新 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4efb9-103">Update windows81GeneralConfiguration</span></span>

<span data-ttu-id="4efb9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4efb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4efb9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4efb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4efb9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4efb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4efb9-107">更新 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4efb9-107">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4efb9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4efb9-108">Prerequisites</span></span>
<span data-ttu-id="4efb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4efb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4efb9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4efb9-111">Permission type</span></span>|<span data-ttu-id="4efb9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4efb9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4efb9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4efb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4efb9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efb9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4efb9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4efb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4efb9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4efb9-116">Not supported.</span></span>|
|<span data-ttu-id="4efb9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4efb9-117">Application</span></span>|<span data-ttu-id="4efb9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efb9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4efb9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4efb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4efb9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4efb9-120">Request headers</span></span>
|<span data-ttu-id="4efb9-121">标头</span><span class="sxs-lookup"><span data-stu-id="4efb9-121">Header</span></span>|<span data-ttu-id="4efb9-122">值</span><span class="sxs-lookup"><span data-stu-id="4efb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4efb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4efb9-123">Authorization</span></span>|<span data-ttu-id="4efb9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4efb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4efb9-125">接受</span><span class="sxs-lookup"><span data-stu-id="4efb9-125">Accept</span></span>|<span data-ttu-id="4efb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4efb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4efb9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4efb9-127">Request body</span></span>
<span data-ttu-id="4efb9-128">在请求正文中，提供 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4efb9-128">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="4efb9-129">下表显示了创建 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4efb9-129">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="4efb9-130">属性</span><span class="sxs-lookup"><span data-stu-id="4efb9-130">Property</span></span>|<span data-ttu-id="4efb9-131">类型</span><span class="sxs-lookup"><span data-stu-id="4efb9-131">Type</span></span>|<span data-ttu-id="4efb9-132">说明</span><span class="sxs-lookup"><span data-stu-id="4efb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4efb9-133">id</span><span class="sxs-lookup"><span data-stu-id="4efb9-133">id</span></span>|<span data-ttu-id="4efb9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4efb9-134">String</span></span>|<span data-ttu-id="4efb9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4efb9-135">Key of the entity.</span></span> <span data-ttu-id="4efb9-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4efb9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4efb9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4efb9-138">DateTimeOffset</span></span>|<span data-ttu-id="4efb9-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4efb9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4efb9-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4efb9-141">roleScopeTagIds</span></span>|<span data-ttu-id="4efb9-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="4efb9-142">String collection</span></span>|<span data-ttu-id="4efb9-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4efb9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4efb9-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4efb9-145">supportsScopeTags</span></span>|<span data-ttu-id="4efb9-146">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-146">Boolean</span></span>|<span data-ttu-id="4efb9-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4efb9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4efb9-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4efb9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4efb9-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4efb9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4efb9-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4efb9-150">This property is read-only.</span></span> <span data-ttu-id="4efb9-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4efb9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4efb9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4efb9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4efb9-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4efb9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4efb9-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4efb9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4efb9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4efb9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4efb9-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4efb9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4efb9-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4efb9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4efb9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4efb9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4efb9-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4efb9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4efb9-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4efb9-164">createdDateTime</span></span>|<span data-ttu-id="4efb9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4efb9-165">DateTimeOffset</span></span>|<span data-ttu-id="4efb9-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4efb9-166">DateTime the object was created.</span></span> <span data-ttu-id="4efb9-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-168">说明</span><span class="sxs-lookup"><span data-stu-id="4efb9-168">description</span></span>|<span data-ttu-id="4efb9-169">String</span><span class="sxs-lookup"><span data-stu-id="4efb9-169">String</span></span>|<span data-ttu-id="4efb9-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4efb9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4efb9-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4efb9-172">displayName</span></span>|<span data-ttu-id="4efb9-173">字符串</span><span class="sxs-lookup"><span data-stu-id="4efb9-173">String</span></span>|<span data-ttu-id="4efb9-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4efb9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4efb9-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-176">version</span><span class="sxs-lookup"><span data-stu-id="4efb9-176">version</span></span>|<span data-ttu-id="4efb9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-177">Int32</span></span>|<span data-ttu-id="4efb9-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4efb9-178">Version of the device configuration.</span></span> <span data-ttu-id="4efb9-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4efb9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4efb9-180">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="4efb9-180">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="4efb9-181">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-181">Boolean</span></span>|<span data-ttu-id="4efb9-182">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="4efb9-182">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="4efb9-183">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="4efb9-183">applyOnlyToWindows81</span></span>|<span data-ttu-id="4efb9-184">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-184">Boolean</span></span>|<span data-ttu-id="4efb9-185">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="4efb9-185">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4efb9-186">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4efb9-186">This property is read-only.</span></span>|
|<span data-ttu-id="4efb9-187">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="4efb9-187">browserBlockAutofill</span></span>|<span data-ttu-id="4efb9-188">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-188">Boolean</span></span>|<span data-ttu-id="4efb9-189">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="4efb9-189">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="4efb9-190">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="4efb9-190">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="4efb9-191">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-191">Boolean</span></span>|<span data-ttu-id="4efb9-192">指示是否阻止自动检测 Intranet 站点。</span><span class="sxs-lookup"><span data-stu-id="4efb9-192">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="4efb9-193">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="4efb9-193">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="4efb9-194">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-194">Boolean</span></span>|<span data-ttu-id="4efb9-195">指示是否阻止企业模式访问。</span><span class="sxs-lookup"><span data-stu-id="4efb9-195">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="4efb9-196">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="4efb9-196">browserBlockJavaScript</span></span>|<span data-ttu-id="4efb9-197">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-197">Boolean</span></span>|<span data-ttu-id="4efb9-198">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="4efb9-198">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="4efb9-199">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="4efb9-199">browserBlockPlugins</span></span>|<span data-ttu-id="4efb9-200">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-200">Boolean</span></span>|<span data-ttu-id="4efb9-201">指示是否阻止插件。</span><span class="sxs-lookup"><span data-stu-id="4efb9-201">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="4efb9-202">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="4efb9-202">browserBlockPopups</span></span>|<span data-ttu-id="4efb9-203">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-203">Boolean</span></span>|<span data-ttu-id="4efb9-204">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="4efb9-204">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="4efb9-205">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="4efb9-205">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="4efb9-206">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-206">Boolean</span></span>|<span data-ttu-id="4efb9-207">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="4efb9-207">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="4efb9-208">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="4efb9-208">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="4efb9-209">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-209">Boolean</span></span>|<span data-ttu-id="4efb9-210">指示是否阻止在 Intranet 站点上使用单字条目。</span><span class="sxs-lookup"><span data-stu-id="4efb9-210">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="4efb9-211">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="4efb9-211">browserRequireSmartScreen</span></span>|<span data-ttu-id="4efb9-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4efb9-212">Boolean</span></span>|<span data-ttu-id="4efb9-213">指示是否要求用户使用智能屏幕筛选器。</span><span class="sxs-lookup"><span data-stu-id="4efb9-213">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="4efb9-214">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="4efb9-214">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="4efb9-215">String</span><span class="sxs-lookup"><span data-stu-id="4efb9-215">String</span></span>|<span data-ttu-id="4efb9-216">企业模式网站列表位置。</span><span class="sxs-lookup"><span data-stu-id="4efb9-216">The enterprise mode site list location.</span></span> <span data-ttu-id="4efb9-217">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="4efb9-217">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="4efb9-218">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4efb9-218">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="4efb9-219">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4efb9-219">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="4efb9-220">Internet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="4efb9-220">The internet security level.</span></span> <span data-ttu-id="4efb9-221">可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-221">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4efb9-222">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4efb9-222">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="4efb9-223">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4efb9-223">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="4efb9-224">Intranet 安全级别。</span><span class="sxs-lookup"><span data-stu-id="4efb9-224">The Intranet security level.</span></span> <span data-ttu-id="4efb9-225">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-225">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4efb9-226">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="4efb9-226">browserLoggingReportLocation</span></span>|<span data-ttu-id="4efb9-227">String</span><span class="sxs-lookup"><span data-stu-id="4efb9-227">String</span></span>|<span data-ttu-id="4efb9-228">日志记录报表位置。</span><span class="sxs-lookup"><span data-stu-id="4efb9-228">The logging report location.</span></span>|
|<span data-ttu-id="4efb9-229">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="4efb9-229">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="4efb9-230">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-230">Boolean</span></span>|<span data-ttu-id="4efb9-231">指示是否要求受限站点具有高安全性。</span><span class="sxs-lookup"><span data-stu-id="4efb9-231">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="4efb9-232">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="4efb9-232">browserRequireFirewall</span></span>|<span data-ttu-id="4efb9-233">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-233">Boolean</span></span>|<span data-ttu-id="4efb9-234">指示是否需要防火墙。</span><span class="sxs-lookup"><span data-stu-id="4efb9-234">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="4efb9-235">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="4efb9-235">browserRequireFraudWarning</span></span>|<span data-ttu-id="4efb9-236">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-236">Boolean</span></span>|<span data-ttu-id="4efb9-237">指示是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="4efb9-237">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="4efb9-238">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4efb9-238">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="4efb9-239">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4efb9-239">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="4efb9-240">受信任的站点安全级别。</span><span class="sxs-lookup"><span data-stu-id="4efb9-240">The trusted sites security level.</span></span> <span data-ttu-id="4efb9-241">可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-241">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4efb9-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="4efb9-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="4efb9-243">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-243">Boolean</span></span>|<span data-ttu-id="4efb9-244">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="4efb9-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="4efb9-245">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="4efb9-245">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="4efb9-246">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-246">Boolean</span></span>|<span data-ttu-id="4efb9-247">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="4efb9-247">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4efb9-248">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="4efb9-248">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="4efb9-249">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-249">Boolean</span></span>|<span data-ttu-id="4efb9-250">指示是否阻止用户使用图片密码和 PIN。</span><span class="sxs-lookup"><span data-stu-id="4efb9-250">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="4efb9-251">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4efb9-251">passwordExpirationDays</span></span>|<span data-ttu-id="4efb9-252">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-252">Int32</span></span>|<span data-ttu-id="4efb9-253">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="4efb9-253">Password expiration in days.</span></span>|
|<span data-ttu-id="4efb9-254">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4efb9-254">passwordMinimumLength</span></span>|<span data-ttu-id="4efb9-255">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-255">Int32</span></span>|<span data-ttu-id="4efb9-256">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="4efb9-256">The minimum password length.</span></span>|
|<span data-ttu-id="4efb9-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4efb9-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4efb9-258">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-258">Int32</span></span>|<span data-ttu-id="4efb9-259">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4efb9-259">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4efb9-260">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4efb9-260">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4efb9-261">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-261">Int32</span></span>|<span data-ttu-id="4efb9-262">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="4efb9-262">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4efb9-263">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4efb9-263">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4efb9-264">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-264">Int32</span></span>|<span data-ttu-id="4efb9-265">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4efb9-265">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="4efb9-266">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="4efb9-266">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4efb9-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4efb9-267">passwordRequiredType</span></span>|[<span data-ttu-id="4efb9-268">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4efb9-268">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4efb9-269">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4efb9-269">The required password type.</span></span> <span data-ttu-id="4efb9-270">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-270">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4efb9-271">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4efb9-271">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4efb9-272">Int32</span><span class="sxs-lookup"><span data-stu-id="4efb9-272">Int32</span></span>|<span data-ttu-id="4efb9-273">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="4efb9-273">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="4efb9-274">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="4efb9-274">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="4efb9-275">布尔</span><span class="sxs-lookup"><span data-stu-id="4efb9-275">Boolean</span></span>|<span data-ttu-id="4efb9-276">指示是否要求对移动设备加密。</span><span class="sxs-lookup"><span data-stu-id="4efb9-276">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="4efb9-277">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="4efb9-277">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="4efb9-278">updateClassification</span><span class="sxs-lookup"><span data-stu-id="4efb9-278">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="4efb9-279">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="4efb9-279">The minimum update classification to install automatically.</span></span> <span data-ttu-id="4efb9-280">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-280">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="4efb9-281">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="4efb9-281">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="4efb9-282">updateClassification</span><span class="sxs-lookup"><span data-stu-id="4efb9-282">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="4efb9-283">自动安装的最小更新分类。</span><span class="sxs-lookup"><span data-stu-id="4efb9-283">The minimum update classification to install automatically.</span></span> <span data-ttu-id="4efb9-284">可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-284">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="4efb9-285">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="4efb9-285">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="4efb9-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="4efb9-286">Boolean</span></span>|<span data-ttu-id="4efb9-287">指示是否需要自动更新。</span><span class="sxs-lookup"><span data-stu-id="4efb9-287">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="4efb9-288">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="4efb9-288">userAccountControlSettings</span></span>|[<span data-ttu-id="4efb9-289">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="4efb9-289">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="4efb9-290">用户帐户控制设置。</span><span class="sxs-lookup"><span data-stu-id="4efb9-290">The user account control settings.</span></span> <span data-ttu-id="4efb9-291">可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。</span><span class="sxs-lookup"><span data-stu-id="4efb9-291">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="4efb9-292">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="4efb9-292">workFoldersUrl</span></span>|<span data-ttu-id="4efb9-293">String</span><span class="sxs-lookup"><span data-stu-id="4efb9-293">String</span></span>|<span data-ttu-id="4efb9-294">工作文件夹 URL。</span><span class="sxs-lookup"><span data-stu-id="4efb9-294">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="4efb9-295">响应</span><span class="sxs-lookup"><span data-stu-id="4efb9-295">Response</span></span>
<span data-ttu-id="4efb9-296">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4efb9-296">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4efb9-297">示例</span><span class="sxs-lookup"><span data-stu-id="4efb9-297">Example</span></span>

### <a name="request"></a><span data-ttu-id="4efb9-298">请求</span><span class="sxs-lookup"><span data-stu-id="4efb9-298">Request</span></span>
<span data-ttu-id="4efb9-299">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4efb9-299">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4efb9-300">响应</span><span class="sxs-lookup"><span data-stu-id="4efb9-300">Response</span></span>
<span data-ttu-id="4efb9-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4efb9-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





