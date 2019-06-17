---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fc7f6b0681a0b9ddb8f25a182a68c5b4310abe3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970182"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="da78a-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="da78a-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="da78a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da78a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da78a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da78a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da78a-106">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da78a-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da78a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da78a-107">Prerequisites</span></span>
<span data-ttu-id="da78a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da78a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da78a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da78a-110">Permission type</span></span>|<span data-ttu-id="da78a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da78a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da78a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da78a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da78a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da78a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da78a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da78a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da78a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da78a-115">Not supported.</span></span>|
|<span data-ttu-id="da78a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da78a-116">Application</span></span>|<span data-ttu-id="da78a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="da78a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da78a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da78a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="da78a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da78a-119">Request headers</span></span>
|<span data-ttu-id="da78a-120">标头</span><span class="sxs-lookup"><span data-stu-id="da78a-120">Header</span></span>|<span data-ttu-id="da78a-121">值</span><span class="sxs-lookup"><span data-stu-id="da78a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da78a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da78a-122">Authorization</span></span>|<span data-ttu-id="da78a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da78a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da78a-124">接受</span><span class="sxs-lookup"><span data-stu-id="da78a-124">Accept</span></span>|<span data-ttu-id="da78a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da78a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da78a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da78a-126">Request body</span></span>
<span data-ttu-id="da78a-127">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da78a-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="da78a-128">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da78a-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="da78a-129">属性</span><span class="sxs-lookup"><span data-stu-id="da78a-129">Property</span></span>|<span data-ttu-id="da78a-130">类型</span><span class="sxs-lookup"><span data-stu-id="da78a-130">Type</span></span>|<span data-ttu-id="da78a-131">说明</span><span class="sxs-lookup"><span data-stu-id="da78a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da78a-132">id</span><span class="sxs-lookup"><span data-stu-id="da78a-132">id</span></span>|<span data-ttu-id="da78a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="da78a-133">String</span></span>|<span data-ttu-id="da78a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da78a-134">Key of the entity.</span></span> <span data-ttu-id="da78a-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da78a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="da78a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da78a-137">DateTimeOffset</span></span>|<span data-ttu-id="da78a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da78a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="da78a-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da78a-140">roleScopeTagIds</span></span>|<span data-ttu-id="da78a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="da78a-141">String collection</span></span>|<span data-ttu-id="da78a-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="da78a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da78a-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da78a-144">supportsScopeTags</span></span>|<span data-ttu-id="da78a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-145">Boolean</span></span>|<span data-ttu-id="da78a-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="da78a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da78a-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="da78a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da78a-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="da78a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da78a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="da78a-149">This property is read-only.</span></span> <span data-ttu-id="da78a-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da78a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="da78a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da78a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="da78a-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="da78a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="da78a-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da78a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="da78a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da78a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="da78a-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="da78a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="da78a-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da78a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="da78a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da78a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="da78a-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="da78a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="da78a-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da78a-163">createdDateTime</span></span>|<span data-ttu-id="da78a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da78a-164">DateTimeOffset</span></span>|<span data-ttu-id="da78a-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da78a-165">DateTime the object was created.</span></span> <span data-ttu-id="da78a-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-167">说明</span><span class="sxs-lookup"><span data-stu-id="da78a-167">description</span></span>|<span data-ttu-id="da78a-168">String</span><span class="sxs-lookup"><span data-stu-id="da78a-168">String</span></span>|<span data-ttu-id="da78a-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="da78a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da78a-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="da78a-171">displayName</span></span>|<span data-ttu-id="da78a-172">String</span><span class="sxs-lookup"><span data-stu-id="da78a-172">String</span></span>|<span data-ttu-id="da78a-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="da78a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da78a-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-175">version</span><span class="sxs-lookup"><span data-stu-id="da78a-175">version</span></span>|<span data-ttu-id="da78a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="da78a-176">Int32</span></span>|<span data-ttu-id="da78a-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="da78a-177">Version of the device configuration.</span></span> <span data-ttu-id="da78a-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da78a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da78a-179">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="da78a-179">appsBlockClipboardSharing</span></span>|<span data-ttu-id="da78a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-180">Boolean</span></span>|<span data-ttu-id="da78a-181">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="da78a-181">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="da78a-182">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="da78a-182">appsBlockCopyPaste</span></span>|<span data-ttu-id="da78a-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-183">Boolean</span></span>|<span data-ttu-id="da78a-184">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="da78a-184">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="da78a-185">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="da78a-185">appsBlockYouTube</span></span>|<span data-ttu-id="da78a-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-186">Boolean</span></span>|<span data-ttu-id="da78a-187">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="da78a-187">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="da78a-188">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-188">bluetoothBlocked</span></span>|<span data-ttu-id="da78a-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-189">Boolean</span></span>|<span data-ttu-id="da78a-190">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="da78a-190">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="da78a-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-191">cameraBlocked</span></span>|<span data-ttu-id="da78a-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-192">Boolean</span></span>|<span data-ttu-id="da78a-193">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="da78a-193">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="da78a-194">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="da78a-194">cellularBlockDataRoaming</span></span>|<span data-ttu-id="da78a-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-195">Boolean</span></span>|<span data-ttu-id="da78a-196">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="da78a-196">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="da78a-197">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="da78a-197">cellularBlockMessaging</span></span>|<span data-ttu-id="da78a-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-198">Boolean</span></span>|<span data-ttu-id="da78a-199">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="da78a-199">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="da78a-200">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="da78a-200">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="da78a-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-201">Boolean</span></span>|<span data-ttu-id="da78a-202">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="da78a-202">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="da78a-203">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="da78a-203">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="da78a-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-204">Boolean</span></span>|<span data-ttu-id="da78a-205">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="da78a-205">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="da78a-206">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="da78a-206">compliantAppsList</span></span>|<span data-ttu-id="da78a-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da78a-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da78a-208">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="da78a-208">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="da78a-209">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="da78a-209">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="da78a-210">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="da78a-210">compliantAppListType</span></span>|[<span data-ttu-id="da78a-211">appListType</span><span class="sxs-lookup"><span data-stu-id="da78a-211">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="da78a-212">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="da78a-212">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="da78a-213">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="da78a-213">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="da78a-214">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="da78a-214">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="da78a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-215">Boolean</span></span>|<span data-ttu-id="da78a-216">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="da78a-216">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="da78a-217">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-217">locationServicesBlocked</span></span>|<span data-ttu-id="da78a-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-218">Boolean</span></span>|<span data-ttu-id="da78a-219">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="da78a-219">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="da78a-220">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="da78a-220">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="da78a-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-221">Boolean</span></span>|<span data-ttu-id="da78a-222">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="da78a-222">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="da78a-223">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-223">googlePlayStoreBlocked</span></span>|<span data-ttu-id="da78a-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-224">Boolean</span></span>|<span data-ttu-id="da78a-225">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="da78a-225">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="da78a-226">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="da78a-226">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="da78a-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-227">Boolean</span></span>|<span data-ttu-id="da78a-228">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="da78a-228">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="da78a-229">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="da78a-229">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="da78a-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-230">Boolean</span></span>|<span data-ttu-id="da78a-231">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="da78a-231">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="da78a-232">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="da78a-232">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="da78a-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-233">Boolean</span></span>|<span data-ttu-id="da78a-234">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="da78a-234">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="da78a-235">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="da78a-235">kioskModeApps</span></span>|<span data-ttu-id="da78a-236">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da78a-236">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da78a-237">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="da78a-237">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="da78a-238">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="da78a-238">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="da78a-239">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-239">nfcBlocked</span></span>|<span data-ttu-id="da78a-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-240">Boolean</span></span>|<span data-ttu-id="da78a-241">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="da78a-241">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="da78a-242">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="da78a-242">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="da78a-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-243">Boolean</span></span>|<span data-ttu-id="da78a-244">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="da78a-244">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="da78a-245">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="da78a-245">passwordBlockTrustAgents</span></span>|<span data-ttu-id="da78a-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-246">Boolean</span></span>|<span data-ttu-id="da78a-247">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="da78a-247">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="da78a-248">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="da78a-248">passwordExpirationDays</span></span>|<span data-ttu-id="da78a-249">Int32</span><span class="sxs-lookup"><span data-stu-id="da78a-249">Int32</span></span>|<span data-ttu-id="da78a-250">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="da78a-250">Number of days before the password expires.</span></span> <span data-ttu-id="da78a-251">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="da78a-251">Valid values 1 to 365</span></span>|
|<span data-ttu-id="da78a-252">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="da78a-252">passwordMinimumLength</span></span>|<span data-ttu-id="da78a-253">Int32</span><span class="sxs-lookup"><span data-stu-id="da78a-253">Int32</span></span>|<span data-ttu-id="da78a-254">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="da78a-254">Minimum length of passwords.</span></span> <span data-ttu-id="da78a-255">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="da78a-255">Valid values 4 to 16</span></span>|
|<span data-ttu-id="da78a-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="da78a-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="da78a-257">Int32</span><span class="sxs-lookup"><span data-stu-id="da78a-257">Int32</span></span>|<span data-ttu-id="da78a-258">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="da78a-258">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="da78a-259">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="da78a-259">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="da78a-260">Int32</span><span class="sxs-lookup"><span data-stu-id="da78a-260">Int32</span></span>|<span data-ttu-id="da78a-261">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="da78a-261">Number of previous passwords to block.</span></span> <span data-ttu-id="da78a-262">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="da78a-262">Valid values 0 to 24</span></span>|
|<span data-ttu-id="da78a-263">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="da78a-263">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="da78a-264">Int32</span><span class="sxs-lookup"><span data-stu-id="da78a-264">Int32</span></span>|<span data-ttu-id="da78a-265">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="da78a-265">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="da78a-266">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="da78a-266">Valid values 1 to 16</span></span>|
|<span data-ttu-id="da78a-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="da78a-267">passwordRequiredType</span></span>|[<span data-ttu-id="da78a-268">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="da78a-268">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="da78a-269">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="da78a-269">Type of password that is required.</span></span> <span data-ttu-id="da78a-270">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="da78a-270">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="da78a-271">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="da78a-271">passwordRequired</span></span>|<span data-ttu-id="da78a-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-272">Boolean</span></span>|<span data-ttu-id="da78a-273">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="da78a-273">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="da78a-274">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-274">powerOffBlocked</span></span>|<span data-ttu-id="da78a-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-275">Boolean</span></span>|<span data-ttu-id="da78a-276">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="da78a-276">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="da78a-277">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-277">factoryResetBlocked</span></span>|<span data-ttu-id="da78a-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-278">Boolean</span></span>|<span data-ttu-id="da78a-279">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="da78a-279">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="da78a-280">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-280">screenCaptureBlocked</span></span>|<span data-ttu-id="da78a-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-281">Boolean</span></span>|<span data-ttu-id="da78a-282">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="da78a-282">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="da78a-283">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="da78a-283">deviceSharingAllowed</span></span>|<span data-ttu-id="da78a-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-284">Boolean</span></span>|<span data-ttu-id="da78a-285">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="da78a-285">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="da78a-286">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="da78a-286">storageBlockGoogleBackup</span></span>|<span data-ttu-id="da78a-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-287">Boolean</span></span>|<span data-ttu-id="da78a-288">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="da78a-288">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="da78a-289">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="da78a-289">storageBlockRemovableStorage</span></span>|<span data-ttu-id="da78a-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-290">Boolean</span></span>|<span data-ttu-id="da78a-291">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="da78a-291">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="da78a-292">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="da78a-292">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="da78a-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-293">Boolean</span></span>|<span data-ttu-id="da78a-294">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="da78a-294">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="da78a-295">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="da78a-295">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="da78a-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-296">Boolean</span></span>|<span data-ttu-id="da78a-297">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="da78a-297">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="da78a-298">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-298">voiceAssistantBlocked</span></span>|<span data-ttu-id="da78a-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-299">Boolean</span></span>|<span data-ttu-id="da78a-300">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="da78a-300">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="da78a-301">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-301">voiceDialingBlocked</span></span>|<span data-ttu-id="da78a-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-302">Boolean</span></span>|<span data-ttu-id="da78a-303">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="da78a-303">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="da78a-304">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="da78a-304">webBrowserBlockPopups</span></span>|<span data-ttu-id="da78a-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-305">Boolean</span></span>|<span data-ttu-id="da78a-306">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="da78a-306">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="da78a-307">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="da78a-307">webBrowserBlockAutofill</span></span>|<span data-ttu-id="da78a-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-308">Boolean</span></span>|<span data-ttu-id="da78a-309">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="da78a-309">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="da78a-310">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="da78a-310">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="da78a-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-311">Boolean</span></span>|<span data-ttu-id="da78a-312">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="da78a-312">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="da78a-313">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-313">webBrowserBlocked</span></span>|<span data-ttu-id="da78a-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-314">Boolean</span></span>|<span data-ttu-id="da78a-315">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="da78a-315">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="da78a-316">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="da78a-316">webBrowserCookieSettings</span></span>|[<span data-ttu-id="da78a-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="da78a-317">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="da78a-318">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="da78a-318">Cookie settings within the web browser.</span></span> <span data-ttu-id="da78a-319">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="da78a-319">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="da78a-320">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="da78a-320">wiFiBlocked</span></span>|<span data-ttu-id="da78a-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-321">Boolean</span></span>|<span data-ttu-id="da78a-322">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="da78a-322">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="da78a-323">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="da78a-323">appsInstallAllowList</span></span>|<span data-ttu-id="da78a-324">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da78a-324">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da78a-325">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="da78a-325">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="da78a-326">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="da78a-326">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="da78a-327">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="da78a-327">appsLaunchBlockList</span></span>|<span data-ttu-id="da78a-328">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da78a-328">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da78a-329">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="da78a-329">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="da78a-330">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="da78a-330">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="da78a-331">appsHideList</span><span class="sxs-lookup"><span data-stu-id="da78a-331">appsHideList</span></span>|<span data-ttu-id="da78a-332">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da78a-332">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da78a-333">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="da78a-333">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="da78a-334">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="da78a-334">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="da78a-335">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="da78a-335">securityRequireVerifyApps</span></span>|<span data-ttu-id="da78a-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="da78a-336">Boolean</span></span>|<span data-ttu-id="da78a-337">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="da78a-337">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="da78a-338">响应</span><span class="sxs-lookup"><span data-stu-id="da78a-338">Response</span></span>
<span data-ttu-id="da78a-339">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da78a-339">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da78a-340">示例</span><span class="sxs-lookup"><span data-stu-id="da78a-340">Example</span></span>

### <a name="request"></a><span data-ttu-id="da78a-341">请求</span><span class="sxs-lookup"><span data-stu-id="da78a-341">Request</span></span>
<span data-ttu-id="da78a-342">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da78a-342">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="da78a-343">响应</span><span class="sxs-lookup"><span data-stu-id="da78a-343">Response</span></span>
<span data-ttu-id="da78a-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da78a-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





