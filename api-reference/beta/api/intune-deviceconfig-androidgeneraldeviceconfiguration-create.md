---
title: 创建 androidGeneralDeviceConfiguration
description: 创建新的 androidGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bb54858e2ef44d6a1f162730201f92542812c0d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49237805"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="950a4-103">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="950a4-103">Create androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="950a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="950a4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="950a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="950a4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="950a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950a4-107">创建新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="950a4-107">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="950a4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="950a4-108">Prerequisites</span></span>
<span data-ttu-id="950a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="950a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950a4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="950a4-111">Permission type</span></span>|<span data-ttu-id="950a4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="950a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="950a4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="950a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="950a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="950a4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="950a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="950a4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="950a4-116">Not supported.</span></span>|
|<span data-ttu-id="950a4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="950a4-117">Application</span></span>|<span data-ttu-id="950a4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950a4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="950a4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="950a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="950a4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="950a4-120">Request headers</span></span>
|<span data-ttu-id="950a4-121">标头</span><span class="sxs-lookup"><span data-stu-id="950a4-121">Header</span></span>|<span data-ttu-id="950a4-122">值</span><span class="sxs-lookup"><span data-stu-id="950a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="950a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="950a4-123">Authorization</span></span>|<span data-ttu-id="950a4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="950a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="950a4-125">接受</span><span class="sxs-lookup"><span data-stu-id="950a4-125">Accept</span></span>|<span data-ttu-id="950a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="950a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="950a4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="950a4-127">Request body</span></span>
<span data-ttu-id="950a4-128">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="950a4-128">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="950a4-129">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="950a4-129">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="950a4-130">属性</span><span class="sxs-lookup"><span data-stu-id="950a4-130">Property</span></span>|<span data-ttu-id="950a4-131">类型</span><span class="sxs-lookup"><span data-stu-id="950a4-131">Type</span></span>|<span data-ttu-id="950a4-132">说明</span><span class="sxs-lookup"><span data-stu-id="950a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950a4-133">id</span><span class="sxs-lookup"><span data-stu-id="950a4-133">id</span></span>|<span data-ttu-id="950a4-134">String</span><span class="sxs-lookup"><span data-stu-id="950a4-134">String</span></span>|<span data-ttu-id="950a4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="950a4-135">Key of the entity.</span></span> <span data-ttu-id="950a4-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="950a4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="950a4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950a4-138">DateTimeOffset</span></span>|<span data-ttu-id="950a4-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="950a4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="950a4-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="950a4-141">roleScopeTagIds</span></span>|<span data-ttu-id="950a4-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="950a4-142">String collection</span></span>|<span data-ttu-id="950a4-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="950a4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="950a4-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="950a4-145">supportsScopeTags</span></span>|<span data-ttu-id="950a4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-146">Boolean</span></span>|<span data-ttu-id="950a4-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="950a4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="950a4-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="950a4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="950a4-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="950a4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="950a4-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="950a4-150">This property is read-only.</span></span> <span data-ttu-id="950a4-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="950a4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="950a4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="950a4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="950a4-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="950a4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="950a4-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="950a4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="950a4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="950a4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="950a4-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="950a4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="950a4-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="950a4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="950a4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="950a4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="950a4-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="950a4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="950a4-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="950a4-164">createdDateTime</span></span>|<span data-ttu-id="950a4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950a4-165">DateTimeOffset</span></span>|<span data-ttu-id="950a4-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="950a4-166">DateTime the object was created.</span></span> <span data-ttu-id="950a4-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-168">description</span><span class="sxs-lookup"><span data-stu-id="950a4-168">description</span></span>|<span data-ttu-id="950a4-169">String</span><span class="sxs-lookup"><span data-stu-id="950a4-169">String</span></span>|<span data-ttu-id="950a4-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="950a4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="950a4-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="950a4-172">displayName</span></span>|<span data-ttu-id="950a4-173">String</span><span class="sxs-lookup"><span data-stu-id="950a4-173">String</span></span>|<span data-ttu-id="950a4-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="950a4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="950a4-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-176">version</span><span class="sxs-lookup"><span data-stu-id="950a4-176">version</span></span>|<span data-ttu-id="950a4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="950a4-177">Int32</span></span>|<span data-ttu-id="950a4-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="950a4-178">Version of the device configuration.</span></span> <span data-ttu-id="950a4-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="950a4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950a4-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="950a4-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="950a4-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-181">Boolean</span></span>|<span data-ttu-id="950a4-182">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="950a4-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="950a4-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="950a4-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="950a4-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-184">Boolean</span></span>|<span data-ttu-id="950a4-185">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="950a4-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="950a4-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="950a4-186">appsBlockYouTube</span></span>|<span data-ttu-id="950a4-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-187">Boolean</span></span>|<span data-ttu-id="950a4-188">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="950a4-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="950a4-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-189">bluetoothBlocked</span></span>|<span data-ttu-id="950a4-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-190">Boolean</span></span>|<span data-ttu-id="950a4-191">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="950a4-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="950a4-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-192">cameraBlocked</span></span>|<span data-ttu-id="950a4-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-193">Boolean</span></span>|<span data-ttu-id="950a4-194">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="950a4-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="950a4-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="950a4-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="950a4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-196">Boolean</span></span>|<span data-ttu-id="950a4-197">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="950a4-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="950a4-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="950a4-198">cellularBlockMessaging</span></span>|<span data-ttu-id="950a4-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-199">Boolean</span></span>|<span data-ttu-id="950a4-200">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="950a4-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="950a4-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="950a4-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="950a4-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-202">Boolean</span></span>|<span data-ttu-id="950a4-203">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="950a4-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="950a4-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="950a4-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="950a4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-205">Boolean</span></span>|<span data-ttu-id="950a4-206">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="950a4-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="950a4-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="950a4-207">compliantAppsList</span></span>|<span data-ttu-id="950a4-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="950a4-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="950a4-209">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="950a4-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="950a4-210">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="950a4-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="950a4-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="950a4-211">compliantAppListType</span></span>|[<span data-ttu-id="950a4-212">appListType</span><span class="sxs-lookup"><span data-stu-id="950a4-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="950a4-213">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="950a4-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="950a4-214">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="950a4-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="950a4-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="950a4-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="950a4-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-216">Boolean</span></span>|<span data-ttu-id="950a4-217">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="950a4-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="950a4-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-218">locationServicesBlocked</span></span>|<span data-ttu-id="950a4-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-219">Boolean</span></span>|<span data-ttu-id="950a4-220">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="950a4-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="950a4-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="950a4-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="950a4-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-222">Boolean</span></span>|<span data-ttu-id="950a4-223">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="950a4-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="950a4-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="950a4-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-225">Boolean</span></span>|<span data-ttu-id="950a4-226">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="950a4-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="950a4-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="950a4-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="950a4-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-228">Boolean</span></span>|<span data-ttu-id="950a4-229">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="950a4-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="950a4-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="950a4-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="950a4-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-231">Boolean</span></span>|<span data-ttu-id="950a4-232">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="950a4-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="950a4-233">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="950a4-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="950a4-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-234">Boolean</span></span>|<span data-ttu-id="950a4-235">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="950a4-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="950a4-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="950a4-236">kioskModeApps</span></span>|<span data-ttu-id="950a4-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="950a4-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="950a4-238">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="950a4-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="950a4-239">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="950a4-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="950a4-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-240">nfcBlocked</span></span>|<span data-ttu-id="950a4-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-241">Boolean</span></span>|<span data-ttu-id="950a4-242">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="950a4-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="950a4-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="950a4-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="950a4-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-244">Boolean</span></span>|<span data-ttu-id="950a4-245">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="950a4-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="950a4-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="950a4-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="950a4-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-247">Boolean</span></span>|<span data-ttu-id="950a4-248">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="950a4-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="950a4-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="950a4-249">passwordExpirationDays</span></span>|<span data-ttu-id="950a4-250">Int32</span><span class="sxs-lookup"><span data-stu-id="950a4-250">Int32</span></span>|<span data-ttu-id="950a4-251">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="950a4-251">Number of days before the password expires.</span></span> <span data-ttu-id="950a4-252">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="950a4-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="950a4-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="950a4-253">passwordMinimumLength</span></span>|<span data-ttu-id="950a4-254">Int32</span><span class="sxs-lookup"><span data-stu-id="950a4-254">Int32</span></span>|<span data-ttu-id="950a4-255">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="950a4-255">Minimum length of passwords.</span></span> <span data-ttu-id="950a4-256">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="950a4-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="950a4-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="950a4-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="950a4-258">Int32</span><span class="sxs-lookup"><span data-stu-id="950a4-258">Int32</span></span>|<span data-ttu-id="950a4-259">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="950a4-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="950a4-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="950a4-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="950a4-261">Int32</span><span class="sxs-lookup"><span data-stu-id="950a4-261">Int32</span></span>|<span data-ttu-id="950a4-262">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="950a4-262">Number of previous passwords to block.</span></span> <span data-ttu-id="950a4-263">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="950a4-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="950a4-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="950a4-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="950a4-265">Int32</span><span class="sxs-lookup"><span data-stu-id="950a4-265">Int32</span></span>|<span data-ttu-id="950a4-266">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="950a4-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="950a4-267">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="950a4-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="950a4-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="950a4-268">passwordRequiredType</span></span>|[<span data-ttu-id="950a4-269">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="950a4-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="950a4-270">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="950a4-270">Type of password that is required.</span></span> <span data-ttu-id="950a4-271">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="950a4-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="950a4-272">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="950a4-272">requiredPasswordComplexity</span></span>|[<span data-ttu-id="950a4-273">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="950a4-273">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="950a4-274">指示 Android 上所需的密码复杂性。</span><span class="sxs-lookup"><span data-stu-id="950a4-274">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="950a4-275">其中一个：无、低、中、高。</span><span class="sxs-lookup"><span data-stu-id="950a4-275">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="950a4-276">这是一个面向 Android 11 + 的 API。</span><span class="sxs-lookup"><span data-stu-id="950a4-276">This is an API targeted to Android 11+.</span></span> <span data-ttu-id="950a4-277">可取值为：`none`、`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="950a4-277">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="950a4-278">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="950a4-278">passwordRequired</span></span>|<span data-ttu-id="950a4-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-279">Boolean</span></span>|<span data-ttu-id="950a4-280">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="950a4-280">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="950a4-281">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-281">powerOffBlocked</span></span>|<span data-ttu-id="950a4-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-282">Boolean</span></span>|<span data-ttu-id="950a4-283">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="950a4-283">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="950a4-284">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-284">factoryResetBlocked</span></span>|<span data-ttu-id="950a4-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-285">Boolean</span></span>|<span data-ttu-id="950a4-286">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="950a4-286">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="950a4-287">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-287">screenCaptureBlocked</span></span>|<span data-ttu-id="950a4-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-288">Boolean</span></span>|<span data-ttu-id="950a4-289">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="950a4-289">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="950a4-290">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="950a4-290">deviceSharingAllowed</span></span>|<span data-ttu-id="950a4-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-291">Boolean</span></span>|<span data-ttu-id="950a4-292">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="950a4-292">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="950a4-293">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="950a4-293">storageBlockGoogleBackup</span></span>|<span data-ttu-id="950a4-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-294">Boolean</span></span>|<span data-ttu-id="950a4-295">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="950a4-295">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="950a4-296">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="950a4-296">storageBlockRemovableStorage</span></span>|<span data-ttu-id="950a4-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-297">Boolean</span></span>|<span data-ttu-id="950a4-298">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="950a4-298">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="950a4-299">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="950a4-299">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="950a4-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-300">Boolean</span></span>|<span data-ttu-id="950a4-301">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="950a4-301">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="950a4-302">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="950a4-302">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="950a4-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-303">Boolean</span></span>|<span data-ttu-id="950a4-304">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="950a4-304">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="950a4-305">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-305">voiceAssistantBlocked</span></span>|<span data-ttu-id="950a4-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-306">Boolean</span></span>|<span data-ttu-id="950a4-307">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="950a4-307">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="950a4-308">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-308">voiceDialingBlocked</span></span>|<span data-ttu-id="950a4-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-309">Boolean</span></span>|<span data-ttu-id="950a4-310">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="950a4-310">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="950a4-311">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="950a4-311">webBrowserBlockPopups</span></span>|<span data-ttu-id="950a4-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-312">Boolean</span></span>|<span data-ttu-id="950a4-313">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="950a4-313">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="950a4-314">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="950a4-314">webBrowserBlockAutofill</span></span>|<span data-ttu-id="950a4-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-315">Boolean</span></span>|<span data-ttu-id="950a4-316">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="950a4-316">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="950a4-317">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="950a4-317">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="950a4-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-318">Boolean</span></span>|<span data-ttu-id="950a4-319">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="950a4-319">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="950a4-320">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-320">webBrowserBlocked</span></span>|<span data-ttu-id="950a4-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-321">Boolean</span></span>|<span data-ttu-id="950a4-322">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="950a4-322">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="950a4-323">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="950a4-323">webBrowserCookieSettings</span></span>|[<span data-ttu-id="950a4-324">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="950a4-324">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="950a4-325">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="950a4-325">Cookie settings within the web browser.</span></span> <span data-ttu-id="950a4-326">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="950a4-326">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="950a4-327">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="950a4-327">wiFiBlocked</span></span>|<span data-ttu-id="950a4-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-328">Boolean</span></span>|<span data-ttu-id="950a4-329">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="950a4-329">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="950a4-330">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="950a4-330">appsInstallAllowList</span></span>|<span data-ttu-id="950a4-331">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="950a4-331">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="950a4-332">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="950a4-332">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="950a4-333">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="950a4-333">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="950a4-334">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="950a4-334">appsLaunchBlockList</span></span>|<span data-ttu-id="950a4-335">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="950a4-335">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="950a4-336">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="950a4-336">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="950a4-337">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="950a4-337">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="950a4-338">appsHideList</span><span class="sxs-lookup"><span data-stu-id="950a4-338">appsHideList</span></span>|<span data-ttu-id="950a4-339">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="950a4-339">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="950a4-340">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="950a4-340">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="950a4-341">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="950a4-341">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="950a4-342">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="950a4-342">securityRequireVerifyApps</span></span>|<span data-ttu-id="950a4-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="950a4-343">Boolean</span></span>|<span data-ttu-id="950a4-344">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="950a4-344">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="950a4-345">响应</span><span class="sxs-lookup"><span data-stu-id="950a4-345">Response</span></span>
<span data-ttu-id="950a4-346">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="950a4-346">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="950a4-347">示例</span><span class="sxs-lookup"><span data-stu-id="950a4-347">Example</span></span>

### <a name="request"></a><span data-ttu-id="950a4-348">请求</span><span class="sxs-lookup"><span data-stu-id="950a4-348">Request</span></span>
<span data-ttu-id="950a4-349">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="950a4-349">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="950a4-350">响应</span><span class="sxs-lookup"><span data-stu-id="950a4-350">Response</span></span>
<span data-ttu-id="950a4-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="950a4-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




