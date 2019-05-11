---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdaccae3110437b3b4dd2de0eaffddf2903db98a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33929656"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="2809f-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2809f-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2809f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2809f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2809f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2809f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2809f-106">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2809f-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2809f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2809f-107">Prerequisites</span></span>
<span data-ttu-id="2809f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2809f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2809f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2809f-110">Permission type</span></span>|<span data-ttu-id="2809f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2809f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2809f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2809f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2809f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2809f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2809f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2809f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2809f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2809f-115">Not supported.</span></span>|
|<span data-ttu-id="2809f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2809f-116">Application</span></span>|<span data-ttu-id="2809f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2809f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2809f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2809f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2809f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2809f-119">Request headers</span></span>
|<span data-ttu-id="2809f-120">标头</span><span class="sxs-lookup"><span data-stu-id="2809f-120">Header</span></span>|<span data-ttu-id="2809f-121">值</span><span class="sxs-lookup"><span data-stu-id="2809f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2809f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2809f-122">Authorization</span></span>|<span data-ttu-id="2809f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2809f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2809f-124">接受</span><span class="sxs-lookup"><span data-stu-id="2809f-124">Accept</span></span>|<span data-ttu-id="2809f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2809f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2809f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2809f-126">Request body</span></span>
<span data-ttu-id="2809f-127">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2809f-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="2809f-128">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2809f-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="2809f-129">属性</span><span class="sxs-lookup"><span data-stu-id="2809f-129">Property</span></span>|<span data-ttu-id="2809f-130">类型</span><span class="sxs-lookup"><span data-stu-id="2809f-130">Type</span></span>|<span data-ttu-id="2809f-131">说明</span><span class="sxs-lookup"><span data-stu-id="2809f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2809f-132">id</span><span class="sxs-lookup"><span data-stu-id="2809f-132">id</span></span>|<span data-ttu-id="2809f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2809f-133">String</span></span>|<span data-ttu-id="2809f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2809f-134">Key of the entity.</span></span> <span data-ttu-id="2809f-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2809f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2809f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2809f-137">DateTimeOffset</span></span>|<span data-ttu-id="2809f-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2809f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2809f-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2809f-140">roleScopeTagIds</span></span>|<span data-ttu-id="2809f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2809f-141">String collection</span></span>|<span data-ttu-id="2809f-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2809f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2809f-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2809f-144">supportsScopeTags</span></span>|<span data-ttu-id="2809f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-145">Boolean</span></span>|<span data-ttu-id="2809f-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2809f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2809f-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2809f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2809f-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2809f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2809f-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2809f-149">This property is read-only.</span></span> <span data-ttu-id="2809f-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2809f-151">createdDateTime</span></span>|<span data-ttu-id="2809f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2809f-152">DateTimeOffset</span></span>|<span data-ttu-id="2809f-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2809f-153">DateTime the object was created.</span></span> <span data-ttu-id="2809f-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-155">说明</span><span class="sxs-lookup"><span data-stu-id="2809f-155">description</span></span>|<span data-ttu-id="2809f-156">String</span><span class="sxs-lookup"><span data-stu-id="2809f-156">String</span></span>|<span data-ttu-id="2809f-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2809f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2809f-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2809f-159">displayName</span></span>|<span data-ttu-id="2809f-160">String</span><span class="sxs-lookup"><span data-stu-id="2809f-160">String</span></span>|<span data-ttu-id="2809f-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2809f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2809f-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-163">version</span><span class="sxs-lookup"><span data-stu-id="2809f-163">version</span></span>|<span data-ttu-id="2809f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2809f-164">Int32</span></span>|<span data-ttu-id="2809f-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2809f-165">Version of the device configuration.</span></span> <span data-ttu-id="2809f-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2809f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2809f-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="2809f-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="2809f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-168">Boolean</span></span>|<span data-ttu-id="2809f-169">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="2809f-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="2809f-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="2809f-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="2809f-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-171">Boolean</span></span>|<span data-ttu-id="2809f-172">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="2809f-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="2809f-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="2809f-173">appsBlockYouTube</span></span>|<span data-ttu-id="2809f-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-174">Boolean</span></span>|<span data-ttu-id="2809f-175">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="2809f-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="2809f-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-176">bluetoothBlocked</span></span>|<span data-ttu-id="2809f-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-177">Boolean</span></span>|<span data-ttu-id="2809f-178">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="2809f-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="2809f-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-179">cameraBlocked</span></span>|<span data-ttu-id="2809f-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-180">Boolean</span></span>|<span data-ttu-id="2809f-181">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="2809f-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="2809f-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="2809f-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="2809f-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-183">Boolean</span></span>|<span data-ttu-id="2809f-184">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="2809f-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="2809f-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="2809f-185">cellularBlockMessaging</span></span>|<span data-ttu-id="2809f-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-186">Boolean</span></span>|<span data-ttu-id="2809f-187">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="2809f-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="2809f-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="2809f-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="2809f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-189">Boolean</span></span>|<span data-ttu-id="2809f-190">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="2809f-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="2809f-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="2809f-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="2809f-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-192">Boolean</span></span>|<span data-ttu-id="2809f-193">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="2809f-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="2809f-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="2809f-194">compliantAppsList</span></span>|<span data-ttu-id="2809f-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2809f-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2809f-196">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="2809f-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="2809f-197">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="2809f-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="2809f-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="2809f-198">compliantAppListType</span></span>|[<span data-ttu-id="2809f-199">appListType</span><span class="sxs-lookup"><span data-stu-id="2809f-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="2809f-200">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="2809f-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="2809f-201">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="2809f-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="2809f-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="2809f-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="2809f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-203">Boolean</span></span>|<span data-ttu-id="2809f-204">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="2809f-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="2809f-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-205">locationServicesBlocked</span></span>|<span data-ttu-id="2809f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-206">Boolean</span></span>|<span data-ttu-id="2809f-207">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="2809f-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="2809f-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="2809f-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="2809f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-209">Boolean</span></span>|<span data-ttu-id="2809f-210">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="2809f-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="2809f-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="2809f-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-212">Boolean</span></span>|<span data-ttu-id="2809f-213">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="2809f-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="2809f-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="2809f-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="2809f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-215">Boolean</span></span>|<span data-ttu-id="2809f-216">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="2809f-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="2809f-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="2809f-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="2809f-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-218">Boolean</span></span>|<span data-ttu-id="2809f-219">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="2809f-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="2809f-220">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="2809f-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="2809f-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-221">Boolean</span></span>|<span data-ttu-id="2809f-222">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2809f-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="2809f-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="2809f-223">kioskModeApps</span></span>|<span data-ttu-id="2809f-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2809f-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2809f-225">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="2809f-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="2809f-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2809f-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2809f-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-227">nfcBlocked</span></span>|<span data-ttu-id="2809f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-228">Boolean</span></span>|<span data-ttu-id="2809f-229">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="2809f-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="2809f-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2809f-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2809f-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-231">Boolean</span></span>|<span data-ttu-id="2809f-232">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="2809f-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2809f-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2809f-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="2809f-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-234">Boolean</span></span>|<span data-ttu-id="2809f-235">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="2809f-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="2809f-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2809f-236">passwordExpirationDays</span></span>|<span data-ttu-id="2809f-237">Int32</span><span class="sxs-lookup"><span data-stu-id="2809f-237">Int32</span></span>|<span data-ttu-id="2809f-238">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2809f-238">Number of days before the password expires.</span></span> <span data-ttu-id="2809f-239">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="2809f-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2809f-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2809f-240">passwordMinimumLength</span></span>|<span data-ttu-id="2809f-241">Int32</span><span class="sxs-lookup"><span data-stu-id="2809f-241">Int32</span></span>|<span data-ttu-id="2809f-242">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="2809f-242">Minimum length of passwords.</span></span> <span data-ttu-id="2809f-243">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="2809f-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2809f-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2809f-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2809f-245">Int32</span><span class="sxs-lookup"><span data-stu-id="2809f-245">Int32</span></span>|<span data-ttu-id="2809f-246">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="2809f-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2809f-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2809f-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2809f-248">Int32</span><span class="sxs-lookup"><span data-stu-id="2809f-248">Int32</span></span>|<span data-ttu-id="2809f-249">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2809f-249">Number of previous passwords to block.</span></span> <span data-ttu-id="2809f-250">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="2809f-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2809f-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2809f-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2809f-252">Int32</span><span class="sxs-lookup"><span data-stu-id="2809f-252">Int32</span></span>|<span data-ttu-id="2809f-253">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="2809f-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="2809f-254">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2809f-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2809f-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2809f-255">passwordRequiredType</span></span>|[<span data-ttu-id="2809f-256">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2809f-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="2809f-257">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2809f-257">Type of password that is required.</span></span> <span data-ttu-id="2809f-258">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="2809f-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="2809f-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2809f-259">passwordRequired</span></span>|<span data-ttu-id="2809f-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-260">Boolean</span></span>|<span data-ttu-id="2809f-261">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="2809f-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="2809f-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-262">powerOffBlocked</span></span>|<span data-ttu-id="2809f-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-263">Boolean</span></span>|<span data-ttu-id="2809f-264">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="2809f-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="2809f-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-265">factoryResetBlocked</span></span>|<span data-ttu-id="2809f-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-266">Boolean</span></span>|<span data-ttu-id="2809f-267">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="2809f-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="2809f-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-268">screenCaptureBlocked</span></span>|<span data-ttu-id="2809f-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-269">Boolean</span></span>|<span data-ttu-id="2809f-270">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="2809f-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="2809f-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="2809f-271">deviceSharingAllowed</span></span>|<span data-ttu-id="2809f-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-272">Boolean</span></span>|<span data-ttu-id="2809f-273">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="2809f-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="2809f-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="2809f-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="2809f-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-275">Boolean</span></span>|<span data-ttu-id="2809f-276">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="2809f-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="2809f-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="2809f-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="2809f-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-278">Boolean</span></span>|<span data-ttu-id="2809f-279">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="2809f-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="2809f-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="2809f-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="2809f-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-281">Boolean</span></span>|<span data-ttu-id="2809f-282">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="2809f-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="2809f-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="2809f-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="2809f-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-284">Boolean</span></span>|<span data-ttu-id="2809f-285">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="2809f-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="2809f-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="2809f-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-287">Boolean</span></span>|<span data-ttu-id="2809f-288">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="2809f-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="2809f-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-289">voiceDialingBlocked</span></span>|<span data-ttu-id="2809f-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-290">Boolean</span></span>|<span data-ttu-id="2809f-291">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="2809f-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="2809f-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="2809f-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="2809f-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-293">Boolean</span></span>|<span data-ttu-id="2809f-294">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="2809f-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="2809f-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="2809f-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="2809f-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-296">Boolean</span></span>|<span data-ttu-id="2809f-297">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="2809f-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="2809f-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="2809f-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="2809f-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-299">Boolean</span></span>|<span data-ttu-id="2809f-300">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="2809f-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="2809f-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-301">webBrowserBlocked</span></span>|<span data-ttu-id="2809f-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-302">Boolean</span></span>|<span data-ttu-id="2809f-303">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="2809f-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="2809f-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="2809f-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="2809f-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="2809f-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="2809f-306">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="2809f-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="2809f-307">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="2809f-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="2809f-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="2809f-308">wiFiBlocked</span></span>|<span data-ttu-id="2809f-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-309">Boolean</span></span>|<span data-ttu-id="2809f-310">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="2809f-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="2809f-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="2809f-311">appsInstallAllowList</span></span>|<span data-ttu-id="2809f-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2809f-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2809f-313">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="2809f-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="2809f-314">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2809f-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2809f-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="2809f-315">appsLaunchBlockList</span></span>|<span data-ttu-id="2809f-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2809f-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2809f-317">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="2809f-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="2809f-318">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2809f-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2809f-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="2809f-319">appsHideList</span></span>|<span data-ttu-id="2809f-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2809f-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2809f-321">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="2809f-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="2809f-322">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2809f-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2809f-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2809f-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="2809f-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="2809f-324">Boolean</span></span>|<span data-ttu-id="2809f-325">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="2809f-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="2809f-326">响应</span><span class="sxs-lookup"><span data-stu-id="2809f-326">Response</span></span>
<span data-ttu-id="2809f-327">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2809f-327">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2809f-328">示例</span><span class="sxs-lookup"><span data-stu-id="2809f-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="2809f-329">请求</span><span class="sxs-lookup"><span data-stu-id="2809f-329">Request</span></span>
<span data-ttu-id="2809f-330">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2809f-330">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2809f-331">响应</span><span class="sxs-lookup"><span data-stu-id="2809f-331">Response</span></span>
<span data-ttu-id="2809f-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2809f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




