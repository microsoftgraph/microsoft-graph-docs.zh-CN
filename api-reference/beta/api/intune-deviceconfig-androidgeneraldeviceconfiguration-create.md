---
title: 创建 androidGeneralDeviceConfiguration
description: 创建新的 androidGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ea439b593f1e0e8d26cf43450a104806140634f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796785"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="25bb6-103">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="25bb6-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="25bb6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25bb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25bb6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25bb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25bb6-106">创建新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25bb6-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25bb6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="25bb6-107">Prerequisites</span></span>
<span data-ttu-id="25bb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25bb6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25bb6-110">Permission type</span></span>|<span data-ttu-id="25bb6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="25bb6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25bb6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25bb6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25bb6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25bb6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25bb6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25bb6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25bb6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25bb6-115">Not supported.</span></span>|
|<span data-ttu-id="25bb6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25bb6-116">Application</span></span>|<span data-ttu-id="25bb6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="25bb6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25bb6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25bb6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="25bb6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25bb6-119">Request headers</span></span>
|<span data-ttu-id="25bb6-120">标头</span><span class="sxs-lookup"><span data-stu-id="25bb6-120">Header</span></span>|<span data-ttu-id="25bb6-121">值</span><span class="sxs-lookup"><span data-stu-id="25bb6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25bb6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25bb6-122">Authorization</span></span>|<span data-ttu-id="25bb6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25bb6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25bb6-124">接受</span><span class="sxs-lookup"><span data-stu-id="25bb6-124">Accept</span></span>|<span data-ttu-id="25bb6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25bb6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25bb6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="25bb6-126">Request body</span></span>
<span data-ttu-id="25bb6-127">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25bb6-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="25bb6-128">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25bb6-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="25bb6-129">属性</span><span class="sxs-lookup"><span data-stu-id="25bb6-129">Property</span></span>|<span data-ttu-id="25bb6-130">类型</span><span class="sxs-lookup"><span data-stu-id="25bb6-130">Type</span></span>|<span data-ttu-id="25bb6-131">说明</span><span class="sxs-lookup"><span data-stu-id="25bb6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25bb6-132">id</span><span class="sxs-lookup"><span data-stu-id="25bb6-132">id</span></span>|<span data-ttu-id="25bb6-133">String</span><span class="sxs-lookup"><span data-stu-id="25bb6-133">String</span></span>|<span data-ttu-id="25bb6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="25bb6-134">Key of the entity.</span></span> <span data-ttu-id="25bb6-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25bb6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="25bb6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25bb6-137">DateTimeOffset</span></span>|<span data-ttu-id="25bb6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="25bb6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="25bb6-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25bb6-140">roleScopeTagIds</span></span>|<span data-ttu-id="25bb6-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="25bb6-141">String collection</span></span>|<span data-ttu-id="25bb6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="25bb6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="25bb6-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="25bb6-144">supportsScopeTags</span></span>|<span data-ttu-id="25bb6-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-145">Boolean</span></span>|<span data-ttu-id="25bb6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="25bb6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="25bb6-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="25bb6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="25bb6-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="25bb6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="25bb6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="25bb6-149">This property is read-only.</span></span> <span data-ttu-id="25bb6-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25bb6-151">createdDateTime</span></span>|<span data-ttu-id="25bb6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25bb6-152">DateTimeOffset</span></span>|<span data-ttu-id="25bb6-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="25bb6-153">DateTime the object was created.</span></span> <span data-ttu-id="25bb6-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-155">description</span><span class="sxs-lookup"><span data-stu-id="25bb6-155">description</span></span>|<span data-ttu-id="25bb6-156">String</span><span class="sxs-lookup"><span data-stu-id="25bb6-156">String</span></span>|<span data-ttu-id="25bb6-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="25bb6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25bb6-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="25bb6-159">displayName</span></span>|<span data-ttu-id="25bb6-160">String</span><span class="sxs-lookup"><span data-stu-id="25bb6-160">String</span></span>|<span data-ttu-id="25bb6-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="25bb6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25bb6-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-163">version</span><span class="sxs-lookup"><span data-stu-id="25bb6-163">version</span></span>|<span data-ttu-id="25bb6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="25bb6-164">Int32</span></span>|<span data-ttu-id="25bb6-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="25bb6-165">Version of the device configuration.</span></span> <span data-ttu-id="25bb6-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25bb6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25bb6-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="25bb6-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="25bb6-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-168">Boolean</span></span>|<span data-ttu-id="25bb6-169">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="25bb6-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="25bb6-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="25bb6-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="25bb6-171">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-171">Boolean</span></span>|<span data-ttu-id="25bb6-172">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="25bb6-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="25bb6-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="25bb6-173">appsBlockYouTube</span></span>|<span data-ttu-id="25bb6-174">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-174">Boolean</span></span>|<span data-ttu-id="25bb6-175">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="25bb6-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="25bb6-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-176">bluetoothBlocked</span></span>|<span data-ttu-id="25bb6-177">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-177">Boolean</span></span>|<span data-ttu-id="25bb6-178">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="25bb6-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="25bb6-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-179">cameraBlocked</span></span>|<span data-ttu-id="25bb6-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-180">Boolean</span></span>|<span data-ttu-id="25bb6-181">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="25bb6-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="25bb6-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="25bb6-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="25bb6-183">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-183">Boolean</span></span>|<span data-ttu-id="25bb6-184">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="25bb6-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="25bb6-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="25bb6-185">cellularBlockMessaging</span></span>|<span data-ttu-id="25bb6-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-186">Boolean</span></span>|<span data-ttu-id="25bb6-187">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="25bb6-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="25bb6-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="25bb6-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="25bb6-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-189">Boolean</span></span>|<span data-ttu-id="25bb6-190">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="25bb6-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="25bb6-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="25bb6-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="25bb6-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-192">Boolean</span></span>|<span data-ttu-id="25bb6-193">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="25bb6-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="25bb6-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="25bb6-194">compliantAppsList</span></span>|<span data-ttu-id="25bb6-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25bb6-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="25bb6-196">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="25bb6-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="25bb6-197">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="25bb6-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="25bb6-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="25bb6-198">compliantAppListType</span></span>|[<span data-ttu-id="25bb6-199">appListType</span><span class="sxs-lookup"><span data-stu-id="25bb6-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="25bb6-200">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="25bb6-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="25bb6-201">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="25bb6-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="25bb6-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="25bb6-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="25bb6-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-203">Boolean</span></span>|<span data-ttu-id="25bb6-204">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="25bb6-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="25bb6-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-205">locationServicesBlocked</span></span>|<span data-ttu-id="25bb6-206">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-206">Boolean</span></span>|<span data-ttu-id="25bb6-207">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="25bb6-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="25bb6-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="25bb6-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="25bb6-209">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-209">Boolean</span></span>|<span data-ttu-id="25bb6-210">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="25bb6-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="25bb6-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="25bb6-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-212">Boolean</span></span>|<span data-ttu-id="25bb6-213">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="25bb6-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="25bb6-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="25bb6-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="25bb6-215">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-215">Boolean</span></span>|<span data-ttu-id="25bb6-216">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="25bb6-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="25bb6-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="25bb6-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="25bb6-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="25bb6-218">Boolean</span></span>|<span data-ttu-id="25bb6-219">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="25bb6-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="25bb6-220">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="25bb6-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="25bb6-221">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-221">Boolean</span></span>|<span data-ttu-id="25bb6-222">指示在 KNOX 模式下是否阻止更改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="25bb6-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="25bb6-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="25bb6-223">kioskModeApps</span></span>|<span data-ttu-id="25bb6-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25bb6-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="25bb6-225">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="25bb6-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="25bb6-226">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="25bb6-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="25bb6-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-227">nfcBlocked</span></span>|<span data-ttu-id="25bb6-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-228">Boolean</span></span>|<span data-ttu-id="25bb6-229">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="25bb6-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="25bb6-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="25bb6-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="25bb6-231">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-231">Boolean</span></span>|<span data-ttu-id="25bb6-232">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="25bb6-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="25bb6-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="25bb6-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="25bb6-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-234">Boolean</span></span>|<span data-ttu-id="25bb6-235">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="25bb6-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="25bb6-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="25bb6-236">passwordExpirationDays</span></span>|<span data-ttu-id="25bb6-237">Int32</span><span class="sxs-lookup"><span data-stu-id="25bb6-237">Int32</span></span>|<span data-ttu-id="25bb6-238">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="25bb6-238">Number of days before the password expires.</span></span> <span data-ttu-id="25bb6-239">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="25bb6-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="25bb6-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="25bb6-240">passwordMinimumLength</span></span>|<span data-ttu-id="25bb6-241">Int32</span><span class="sxs-lookup"><span data-stu-id="25bb6-241">Int32</span></span>|<span data-ttu-id="25bb6-242">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="25bb6-242">Minimum length of passwords.</span></span> <span data-ttu-id="25bb6-243">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="25bb6-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="25bb6-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="25bb6-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="25bb6-245">Int32</span><span class="sxs-lookup"><span data-stu-id="25bb6-245">Int32</span></span>|<span data-ttu-id="25bb6-246">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="25bb6-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="25bb6-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="25bb6-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="25bb6-248">Int32</span><span class="sxs-lookup"><span data-stu-id="25bb6-248">Int32</span></span>|<span data-ttu-id="25bb6-249">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="25bb6-249">Number of previous passwords to block.</span></span> <span data-ttu-id="25bb6-250">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="25bb6-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="25bb6-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="25bb6-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="25bb6-252">Int32</span><span class="sxs-lookup"><span data-stu-id="25bb6-252">Int32</span></span>|<span data-ttu-id="25bb6-253">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="25bb6-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="25bb6-254">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="25bb6-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="25bb6-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="25bb6-255">passwordRequiredType</span></span>|[<span data-ttu-id="25bb6-256">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="25bb6-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="25bb6-257">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="25bb6-257">Type of password that is required.</span></span> <span data-ttu-id="25bb6-258">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="25bb6-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="25bb6-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="25bb6-259">passwordRequired</span></span>|<span data-ttu-id="25bb6-260">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-260">Boolean</span></span>|<span data-ttu-id="25bb6-261">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="25bb6-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="25bb6-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-262">powerOffBlocked</span></span>|<span data-ttu-id="25bb6-263">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-263">Boolean</span></span>|<span data-ttu-id="25bb6-264">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="25bb6-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="25bb6-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-265">factoryResetBlocked</span></span>|<span data-ttu-id="25bb6-266">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-266">Boolean</span></span>|<span data-ttu-id="25bb6-267">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="25bb6-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="25bb6-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-268">screenCaptureBlocked</span></span>|<span data-ttu-id="25bb6-269">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-269">Boolean</span></span>|<span data-ttu-id="25bb6-270">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="25bb6-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="25bb6-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="25bb6-271">deviceSharingAllowed</span></span>|<span data-ttu-id="25bb6-272">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-272">Boolean</span></span>|<span data-ttu-id="25bb6-273">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="25bb6-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="25bb6-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="25bb6-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="25bb6-275">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-275">Boolean</span></span>|<span data-ttu-id="25bb6-276">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="25bb6-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="25bb6-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="25bb6-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="25bb6-278">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-278">Boolean</span></span>|<span data-ttu-id="25bb6-279">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="25bb6-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="25bb6-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="25bb6-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="25bb6-281">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-281">Boolean</span></span>|<span data-ttu-id="25bb6-282">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="25bb6-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="25bb6-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="25bb6-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="25bb6-284">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-284">Boolean</span></span>|<span data-ttu-id="25bb6-285">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="25bb6-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="25bb6-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="25bb6-287">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-287">Boolean</span></span>|<span data-ttu-id="25bb6-288">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="25bb6-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="25bb6-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-289">voiceDialingBlocked</span></span>|<span data-ttu-id="25bb6-290">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-290">Boolean</span></span>|<span data-ttu-id="25bb6-291">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="25bb6-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="25bb6-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="25bb6-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="25bb6-293">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-293">Boolean</span></span>|<span data-ttu-id="25bb6-294">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="25bb6-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="25bb6-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="25bb6-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="25bb6-296">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-296">Boolean</span></span>|<span data-ttu-id="25bb6-297">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="25bb6-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="25bb6-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="25bb6-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="25bb6-299">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-299">Boolean</span></span>|<span data-ttu-id="25bb6-300">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="25bb6-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="25bb6-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-301">webBrowserBlocked</span></span>|<span data-ttu-id="25bb6-302">布尔值</span><span class="sxs-lookup"><span data-stu-id="25bb6-302">Boolean</span></span>|<span data-ttu-id="25bb6-303">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="25bb6-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="25bb6-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="25bb6-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="25bb6-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="25bb6-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="25bb6-306">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="25bb6-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="25bb6-307">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="25bb6-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="25bb6-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="25bb6-308">wiFiBlocked</span></span>|<span data-ttu-id="25bb6-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="25bb6-309">Boolean</span></span>|<span data-ttu-id="25bb6-310">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="25bb6-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="25bb6-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="25bb6-311">appsInstallAllowList</span></span>|<span data-ttu-id="25bb6-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25bb6-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="25bb6-313">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="25bb6-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="25bb6-314">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="25bb6-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="25bb6-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="25bb6-315">appsLaunchBlockList</span></span>|<span data-ttu-id="25bb6-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25bb6-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="25bb6-317">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="25bb6-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="25bb6-318">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="25bb6-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="25bb6-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="25bb6-319">appsHideList</span></span>|<span data-ttu-id="25bb6-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25bb6-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="25bb6-321">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="25bb6-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="25bb6-322">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="25bb6-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="25bb6-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="25bb6-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="25bb6-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="25bb6-324">Boolean</span></span>|<span data-ttu-id="25bb6-325">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="25bb6-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="25bb6-326">响应</span><span class="sxs-lookup"><span data-stu-id="25bb6-326">Response</span></span>
<span data-ttu-id="25bb6-327">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25bb6-327">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25bb6-328">示例</span><span class="sxs-lookup"><span data-stu-id="25bb6-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="25bb6-329">请求</span><span class="sxs-lookup"><span data-stu-id="25bb6-329">Request</span></span>
<span data-ttu-id="25bb6-330">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25bb6-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="25bb6-331">响应</span><span class="sxs-lookup"><span data-stu-id="25bb6-331">Response</span></span>
<span data-ttu-id="25bb6-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25bb6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





