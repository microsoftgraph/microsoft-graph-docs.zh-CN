---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a96b820670ee86fb425f128d964382df951e70b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143762"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="4f764-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f764-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4f764-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f764-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f764-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f764-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f764-106">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f764-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f764-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f764-107">Prerequisites</span></span>
<span data-ttu-id="4f764-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4f764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4f764-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f764-110">Permission type</span></span>|<span data-ttu-id="4f764-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4f764-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f764-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f764-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f764-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f764-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f764-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f764-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f764-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f764-115">Not supported.</span></span>|
|<span data-ttu-id="4f764-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f764-116">Application</span></span>|<span data-ttu-id="4f764-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f764-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f764-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f764-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4f764-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f764-119">Request headers</span></span>
|<span data-ttu-id="4f764-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f764-120">Header</span></span>|<span data-ttu-id="4f764-121">值</span><span class="sxs-lookup"><span data-stu-id="4f764-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f764-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f764-122">Authorization</span></span>|<span data-ttu-id="4f764-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f764-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f764-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f764-124">Accept</span></span>|<span data-ttu-id="4f764-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f764-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f764-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f764-126">Request body</span></span>
<span data-ttu-id="4f764-127">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f764-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="4f764-128">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4f764-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="4f764-129">属性</span><span class="sxs-lookup"><span data-stu-id="4f764-129">Property</span></span>|<span data-ttu-id="4f764-130">类型</span><span class="sxs-lookup"><span data-stu-id="4f764-130">Type</span></span>|<span data-ttu-id="4f764-131">说明</span><span class="sxs-lookup"><span data-stu-id="4f764-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f764-132">id</span><span class="sxs-lookup"><span data-stu-id="4f764-132">id</span></span>|<span data-ttu-id="4f764-133">String</span><span class="sxs-lookup"><span data-stu-id="4f764-133">String</span></span>|<span data-ttu-id="4f764-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4f764-134">Key of the entity.</span></span> <span data-ttu-id="4f764-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f764-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4f764-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f764-137">DateTimeOffset</span></span>|<span data-ttu-id="4f764-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4f764-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4f764-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f764-140">roleScopeTagIds</span></span>|<span data-ttu-id="4f764-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4f764-141">String collection</span></span>|<span data-ttu-id="4f764-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4f764-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f764-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4f764-144">supportsScopeTags</span></span>|<span data-ttu-id="4f764-145">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-145">Boolean</span></span>|<span data-ttu-id="4f764-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4f764-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4f764-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4f764-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4f764-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4f764-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4f764-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4f764-149">This property is read-only.</span></span> <span data-ttu-id="4f764-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f764-151">createdDateTime</span></span>|<span data-ttu-id="4f764-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f764-152">DateTimeOffset</span></span>|<span data-ttu-id="4f764-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4f764-153">DateTime the object was created.</span></span> <span data-ttu-id="4f764-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-155">description</span><span class="sxs-lookup"><span data-stu-id="4f764-155">description</span></span>|<span data-ttu-id="4f764-156">String</span><span class="sxs-lookup"><span data-stu-id="4f764-156">String</span></span>|<span data-ttu-id="4f764-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4f764-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f764-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4f764-159">displayName</span></span>|<span data-ttu-id="4f764-160">String</span><span class="sxs-lookup"><span data-stu-id="4f764-160">String</span></span>|<span data-ttu-id="4f764-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4f764-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f764-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-163">version</span><span class="sxs-lookup"><span data-stu-id="4f764-163">version</span></span>|<span data-ttu-id="4f764-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4f764-164">Int32</span></span>|<span data-ttu-id="4f764-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4f764-165">Version of the device configuration.</span></span> <span data-ttu-id="4f764-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f764-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f764-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="4f764-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="4f764-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-168">Boolean</span></span>|<span data-ttu-id="4f764-169">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="4f764-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="4f764-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4f764-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="4f764-171">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-171">Boolean</span></span>|<span data-ttu-id="4f764-172">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="4f764-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="4f764-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="4f764-173">appsBlockYouTube</span></span>|<span data-ttu-id="4f764-174">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-174">Boolean</span></span>|<span data-ttu-id="4f764-175">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="4f764-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="4f764-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-176">bluetoothBlocked</span></span>|<span data-ttu-id="4f764-177">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-177">Boolean</span></span>|<span data-ttu-id="4f764-178">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="4f764-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="4f764-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-179">cameraBlocked</span></span>|<span data-ttu-id="4f764-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-180">Boolean</span></span>|<span data-ttu-id="4f764-181">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="4f764-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="4f764-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="4f764-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="4f764-183">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-183">Boolean</span></span>|<span data-ttu-id="4f764-184">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="4f764-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="4f764-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="4f764-185">cellularBlockMessaging</span></span>|<span data-ttu-id="4f764-186">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-186">Boolean</span></span>|<span data-ttu-id="4f764-187">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="4f764-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="4f764-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="4f764-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="4f764-189">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-189">Boolean</span></span>|<span data-ttu-id="4f764-190">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="4f764-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="4f764-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="4f764-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="4f764-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-192">Boolean</span></span>|<span data-ttu-id="4f764-193">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="4f764-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="4f764-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4f764-194">compliantAppsList</span></span>|<span data-ttu-id="4f764-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f764-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4f764-196">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="4f764-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4f764-197">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4f764-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4f764-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4f764-198">compliantAppListType</span></span>|[<span data-ttu-id="4f764-199">appListType</span><span class="sxs-lookup"><span data-stu-id="4f764-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4f764-200">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="4f764-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="4f764-201">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="4f764-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4f764-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4f764-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4f764-203">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-203">Boolean</span></span>|<span data-ttu-id="4f764-204">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="4f764-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4f764-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-205">locationServicesBlocked</span></span>|<span data-ttu-id="4f764-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-206">Boolean</span></span>|<span data-ttu-id="4f764-207">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="4f764-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4f764-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="4f764-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="4f764-209">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-209">Boolean</span></span>|<span data-ttu-id="4f764-210">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="4f764-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="4f764-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="4f764-212">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-212">Boolean</span></span>|<span data-ttu-id="4f764-213">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="4f764-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="4f764-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="4f764-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="4f764-215">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-215">Boolean</span></span>|<span data-ttu-id="4f764-216">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="4f764-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="4f764-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="4f764-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="4f764-218">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-218">Boolean</span></span>|<span data-ttu-id="4f764-219">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="4f764-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="4f764-220">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="4f764-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="4f764-221">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-221">Boolean</span></span>|<span data-ttu-id="4f764-222">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4f764-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="4f764-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="4f764-223">kioskModeApps</span></span>|<span data-ttu-id="4f764-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f764-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4f764-225">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="4f764-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="4f764-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4f764-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4f764-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-227">nfcBlocked</span></span>|<span data-ttu-id="4f764-228">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-228">Boolean</span></span>|<span data-ttu-id="4f764-229">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="4f764-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4f764-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="4f764-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="4f764-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-231">Boolean</span></span>|<span data-ttu-id="4f764-232">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="4f764-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="4f764-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="4f764-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="4f764-234">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-234">Boolean</span></span>|<span data-ttu-id="4f764-235">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="4f764-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="4f764-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4f764-236">passwordExpirationDays</span></span>|<span data-ttu-id="4f764-237">Int32</span><span class="sxs-lookup"><span data-stu-id="4f764-237">Int32</span></span>|<span data-ttu-id="4f764-238">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4f764-238">Number of days before the password expires.</span></span> <span data-ttu-id="4f764-239">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="4f764-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4f764-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4f764-240">passwordMinimumLength</span></span>|<span data-ttu-id="4f764-241">Int32</span><span class="sxs-lookup"><span data-stu-id="4f764-241">Int32</span></span>|<span data-ttu-id="4f764-242">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4f764-242">Minimum length of passwords.</span></span> <span data-ttu-id="4f764-243">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="4f764-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4f764-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4f764-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4f764-245">Int32</span><span class="sxs-lookup"><span data-stu-id="4f764-245">Int32</span></span>|<span data-ttu-id="4f764-246">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4f764-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4f764-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4f764-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4f764-248">Int32</span><span class="sxs-lookup"><span data-stu-id="4f764-248">Int32</span></span>|<span data-ttu-id="4f764-249">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4f764-249">Number of previous passwords to block.</span></span> <span data-ttu-id="4f764-250">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="4f764-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4f764-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4f764-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4f764-252">Int32</span><span class="sxs-lookup"><span data-stu-id="4f764-252">Int32</span></span>|<span data-ttu-id="4f764-253">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="4f764-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="4f764-254">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="4f764-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4f764-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4f764-255">passwordRequiredType</span></span>|[<span data-ttu-id="4f764-256">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4f764-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="4f764-257">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4f764-257">Type of password that is required.</span></span> <span data-ttu-id="4f764-258">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="4f764-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="4f764-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4f764-259">passwordRequired</span></span>|<span data-ttu-id="4f764-260">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-260">Boolean</span></span>|<span data-ttu-id="4f764-261">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4f764-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4f764-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-262">powerOffBlocked</span></span>|<span data-ttu-id="4f764-263">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-263">Boolean</span></span>|<span data-ttu-id="4f764-264">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="4f764-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="4f764-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-265">factoryResetBlocked</span></span>|<span data-ttu-id="4f764-266">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-266">Boolean</span></span>|<span data-ttu-id="4f764-267">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="4f764-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="4f764-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-268">screenCaptureBlocked</span></span>|<span data-ttu-id="4f764-269">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-269">Boolean</span></span>|<span data-ttu-id="4f764-270">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="4f764-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4f764-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="4f764-271">deviceSharingAllowed</span></span>|<span data-ttu-id="4f764-272">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-272">Boolean</span></span>|<span data-ttu-id="4f764-273">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="4f764-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="4f764-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="4f764-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="4f764-275">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-275">Boolean</span></span>|<span data-ttu-id="4f764-276">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="4f764-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="4f764-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4f764-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4f764-278">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-278">Boolean</span></span>|<span data-ttu-id="4f764-279">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="4f764-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="4f764-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="4f764-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="4f764-281">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-281">Boolean</span></span>|<span data-ttu-id="4f764-282">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="4f764-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="4f764-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="4f764-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="4f764-284">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-284">Boolean</span></span>|<span data-ttu-id="4f764-285">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="4f764-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="4f764-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="4f764-287">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-287">Boolean</span></span>|<span data-ttu-id="4f764-288">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="4f764-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="4f764-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-289">voiceDialingBlocked</span></span>|<span data-ttu-id="4f764-290">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-290">Boolean</span></span>|<span data-ttu-id="4f764-291">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="4f764-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="4f764-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="4f764-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="4f764-293">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-293">Boolean</span></span>|<span data-ttu-id="4f764-294">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="4f764-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="4f764-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="4f764-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="4f764-296">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-296">Boolean</span></span>|<span data-ttu-id="4f764-297">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="4f764-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="4f764-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="4f764-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="4f764-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-299">Boolean</span></span>|<span data-ttu-id="4f764-300">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="4f764-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="4f764-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-301">webBrowserBlocked</span></span>|<span data-ttu-id="4f764-302">布尔</span><span class="sxs-lookup"><span data-stu-id="4f764-302">Boolean</span></span>|<span data-ttu-id="4f764-303">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="4f764-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4f764-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="4f764-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="4f764-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="4f764-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="4f764-306">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="4f764-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="4f764-307">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="4f764-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="4f764-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="4f764-308">wiFiBlocked</span></span>|<span data-ttu-id="4f764-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-309">Boolean</span></span>|<span data-ttu-id="4f764-310">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="4f764-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="4f764-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="4f764-311">appsInstallAllowList</span></span>|<span data-ttu-id="4f764-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f764-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4f764-313">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="4f764-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="4f764-314">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4f764-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4f764-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="4f764-315">appsLaunchBlockList</span></span>|<span data-ttu-id="4f764-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f764-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4f764-317">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="4f764-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="4f764-318">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4f764-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4f764-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="4f764-319">appsHideList</span></span>|<span data-ttu-id="4f764-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f764-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4f764-321">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="4f764-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="4f764-322">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4f764-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4f764-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4f764-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="4f764-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f764-324">Boolean</span></span>|<span data-ttu-id="4f764-325">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="4f764-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="4f764-326">响应</span><span class="sxs-lookup"><span data-stu-id="4f764-326">Response</span></span>
<span data-ttu-id="4f764-327">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f764-327">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f764-328">示例</span><span class="sxs-lookup"><span data-stu-id="4f764-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f764-329">请求</span><span class="sxs-lookup"><span data-stu-id="4f764-329">Request</span></span>
<span data-ttu-id="4f764-330">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f764-330">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3161

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="4f764-331">响应</span><span class="sxs-lookup"><span data-stu-id="4f764-331">Response</span></span>
<span data-ttu-id="4f764-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f764-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




