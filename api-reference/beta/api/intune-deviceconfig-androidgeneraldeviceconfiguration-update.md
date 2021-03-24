---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8db51e97f79ac6e8dbe32236dd80d3dcff3307b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138034"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="9be63-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9be63-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="9be63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9be63-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9be63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9be63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9be63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9be63-107">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9be63-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9be63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9be63-108">Prerequisites</span></span>
<span data-ttu-id="9be63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9be63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9be63-111">Permission type</span></span>|<span data-ttu-id="9be63-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9be63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9be63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9be63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9be63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9be63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9be63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9be63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9be63-116">Not supported.</span></span>|
|<span data-ttu-id="9be63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9be63-117">Application</span></span>|<span data-ttu-id="9be63-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be63-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9be63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9be63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9be63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9be63-120">Request headers</span></span>
|<span data-ttu-id="9be63-121">标头</span><span class="sxs-lookup"><span data-stu-id="9be63-121">Header</span></span>|<span data-ttu-id="9be63-122">值</span><span class="sxs-lookup"><span data-stu-id="9be63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9be63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9be63-123">Authorization</span></span>|<span data-ttu-id="9be63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9be63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9be63-125">接受</span><span class="sxs-lookup"><span data-stu-id="9be63-125">Accept</span></span>|<span data-ttu-id="9be63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9be63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9be63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9be63-127">Request body</span></span>
<span data-ttu-id="9be63-128">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9be63-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="9be63-129">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9be63-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="9be63-130">属性</span><span class="sxs-lookup"><span data-stu-id="9be63-130">Property</span></span>|<span data-ttu-id="9be63-131">类型</span><span class="sxs-lookup"><span data-stu-id="9be63-131">Type</span></span>|<span data-ttu-id="9be63-132">说明</span><span class="sxs-lookup"><span data-stu-id="9be63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9be63-133">id</span><span class="sxs-lookup"><span data-stu-id="9be63-133">id</span></span>|<span data-ttu-id="9be63-134">String</span><span class="sxs-lookup"><span data-stu-id="9be63-134">String</span></span>|<span data-ttu-id="9be63-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9be63-135">Key of the entity.</span></span> <span data-ttu-id="9be63-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9be63-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9be63-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9be63-138">DateTimeOffset</span></span>|<span data-ttu-id="9be63-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9be63-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9be63-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9be63-141">roleScopeTagIds</span></span>|<span data-ttu-id="9be63-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9be63-142">String collection</span></span>|<span data-ttu-id="9be63-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9be63-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9be63-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9be63-145">supportsScopeTags</span></span>|<span data-ttu-id="9be63-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-146">Boolean</span></span>|<span data-ttu-id="9be63-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="9be63-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9be63-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="9be63-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9be63-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="9be63-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9be63-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9be63-150">This property is read-only.</span></span> <span data-ttu-id="9be63-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9be63-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9be63-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9be63-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9be63-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="9be63-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9be63-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9be63-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9be63-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9be63-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9be63-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9be63-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9be63-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9be63-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9be63-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9be63-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9be63-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9be63-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9be63-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9be63-164">createdDateTime</span></span>|<span data-ttu-id="9be63-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9be63-165">DateTimeOffset</span></span>|<span data-ttu-id="9be63-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9be63-166">DateTime the object was created.</span></span> <span data-ttu-id="9be63-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-168">说明</span><span class="sxs-lookup"><span data-stu-id="9be63-168">description</span></span>|<span data-ttu-id="9be63-169">String</span><span class="sxs-lookup"><span data-stu-id="9be63-169">String</span></span>|<span data-ttu-id="9be63-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9be63-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9be63-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9be63-172">displayName</span></span>|<span data-ttu-id="9be63-173">String</span><span class="sxs-lookup"><span data-stu-id="9be63-173">String</span></span>|<span data-ttu-id="9be63-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9be63-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9be63-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-176">version</span><span class="sxs-lookup"><span data-stu-id="9be63-176">version</span></span>|<span data-ttu-id="9be63-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9be63-177">Int32</span></span>|<span data-ttu-id="9be63-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9be63-178">Version of the device configuration.</span></span> <span data-ttu-id="9be63-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9be63-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9be63-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="9be63-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="9be63-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-181">Boolean</span></span>|<span data-ttu-id="9be63-182">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="9be63-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="9be63-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="9be63-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="9be63-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-184">Boolean</span></span>|<span data-ttu-id="9be63-185">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="9be63-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="9be63-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="9be63-186">appsBlockYouTube</span></span>|<span data-ttu-id="9be63-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-187">Boolean</span></span>|<span data-ttu-id="9be63-188">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="9be63-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="9be63-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-189">bluetoothBlocked</span></span>|<span data-ttu-id="9be63-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-190">Boolean</span></span>|<span data-ttu-id="9be63-191">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="9be63-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="9be63-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-192">cameraBlocked</span></span>|<span data-ttu-id="9be63-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-193">Boolean</span></span>|<span data-ttu-id="9be63-194">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="9be63-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="9be63-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="9be63-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="9be63-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-196">Boolean</span></span>|<span data-ttu-id="9be63-197">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="9be63-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="9be63-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="9be63-198">cellularBlockMessaging</span></span>|<span data-ttu-id="9be63-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-199">Boolean</span></span>|<span data-ttu-id="9be63-200">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="9be63-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="9be63-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="9be63-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="9be63-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-202">Boolean</span></span>|<span data-ttu-id="9be63-203">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="9be63-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="9be63-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="9be63-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="9be63-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-205">Boolean</span></span>|<span data-ttu-id="9be63-206">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="9be63-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="9be63-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="9be63-207">compliantAppsList</span></span>|<span data-ttu-id="9be63-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9be63-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9be63-209">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="9be63-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="9be63-210">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="9be63-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9be63-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="9be63-211">compliantAppListType</span></span>|[<span data-ttu-id="9be63-212">appListType</span><span class="sxs-lookup"><span data-stu-id="9be63-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9be63-213">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="9be63-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="9be63-214">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="9be63-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9be63-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="9be63-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="9be63-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-216">Boolean</span></span>|<span data-ttu-id="9be63-217">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="9be63-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9be63-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-218">locationServicesBlocked</span></span>|<span data-ttu-id="9be63-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-219">Boolean</span></span>|<span data-ttu-id="9be63-220">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="9be63-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="9be63-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="9be63-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="9be63-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-222">Boolean</span></span>|<span data-ttu-id="9be63-223">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="9be63-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="9be63-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="9be63-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-225">Boolean</span></span>|<span data-ttu-id="9be63-226">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="9be63-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="9be63-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="9be63-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="9be63-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-228">Boolean</span></span>|<span data-ttu-id="9be63-229">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="9be63-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="9be63-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="9be63-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="9be63-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-231">Boolean</span></span>|<span data-ttu-id="9be63-232">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="9be63-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="9be63-233">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="9be63-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="9be63-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-234">Boolean</span></span>|<span data-ttu-id="9be63-235">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9be63-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="9be63-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="9be63-236">kioskModeApps</span></span>|<span data-ttu-id="9be63-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9be63-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9be63-238">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="9be63-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="9be63-239">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9be63-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9be63-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-240">nfcBlocked</span></span>|<span data-ttu-id="9be63-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-241">Boolean</span></span>|<span data-ttu-id="9be63-242">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="9be63-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="9be63-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="9be63-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="9be63-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-244">Boolean</span></span>|<span data-ttu-id="9be63-245">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="9be63-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="9be63-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="9be63-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="9be63-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-247">Boolean</span></span>|<span data-ttu-id="9be63-248">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="9be63-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="9be63-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9be63-249">passwordExpirationDays</span></span>|<span data-ttu-id="9be63-250">Int32</span><span class="sxs-lookup"><span data-stu-id="9be63-250">Int32</span></span>|<span data-ttu-id="9be63-251">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="9be63-251">Number of days before the password expires.</span></span> <span data-ttu-id="9be63-252">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="9be63-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9be63-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9be63-253">passwordMinimumLength</span></span>|<span data-ttu-id="9be63-254">Int32</span><span class="sxs-lookup"><span data-stu-id="9be63-254">Int32</span></span>|<span data-ttu-id="9be63-255">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9be63-255">Minimum length of passwords.</span></span> <span data-ttu-id="9be63-256">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="9be63-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9be63-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9be63-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9be63-258">Int32</span><span class="sxs-lookup"><span data-stu-id="9be63-258">Int32</span></span>|<span data-ttu-id="9be63-259">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="9be63-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9be63-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9be63-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9be63-261">Int32</span><span class="sxs-lookup"><span data-stu-id="9be63-261">Int32</span></span>|<span data-ttu-id="9be63-262">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="9be63-262">Number of previous passwords to block.</span></span> <span data-ttu-id="9be63-263">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="9be63-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9be63-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9be63-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9be63-265">Int32</span><span class="sxs-lookup"><span data-stu-id="9be63-265">Int32</span></span>|<span data-ttu-id="9be63-266">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="9be63-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="9be63-267">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="9be63-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9be63-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9be63-268">passwordRequiredType</span></span>|[<span data-ttu-id="9be63-269">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9be63-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="9be63-270">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9be63-270">Type of password that is required.</span></span> <span data-ttu-id="9be63-271">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="9be63-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="9be63-272">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="9be63-272">requiredPasswordComplexity</span></span>|[<span data-ttu-id="9be63-273">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="9be63-273">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="9be63-274">指示 Android 上所需的密码复杂性。</span><span class="sxs-lookup"><span data-stu-id="9be63-274">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="9be63-275">其中一个：NONE、LOW、MEDIUM、HIGH。</span><span class="sxs-lookup"><span data-stu-id="9be63-275">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="9be63-276">这是面向 Android 11+的 API。</span><span class="sxs-lookup"><span data-stu-id="9be63-276">This is an API targeted to Android 11+.</span></span> <span data-ttu-id="9be63-277">可取值为：`none`、`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="9be63-277">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="9be63-278">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9be63-278">passwordRequired</span></span>|<span data-ttu-id="9be63-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-279">Boolean</span></span>|<span data-ttu-id="9be63-280">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="9be63-280">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="9be63-281">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-281">powerOffBlocked</span></span>|<span data-ttu-id="9be63-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-282">Boolean</span></span>|<span data-ttu-id="9be63-283">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="9be63-283">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="9be63-284">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-284">factoryResetBlocked</span></span>|<span data-ttu-id="9be63-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-285">Boolean</span></span>|<span data-ttu-id="9be63-286">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="9be63-286">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="9be63-287">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-287">screenCaptureBlocked</span></span>|<span data-ttu-id="9be63-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-288">Boolean</span></span>|<span data-ttu-id="9be63-289">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="9be63-289">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="9be63-290">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="9be63-290">deviceSharingAllowed</span></span>|<span data-ttu-id="9be63-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-291">Boolean</span></span>|<span data-ttu-id="9be63-292">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="9be63-292">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="9be63-293">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="9be63-293">storageBlockGoogleBackup</span></span>|<span data-ttu-id="9be63-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-294">Boolean</span></span>|<span data-ttu-id="9be63-295">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="9be63-295">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="9be63-296">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="9be63-296">storageBlockRemovableStorage</span></span>|<span data-ttu-id="9be63-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-297">Boolean</span></span>|<span data-ttu-id="9be63-298">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="9be63-298">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="9be63-299">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="9be63-299">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="9be63-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-300">Boolean</span></span>|<span data-ttu-id="9be63-301">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="9be63-301">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="9be63-302">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="9be63-302">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="9be63-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-303">Boolean</span></span>|<span data-ttu-id="9be63-304">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="9be63-304">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="9be63-305">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-305">voiceAssistantBlocked</span></span>|<span data-ttu-id="9be63-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-306">Boolean</span></span>|<span data-ttu-id="9be63-307">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="9be63-307">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="9be63-308">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-308">voiceDialingBlocked</span></span>|<span data-ttu-id="9be63-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-309">Boolean</span></span>|<span data-ttu-id="9be63-310">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="9be63-310">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="9be63-311">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="9be63-311">webBrowserBlockPopups</span></span>|<span data-ttu-id="9be63-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-312">Boolean</span></span>|<span data-ttu-id="9be63-313">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="9be63-313">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="9be63-314">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="9be63-314">webBrowserBlockAutofill</span></span>|<span data-ttu-id="9be63-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-315">Boolean</span></span>|<span data-ttu-id="9be63-316">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="9be63-316">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="9be63-317">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="9be63-317">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="9be63-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-318">Boolean</span></span>|<span data-ttu-id="9be63-319">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="9be63-319">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="9be63-320">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-320">webBrowserBlocked</span></span>|<span data-ttu-id="9be63-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-321">Boolean</span></span>|<span data-ttu-id="9be63-322">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="9be63-322">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="9be63-323">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9be63-323">webBrowserCookieSettings</span></span>|[<span data-ttu-id="9be63-324">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9be63-324">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="9be63-325">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="9be63-325">Cookie settings within the web browser.</span></span> <span data-ttu-id="9be63-326">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="9be63-326">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="9be63-327">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="9be63-327">wiFiBlocked</span></span>|<span data-ttu-id="9be63-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-328">Boolean</span></span>|<span data-ttu-id="9be63-329">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="9be63-329">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="9be63-330">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="9be63-330">appsInstallAllowList</span></span>|<span data-ttu-id="9be63-331">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9be63-331">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9be63-332">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="9be63-332">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="9be63-333">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9be63-333">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9be63-334">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="9be63-334">appsLaunchBlockList</span></span>|<span data-ttu-id="9be63-335">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9be63-335">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9be63-336">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="9be63-336">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="9be63-337">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9be63-337">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9be63-338">appsHideList</span><span class="sxs-lookup"><span data-stu-id="9be63-338">appsHideList</span></span>|<span data-ttu-id="9be63-339">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9be63-339">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9be63-340">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="9be63-340">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="9be63-341">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9be63-341">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9be63-342">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="9be63-342">securityRequireVerifyApps</span></span>|<span data-ttu-id="9be63-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be63-343">Boolean</span></span>|<span data-ttu-id="9be63-344">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="9be63-344">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="9be63-345">响应</span><span class="sxs-lookup"><span data-stu-id="9be63-345">Response</span></span>
<span data-ttu-id="9be63-346">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9be63-346">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9be63-347">示例</span><span class="sxs-lookup"><span data-stu-id="9be63-347">Example</span></span>

### <a name="request"></a><span data-ttu-id="9be63-348">请求</span><span class="sxs-lookup"><span data-stu-id="9be63-348">Request</span></span>
<span data-ttu-id="9be63-349">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9be63-349">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3974

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="9be63-350">响应</span><span class="sxs-lookup"><span data-stu-id="9be63-350">Response</span></span>
<span data-ttu-id="9be63-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9be63-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4146

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
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
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```




