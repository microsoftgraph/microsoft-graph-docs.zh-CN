---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb2e33c9facbed7885b9ed629135c42e0c129667
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43435688"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="3bbe2-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bbe2-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="3bbe2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bbe2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bbe2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bbe2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bbe2-107">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bbe2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3bbe2-108">Prerequisites</span></span>
<span data-ttu-id="3bbe2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bbe2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bbe2-111">Permission type</span></span>|<span data-ttu-id="3bbe2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3bbe2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bbe2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bbe2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bbe2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bbe2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bbe2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bbe2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bbe2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-116">Not supported.</span></span>|
|<span data-ttu-id="3bbe2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bbe2-117">Application</span></span>|<span data-ttu-id="3bbe2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bbe2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bbe2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bbe2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3bbe2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bbe2-120">Request headers</span></span>
|<span data-ttu-id="3bbe2-121">标头</span><span class="sxs-lookup"><span data-stu-id="3bbe2-121">Header</span></span>|<span data-ttu-id="3bbe2-122">值</span><span class="sxs-lookup"><span data-stu-id="3bbe2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bbe2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bbe2-123">Authorization</span></span>|<span data-ttu-id="3bbe2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bbe2-125">接受</span><span class="sxs-lookup"><span data-stu-id="3bbe2-125">Accept</span></span>|<span data-ttu-id="3bbe2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bbe2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bbe2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bbe2-127">Request body</span></span>
<span data-ttu-id="3bbe2-128">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="3bbe2-129">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="3bbe2-130">属性</span><span class="sxs-lookup"><span data-stu-id="3bbe2-130">Property</span></span>|<span data-ttu-id="3bbe2-131">类型</span><span class="sxs-lookup"><span data-stu-id="3bbe2-131">Type</span></span>|<span data-ttu-id="3bbe2-132">说明</span><span class="sxs-lookup"><span data-stu-id="3bbe2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bbe2-133">id</span><span class="sxs-lookup"><span data-stu-id="3bbe2-133">id</span></span>|<span data-ttu-id="3bbe2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3bbe2-134">String</span></span>|<span data-ttu-id="3bbe2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-135">Key of the entity.</span></span> <span data-ttu-id="3bbe2-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bbe2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3bbe2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bbe2-138">DateTimeOffset</span></span>|<span data-ttu-id="3bbe2-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3bbe2-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3bbe2-141">roleScopeTagIds</span></span>|<span data-ttu-id="3bbe2-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="3bbe2-142">String collection</span></span>|<span data-ttu-id="3bbe2-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3bbe2-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3bbe2-145">supportsScopeTags</span></span>|<span data-ttu-id="3bbe2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-146">Boolean</span></span>|<span data-ttu-id="3bbe2-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3bbe2-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3bbe2-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3bbe2-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-150">This property is read-only.</span></span> <span data-ttu-id="3bbe2-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3bbe2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3bbe2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3bbe2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3bbe2-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3bbe2-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3bbe2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3bbe2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3bbe2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3bbe2-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3bbe2-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bbe2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3bbe2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bbe2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3bbe2-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3bbe2-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bbe2-164">createdDateTime</span></span>|<span data-ttu-id="3bbe2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bbe2-165">DateTimeOffset</span></span>|<span data-ttu-id="3bbe2-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-166">DateTime the object was created.</span></span> <span data-ttu-id="3bbe2-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-168">description</span><span class="sxs-lookup"><span data-stu-id="3bbe2-168">description</span></span>|<span data-ttu-id="3bbe2-169">String</span><span class="sxs-lookup"><span data-stu-id="3bbe2-169">String</span></span>|<span data-ttu-id="3bbe2-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3bbe2-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3bbe2-172">displayName</span></span>|<span data-ttu-id="3bbe2-173">String</span><span class="sxs-lookup"><span data-stu-id="3bbe2-173">String</span></span>|<span data-ttu-id="3bbe2-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3bbe2-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-176">version</span><span class="sxs-lookup"><span data-stu-id="3bbe2-176">version</span></span>|<span data-ttu-id="3bbe2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbe2-177">Int32</span></span>|<span data-ttu-id="3bbe2-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-178">Version of the device configuration.</span></span> <span data-ttu-id="3bbe2-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bbe2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bbe2-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="3bbe2-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="3bbe2-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-181">Boolean</span></span>|<span data-ttu-id="3bbe2-182">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="3bbe2-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="3bbe2-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="3bbe2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-184">Boolean</span></span>|<span data-ttu-id="3bbe2-185">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="3bbe2-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="3bbe2-186">appsBlockYouTube</span></span>|<span data-ttu-id="3bbe2-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-187">Boolean</span></span>|<span data-ttu-id="3bbe2-188">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="3bbe2-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-189">bluetoothBlocked</span></span>|<span data-ttu-id="3bbe2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-190">Boolean</span></span>|<span data-ttu-id="3bbe2-191">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="3bbe2-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-192">cameraBlocked</span></span>|<span data-ttu-id="3bbe2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-193">Boolean</span></span>|<span data-ttu-id="3bbe2-194">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="3bbe2-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="3bbe2-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="3bbe2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-196">Boolean</span></span>|<span data-ttu-id="3bbe2-197">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="3bbe2-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="3bbe2-198">cellularBlockMessaging</span></span>|<span data-ttu-id="3bbe2-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-199">Boolean</span></span>|<span data-ttu-id="3bbe2-200">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="3bbe2-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="3bbe2-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="3bbe2-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-202">Boolean</span></span>|<span data-ttu-id="3bbe2-203">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="3bbe2-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="3bbe2-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="3bbe2-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-205">Boolean</span></span>|<span data-ttu-id="3bbe2-206">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="3bbe2-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="3bbe2-207">compliantAppsList</span></span>|<span data-ttu-id="3bbe2-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bbe2-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3bbe2-209">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="3bbe2-210">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="3bbe2-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="3bbe2-211">compliantAppListType</span></span>|[<span data-ttu-id="3bbe2-212">appListType</span><span class="sxs-lookup"><span data-stu-id="3bbe2-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="3bbe2-213">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="3bbe2-214">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="3bbe2-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="3bbe2-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="3bbe2-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-216">Boolean</span></span>|<span data-ttu-id="3bbe2-217">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="3bbe2-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-218">locationServicesBlocked</span></span>|<span data-ttu-id="3bbe2-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-219">Boolean</span></span>|<span data-ttu-id="3bbe2-220">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="3bbe2-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="3bbe2-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="3bbe2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-222">Boolean</span></span>|<span data-ttu-id="3bbe2-223">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="3bbe2-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="3bbe2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-225">Boolean</span></span>|<span data-ttu-id="3bbe2-226">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="3bbe2-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="3bbe2-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="3bbe2-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-228">Boolean</span></span>|<span data-ttu-id="3bbe2-229">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="3bbe2-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="3bbe2-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="3bbe2-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-231">Boolean</span></span>|<span data-ttu-id="3bbe2-232">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="3bbe2-233">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="3bbe2-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="3bbe2-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-234">Boolean</span></span>|<span data-ttu-id="3bbe2-235">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="3bbe2-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="3bbe2-236">kioskModeApps</span></span>|<span data-ttu-id="3bbe2-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bbe2-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3bbe2-238">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="3bbe2-239">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3bbe2-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-240">nfcBlocked</span></span>|<span data-ttu-id="3bbe2-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-241">Boolean</span></span>|<span data-ttu-id="3bbe2-242">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="3bbe2-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="3bbe2-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="3bbe2-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-244">Boolean</span></span>|<span data-ttu-id="3bbe2-245">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="3bbe2-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="3bbe2-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="3bbe2-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-247">Boolean</span></span>|<span data-ttu-id="3bbe2-248">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="3bbe2-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3bbe2-249">passwordExpirationDays</span></span>|<span data-ttu-id="3bbe2-250">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbe2-250">Int32</span></span>|<span data-ttu-id="3bbe2-251">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-251">Number of days before the password expires.</span></span> <span data-ttu-id="3bbe2-252">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3bbe2-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3bbe2-253">passwordMinimumLength</span></span>|<span data-ttu-id="3bbe2-254">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbe2-254">Int32</span></span>|<span data-ttu-id="3bbe2-255">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-255">Minimum length of passwords.</span></span> <span data-ttu-id="3bbe2-256">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="3bbe2-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3bbe2-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3bbe2-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3bbe2-258">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbe2-258">Int32</span></span>|<span data-ttu-id="3bbe2-259">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3bbe2-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3bbe2-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3bbe2-261">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbe2-261">Int32</span></span>|<span data-ttu-id="3bbe2-262">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-262">Number of previous passwords to block.</span></span> <span data-ttu-id="3bbe2-263">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="3bbe2-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3bbe2-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3bbe2-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3bbe2-265">Int32</span><span class="sxs-lookup"><span data-stu-id="3bbe2-265">Int32</span></span>|<span data-ttu-id="3bbe2-266">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="3bbe2-267">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="3bbe2-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3bbe2-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3bbe2-268">passwordRequiredType</span></span>|[<span data-ttu-id="3bbe2-269">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3bbe2-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="3bbe2-270">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-270">Type of password that is required.</span></span> <span data-ttu-id="3bbe2-271">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="3bbe2-272">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3bbe2-272">passwordRequired</span></span>|<span data-ttu-id="3bbe2-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-273">Boolean</span></span>|<span data-ttu-id="3bbe2-274">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-274">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="3bbe2-275">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-275">powerOffBlocked</span></span>|<span data-ttu-id="3bbe2-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-276">Boolean</span></span>|<span data-ttu-id="3bbe2-277">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-277">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="3bbe2-278">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-278">factoryResetBlocked</span></span>|<span data-ttu-id="3bbe2-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-279">Boolean</span></span>|<span data-ttu-id="3bbe2-280">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-280">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="3bbe2-281">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-281">screenCaptureBlocked</span></span>|<span data-ttu-id="3bbe2-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-282">Boolean</span></span>|<span data-ttu-id="3bbe2-283">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-283">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="3bbe2-284">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="3bbe2-284">deviceSharingAllowed</span></span>|<span data-ttu-id="3bbe2-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-285">Boolean</span></span>|<span data-ttu-id="3bbe2-286">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-286">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="3bbe2-287">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="3bbe2-287">storageBlockGoogleBackup</span></span>|<span data-ttu-id="3bbe2-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-288">Boolean</span></span>|<span data-ttu-id="3bbe2-289">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-289">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="3bbe2-290">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="3bbe2-290">storageBlockRemovableStorage</span></span>|<span data-ttu-id="3bbe2-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-291">Boolean</span></span>|<span data-ttu-id="3bbe2-292">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-292">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="3bbe2-293">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="3bbe2-293">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="3bbe2-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-294">Boolean</span></span>|<span data-ttu-id="3bbe2-295">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-295">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="3bbe2-296">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="3bbe2-296">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="3bbe2-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-297">Boolean</span></span>|<span data-ttu-id="3bbe2-298">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-298">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="3bbe2-299">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-299">voiceAssistantBlocked</span></span>|<span data-ttu-id="3bbe2-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-300">Boolean</span></span>|<span data-ttu-id="3bbe2-301">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-301">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="3bbe2-302">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-302">voiceDialingBlocked</span></span>|<span data-ttu-id="3bbe2-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-303">Boolean</span></span>|<span data-ttu-id="3bbe2-304">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-304">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="3bbe2-305">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="3bbe2-305">webBrowserBlockPopups</span></span>|<span data-ttu-id="3bbe2-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-306">Boolean</span></span>|<span data-ttu-id="3bbe2-307">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-307">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="3bbe2-308">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="3bbe2-308">webBrowserBlockAutofill</span></span>|<span data-ttu-id="3bbe2-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-309">Boolean</span></span>|<span data-ttu-id="3bbe2-310">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-310">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="3bbe2-311">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="3bbe2-311">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="3bbe2-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-312">Boolean</span></span>|<span data-ttu-id="3bbe2-313">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-313">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="3bbe2-314">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-314">webBrowserBlocked</span></span>|<span data-ttu-id="3bbe2-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-315">Boolean</span></span>|<span data-ttu-id="3bbe2-316">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-316">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="3bbe2-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="3bbe2-317">webBrowserCookieSettings</span></span>|[<span data-ttu-id="3bbe2-318">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="3bbe2-318">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="3bbe2-319">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-319">Cookie settings within the web browser.</span></span> <span data-ttu-id="3bbe2-320">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-320">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="3bbe2-321">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="3bbe2-321">wiFiBlocked</span></span>|<span data-ttu-id="3bbe2-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-322">Boolean</span></span>|<span data-ttu-id="3bbe2-323">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-323">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="3bbe2-324">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="3bbe2-324">appsInstallAllowList</span></span>|<span data-ttu-id="3bbe2-325">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bbe2-325">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3bbe2-326">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-326">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="3bbe2-327">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-327">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3bbe2-328">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="3bbe2-328">appsLaunchBlockList</span></span>|<span data-ttu-id="3bbe2-329">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bbe2-329">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3bbe2-330">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-330">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="3bbe2-331">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-331">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3bbe2-332">appsHideList</span><span class="sxs-lookup"><span data-stu-id="3bbe2-332">appsHideList</span></span>|<span data-ttu-id="3bbe2-333">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bbe2-333">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3bbe2-334">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-334">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="3bbe2-335">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-335">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3bbe2-336">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3bbe2-336">securityRequireVerifyApps</span></span>|<span data-ttu-id="3bbe2-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bbe2-337">Boolean</span></span>|<span data-ttu-id="3bbe2-338">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-338">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="3bbe2-339">响应</span><span class="sxs-lookup"><span data-stu-id="3bbe2-339">Response</span></span>
<span data-ttu-id="3bbe2-340">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-340">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bbe2-341">示例</span><span class="sxs-lookup"><span data-stu-id="3bbe2-341">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bbe2-342">请求</span><span class="sxs-lookup"><span data-stu-id="3bbe2-342">Request</span></span>
<span data-ttu-id="3bbe2-343">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-343">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3934

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

### <a name="response"></a><span data-ttu-id="3bbe2-344">响应</span><span class="sxs-lookup"><span data-stu-id="3bbe2-344">Response</span></span>
<span data-ttu-id="3bbe2-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3bbe2-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4106

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



