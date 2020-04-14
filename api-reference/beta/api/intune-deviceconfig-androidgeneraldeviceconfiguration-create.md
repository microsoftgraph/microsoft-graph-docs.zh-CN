---
title: 创建 androidGeneralDeviceConfiguration
description: 创建新的 androidGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 468b5c4b06dc644bc237ef573362e8868373a6af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43435734"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="931b1-103">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="931b1-103">Create androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="931b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="931b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="931b1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="931b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="931b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="931b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="931b1-107">创建新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="931b1-107">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="931b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="931b1-108">Prerequisites</span></span>
<span data-ttu-id="931b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="931b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="931b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="931b1-111">Permission type</span></span>|<span data-ttu-id="931b1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="931b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="931b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="931b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="931b1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="931b1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="931b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="931b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="931b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="931b1-116">Not supported.</span></span>|
|<span data-ttu-id="931b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="931b1-117">Application</span></span>|<span data-ttu-id="931b1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="931b1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="931b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="931b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="931b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="931b1-120">Request headers</span></span>
|<span data-ttu-id="931b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="931b1-121">Header</span></span>|<span data-ttu-id="931b1-122">值</span><span class="sxs-lookup"><span data-stu-id="931b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="931b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="931b1-123">Authorization</span></span>|<span data-ttu-id="931b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="931b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="931b1-125">接受</span><span class="sxs-lookup"><span data-stu-id="931b1-125">Accept</span></span>|<span data-ttu-id="931b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="931b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="931b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="931b1-127">Request body</span></span>
<span data-ttu-id="931b1-128">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="931b1-128">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="931b1-129">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="931b1-129">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="931b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="931b1-130">Property</span></span>|<span data-ttu-id="931b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="931b1-131">Type</span></span>|<span data-ttu-id="931b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="931b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="931b1-133">id</span><span class="sxs-lookup"><span data-stu-id="931b1-133">id</span></span>|<span data-ttu-id="931b1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="931b1-134">String</span></span>|<span data-ttu-id="931b1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="931b1-135">Key of the entity.</span></span> <span data-ttu-id="931b1-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="931b1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="931b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="931b1-138">DateTimeOffset</span></span>|<span data-ttu-id="931b1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="931b1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="931b1-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="931b1-141">roleScopeTagIds</span></span>|<span data-ttu-id="931b1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="931b1-142">String collection</span></span>|<span data-ttu-id="931b1-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="931b1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="931b1-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="931b1-145">supportsScopeTags</span></span>|<span data-ttu-id="931b1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-146">Boolean</span></span>|<span data-ttu-id="931b1-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="931b1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="931b1-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="931b1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="931b1-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="931b1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="931b1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="931b1-150">This property is read-only.</span></span> <span data-ttu-id="931b1-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="931b1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="931b1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="931b1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="931b1-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="931b1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="931b1-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="931b1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="931b1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="931b1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="931b1-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="931b1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="931b1-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="931b1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="931b1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="931b1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="931b1-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="931b1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="931b1-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="931b1-164">createdDateTime</span></span>|<span data-ttu-id="931b1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="931b1-165">DateTimeOffset</span></span>|<span data-ttu-id="931b1-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="931b1-166">DateTime the object was created.</span></span> <span data-ttu-id="931b1-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-168">description</span><span class="sxs-lookup"><span data-stu-id="931b1-168">description</span></span>|<span data-ttu-id="931b1-169">String</span><span class="sxs-lookup"><span data-stu-id="931b1-169">String</span></span>|<span data-ttu-id="931b1-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="931b1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="931b1-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="931b1-172">displayName</span></span>|<span data-ttu-id="931b1-173">String</span><span class="sxs-lookup"><span data-stu-id="931b1-173">String</span></span>|<span data-ttu-id="931b1-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="931b1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="931b1-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-176">version</span><span class="sxs-lookup"><span data-stu-id="931b1-176">version</span></span>|<span data-ttu-id="931b1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="931b1-177">Int32</span></span>|<span data-ttu-id="931b1-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="931b1-178">Version of the device configuration.</span></span> <span data-ttu-id="931b1-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="931b1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="931b1-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="931b1-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="931b1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-181">Boolean</span></span>|<span data-ttu-id="931b1-182">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="931b1-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="931b1-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="931b1-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="931b1-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-184">Boolean</span></span>|<span data-ttu-id="931b1-185">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="931b1-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="931b1-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="931b1-186">appsBlockYouTube</span></span>|<span data-ttu-id="931b1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-187">Boolean</span></span>|<span data-ttu-id="931b1-188">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="931b1-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="931b1-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-189">bluetoothBlocked</span></span>|<span data-ttu-id="931b1-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-190">Boolean</span></span>|<span data-ttu-id="931b1-191">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="931b1-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="931b1-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-192">cameraBlocked</span></span>|<span data-ttu-id="931b1-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-193">Boolean</span></span>|<span data-ttu-id="931b1-194">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="931b1-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="931b1-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="931b1-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="931b1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-196">Boolean</span></span>|<span data-ttu-id="931b1-197">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="931b1-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="931b1-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="931b1-198">cellularBlockMessaging</span></span>|<span data-ttu-id="931b1-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-199">Boolean</span></span>|<span data-ttu-id="931b1-200">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="931b1-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="931b1-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="931b1-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="931b1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-202">Boolean</span></span>|<span data-ttu-id="931b1-203">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="931b1-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="931b1-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="931b1-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="931b1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-205">Boolean</span></span>|<span data-ttu-id="931b1-206">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="931b1-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="931b1-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="931b1-207">compliantAppsList</span></span>|<span data-ttu-id="931b1-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="931b1-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="931b1-209">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="931b1-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="931b1-210">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="931b1-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="931b1-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="931b1-211">compliantAppListType</span></span>|[<span data-ttu-id="931b1-212">appListType</span><span class="sxs-lookup"><span data-stu-id="931b1-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="931b1-213">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="931b1-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="931b1-214">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="931b1-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="931b1-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="931b1-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="931b1-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-216">Boolean</span></span>|<span data-ttu-id="931b1-217">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="931b1-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="931b1-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-218">locationServicesBlocked</span></span>|<span data-ttu-id="931b1-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-219">Boolean</span></span>|<span data-ttu-id="931b1-220">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="931b1-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="931b1-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="931b1-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="931b1-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-222">Boolean</span></span>|<span data-ttu-id="931b1-223">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="931b1-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="931b1-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="931b1-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-225">Boolean</span></span>|<span data-ttu-id="931b1-226">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="931b1-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="931b1-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="931b1-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="931b1-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-228">Boolean</span></span>|<span data-ttu-id="931b1-229">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="931b1-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="931b1-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="931b1-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="931b1-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-231">Boolean</span></span>|<span data-ttu-id="931b1-232">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="931b1-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="931b1-233">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="931b1-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="931b1-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-234">Boolean</span></span>|<span data-ttu-id="931b1-235">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="931b1-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="931b1-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="931b1-236">kioskModeApps</span></span>|<span data-ttu-id="931b1-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="931b1-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="931b1-238">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="931b1-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="931b1-239">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="931b1-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="931b1-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-240">nfcBlocked</span></span>|<span data-ttu-id="931b1-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-241">Boolean</span></span>|<span data-ttu-id="931b1-242">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="931b1-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="931b1-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="931b1-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="931b1-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-244">Boolean</span></span>|<span data-ttu-id="931b1-245">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="931b1-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="931b1-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="931b1-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="931b1-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-247">Boolean</span></span>|<span data-ttu-id="931b1-248">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="931b1-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="931b1-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="931b1-249">passwordExpirationDays</span></span>|<span data-ttu-id="931b1-250">Int32</span><span class="sxs-lookup"><span data-stu-id="931b1-250">Int32</span></span>|<span data-ttu-id="931b1-251">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="931b1-251">Number of days before the password expires.</span></span> <span data-ttu-id="931b1-252">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="931b1-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="931b1-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="931b1-253">passwordMinimumLength</span></span>|<span data-ttu-id="931b1-254">Int32</span><span class="sxs-lookup"><span data-stu-id="931b1-254">Int32</span></span>|<span data-ttu-id="931b1-255">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="931b1-255">Minimum length of passwords.</span></span> <span data-ttu-id="931b1-256">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="931b1-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="931b1-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="931b1-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="931b1-258">Int32</span><span class="sxs-lookup"><span data-stu-id="931b1-258">Int32</span></span>|<span data-ttu-id="931b1-259">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="931b1-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="931b1-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="931b1-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="931b1-261">Int32</span><span class="sxs-lookup"><span data-stu-id="931b1-261">Int32</span></span>|<span data-ttu-id="931b1-262">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="931b1-262">Number of previous passwords to block.</span></span> <span data-ttu-id="931b1-263">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="931b1-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="931b1-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="931b1-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="931b1-265">Int32</span><span class="sxs-lookup"><span data-stu-id="931b1-265">Int32</span></span>|<span data-ttu-id="931b1-266">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="931b1-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="931b1-267">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="931b1-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="931b1-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="931b1-268">passwordRequiredType</span></span>|[<span data-ttu-id="931b1-269">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="931b1-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="931b1-270">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="931b1-270">Type of password that is required.</span></span> <span data-ttu-id="931b1-271">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="931b1-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="931b1-272">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="931b1-272">passwordRequired</span></span>|<span data-ttu-id="931b1-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-273">Boolean</span></span>|<span data-ttu-id="931b1-274">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="931b1-274">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="931b1-275">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-275">powerOffBlocked</span></span>|<span data-ttu-id="931b1-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-276">Boolean</span></span>|<span data-ttu-id="931b1-277">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="931b1-277">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="931b1-278">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-278">factoryResetBlocked</span></span>|<span data-ttu-id="931b1-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-279">Boolean</span></span>|<span data-ttu-id="931b1-280">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="931b1-280">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="931b1-281">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-281">screenCaptureBlocked</span></span>|<span data-ttu-id="931b1-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-282">Boolean</span></span>|<span data-ttu-id="931b1-283">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="931b1-283">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="931b1-284">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="931b1-284">deviceSharingAllowed</span></span>|<span data-ttu-id="931b1-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-285">Boolean</span></span>|<span data-ttu-id="931b1-286">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="931b1-286">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="931b1-287">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="931b1-287">storageBlockGoogleBackup</span></span>|<span data-ttu-id="931b1-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-288">Boolean</span></span>|<span data-ttu-id="931b1-289">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="931b1-289">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="931b1-290">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="931b1-290">storageBlockRemovableStorage</span></span>|<span data-ttu-id="931b1-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-291">Boolean</span></span>|<span data-ttu-id="931b1-292">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="931b1-292">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="931b1-293">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="931b1-293">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="931b1-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-294">Boolean</span></span>|<span data-ttu-id="931b1-295">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="931b1-295">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="931b1-296">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="931b1-296">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="931b1-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-297">Boolean</span></span>|<span data-ttu-id="931b1-298">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="931b1-298">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="931b1-299">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-299">voiceAssistantBlocked</span></span>|<span data-ttu-id="931b1-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-300">Boolean</span></span>|<span data-ttu-id="931b1-301">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="931b1-301">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="931b1-302">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-302">voiceDialingBlocked</span></span>|<span data-ttu-id="931b1-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-303">Boolean</span></span>|<span data-ttu-id="931b1-304">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="931b1-304">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="931b1-305">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="931b1-305">webBrowserBlockPopups</span></span>|<span data-ttu-id="931b1-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-306">Boolean</span></span>|<span data-ttu-id="931b1-307">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="931b1-307">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="931b1-308">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="931b1-308">webBrowserBlockAutofill</span></span>|<span data-ttu-id="931b1-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-309">Boolean</span></span>|<span data-ttu-id="931b1-310">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="931b1-310">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="931b1-311">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="931b1-311">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="931b1-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-312">Boolean</span></span>|<span data-ttu-id="931b1-313">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="931b1-313">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="931b1-314">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-314">webBrowserBlocked</span></span>|<span data-ttu-id="931b1-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-315">Boolean</span></span>|<span data-ttu-id="931b1-316">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="931b1-316">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="931b1-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="931b1-317">webBrowserCookieSettings</span></span>|[<span data-ttu-id="931b1-318">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="931b1-318">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="931b1-319">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="931b1-319">Cookie settings within the web browser.</span></span> <span data-ttu-id="931b1-320">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="931b1-320">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="931b1-321">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="931b1-321">wiFiBlocked</span></span>|<span data-ttu-id="931b1-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-322">Boolean</span></span>|<span data-ttu-id="931b1-323">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="931b1-323">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="931b1-324">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="931b1-324">appsInstallAllowList</span></span>|<span data-ttu-id="931b1-325">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="931b1-325">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="931b1-326">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="931b1-326">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="931b1-327">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="931b1-327">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="931b1-328">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="931b1-328">appsLaunchBlockList</span></span>|<span data-ttu-id="931b1-329">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="931b1-329">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="931b1-330">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="931b1-330">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="931b1-331">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="931b1-331">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="931b1-332">appsHideList</span><span class="sxs-lookup"><span data-stu-id="931b1-332">appsHideList</span></span>|<span data-ttu-id="931b1-333">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="931b1-333">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="931b1-334">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="931b1-334">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="931b1-335">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="931b1-335">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="931b1-336">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="931b1-336">securityRequireVerifyApps</span></span>|<span data-ttu-id="931b1-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="931b1-337">Boolean</span></span>|<span data-ttu-id="931b1-338">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="931b1-338">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="931b1-339">响应</span><span class="sxs-lookup"><span data-stu-id="931b1-339">Response</span></span>
<span data-ttu-id="931b1-340">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="931b1-340">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="931b1-341">示例</span><span class="sxs-lookup"><span data-stu-id="931b1-341">Example</span></span>

### <a name="request"></a><span data-ttu-id="931b1-342">请求</span><span class="sxs-lookup"><span data-stu-id="931b1-342">Request</span></span>
<span data-ttu-id="931b1-343">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="931b1-343">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="931b1-344">响应</span><span class="sxs-lookup"><span data-stu-id="931b1-344">Response</span></span>
<span data-ttu-id="931b1-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="931b1-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



