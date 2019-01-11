---
title: 创建 androidGeneralDeviceConfiguration
description: 创建新的 androidGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 779b93ce25eb9fe5044a166a78ac7d02ab77201c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842439"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="3a540-103">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a540-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="3a540-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3a540-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a540-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3a540-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a540-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3a540-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a540-107">创建新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a540-107">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a540-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3a540-108">Prerequisites</span></span>
<span data-ttu-id="3a540-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3a540-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a540-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a540-111">Permission type</span></span>|<span data-ttu-id="3a540-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3a540-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a540-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a540-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a540-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a540-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a540-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a540-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a540-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a540-116">Not supported.</span></span>|
|<span data-ttu-id="3a540-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a540-117">Application</span></span>|<span data-ttu-id="3a540-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a540-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a540-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a540-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3a540-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a540-120">Request headers</span></span>
|<span data-ttu-id="3a540-121">标头</span><span class="sxs-lookup"><span data-stu-id="3a540-121">Header</span></span>|<span data-ttu-id="3a540-122">值</span><span class="sxs-lookup"><span data-stu-id="3a540-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a540-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a540-123">Authorization</span></span>|<span data-ttu-id="3a540-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3a540-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a540-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a540-125">Accept</span></span>|<span data-ttu-id="3a540-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a540-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a540-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a540-127">Request body</span></span>
<span data-ttu-id="3a540-128">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a540-128">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="3a540-129">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3a540-129">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="3a540-130">属性</span><span class="sxs-lookup"><span data-stu-id="3a540-130">Property</span></span>|<span data-ttu-id="3a540-131">类型</span><span class="sxs-lookup"><span data-stu-id="3a540-131">Type</span></span>|<span data-ttu-id="3a540-132">说明</span><span class="sxs-lookup"><span data-stu-id="3a540-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a540-133">id</span><span class="sxs-lookup"><span data-stu-id="3a540-133">id</span></span>|<span data-ttu-id="3a540-134">String</span><span class="sxs-lookup"><span data-stu-id="3a540-134">String</span></span>|<span data-ttu-id="3a540-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3a540-135">Key of the entity.</span></span> <span data-ttu-id="3a540-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a540-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3a540-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a540-138">DateTimeOffset</span></span>|<span data-ttu-id="3a540-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3a540-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3a540-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a540-141">roleScopeTagIds</span></span>|<span data-ttu-id="3a540-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="3a540-142">String collection</span></span>|<span data-ttu-id="3a540-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="3a540-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a540-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3a540-145">supportsScopeTags</span></span>|<span data-ttu-id="3a540-146">布尔</span><span class="sxs-lookup"><span data-stu-id="3a540-146">Boolean</span></span>|<span data-ttu-id="3a540-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="3a540-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3a540-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="3a540-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3a540-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="3a540-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3a540-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3a540-150">This property is read-only.</span></span> <span data-ttu-id="3a540-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a540-152">createdDateTime</span></span>|<span data-ttu-id="3a540-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a540-153">DateTimeOffset</span></span>|<span data-ttu-id="3a540-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3a540-154">DateTime the object was created.</span></span> <span data-ttu-id="3a540-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-156">description</span><span class="sxs-lookup"><span data-stu-id="3a540-156">description</span></span>|<span data-ttu-id="3a540-157">String</span><span class="sxs-lookup"><span data-stu-id="3a540-157">String</span></span>|<span data-ttu-id="3a540-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3a540-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a540-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3a540-160">displayName</span></span>|<span data-ttu-id="3a540-161">String</span><span class="sxs-lookup"><span data-stu-id="3a540-161">String</span></span>|<span data-ttu-id="3a540-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3a540-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a540-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-164">version</span><span class="sxs-lookup"><span data-stu-id="3a540-164">version</span></span>|<span data-ttu-id="3a540-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3a540-165">Int32</span></span>|<span data-ttu-id="3a540-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3a540-166">Version of the device configuration.</span></span> <span data-ttu-id="3a540-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a540-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a540-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="3a540-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="3a540-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-169">Boolean</span></span>|<span data-ttu-id="3a540-170">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="3a540-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="3a540-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="3a540-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="3a540-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-172">Boolean</span></span>|<span data-ttu-id="3a540-173">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="3a540-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="3a540-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="3a540-174">appsBlockYouTube</span></span>|<span data-ttu-id="3a540-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-175">Boolean</span></span>|<span data-ttu-id="3a540-176">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="3a540-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="3a540-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-177">bluetoothBlocked</span></span>|<span data-ttu-id="3a540-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-178">Boolean</span></span>|<span data-ttu-id="3a540-179">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="3a540-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="3a540-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-180">cameraBlocked</span></span>|<span data-ttu-id="3a540-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-181">Boolean</span></span>|<span data-ttu-id="3a540-182">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="3a540-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="3a540-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="3a540-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="3a540-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-184">Boolean</span></span>|<span data-ttu-id="3a540-185">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="3a540-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="3a540-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="3a540-186">cellularBlockMessaging</span></span>|<span data-ttu-id="3a540-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-187">Boolean</span></span>|<span data-ttu-id="3a540-188">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="3a540-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="3a540-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="3a540-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="3a540-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-190">Boolean</span></span>|<span data-ttu-id="3a540-191">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="3a540-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="3a540-192">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="3a540-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="3a540-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-193">Boolean</span></span>|<span data-ttu-id="3a540-194">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="3a540-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="3a540-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="3a540-195">compliantAppsList</span></span>|<span data-ttu-id="3a540-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a540-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3a540-197">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="3a540-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="3a540-198">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="3a540-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="3a540-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="3a540-199">compliantAppListType</span></span>|[<span data-ttu-id="3a540-200">appListType</span><span class="sxs-lookup"><span data-stu-id="3a540-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="3a540-201">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="3a540-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="3a540-202">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="3a540-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="3a540-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="3a540-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="3a540-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-204">Boolean</span></span>|<span data-ttu-id="3a540-205">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="3a540-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="3a540-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-206">locationServicesBlocked</span></span>|<span data-ttu-id="3a540-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-207">Boolean</span></span>|<span data-ttu-id="3a540-208">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="3a540-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="3a540-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="3a540-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="3a540-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-210">Boolean</span></span>|<span data-ttu-id="3a540-211">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="3a540-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="3a540-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="3a540-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-213">Boolean</span></span>|<span data-ttu-id="3a540-214">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="3a540-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="3a540-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="3a540-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="3a540-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-216">Boolean</span></span>|<span data-ttu-id="3a540-217">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="3a540-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="3a540-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="3a540-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="3a540-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-219">Boolean</span></span>|<span data-ttu-id="3a540-220">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="3a540-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="3a540-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="3a540-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="3a540-222">布尔</span><span class="sxs-lookup"><span data-stu-id="3a540-222">Boolean</span></span>|<span data-ttu-id="3a540-223">指示阻止不断变化的日期和时间在 KNOX 模式下。</span><span class="sxs-lookup"><span data-stu-id="3a540-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="3a540-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="3a540-224">kioskModeApps</span></span>|<span data-ttu-id="3a540-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a540-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3a540-226">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3a540-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="3a540-227">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3a540-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3a540-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-228">nfcBlocked</span></span>|<span data-ttu-id="3a540-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-229">Boolean</span></span>|<span data-ttu-id="3a540-230">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="3a540-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="3a540-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="3a540-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="3a540-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-232">Boolean</span></span>|<span data-ttu-id="3a540-233">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="3a540-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="3a540-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="3a540-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="3a540-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-235">Boolean</span></span>|<span data-ttu-id="3a540-236">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="3a540-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="3a540-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3a540-237">passwordExpirationDays</span></span>|<span data-ttu-id="3a540-238">Int32</span><span class="sxs-lookup"><span data-stu-id="3a540-238">Int32</span></span>|<span data-ttu-id="3a540-239">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="3a540-239">Number of days before the password expires.</span></span> <span data-ttu-id="3a540-240">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="3a540-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3a540-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3a540-241">passwordMinimumLength</span></span>|<span data-ttu-id="3a540-242">Int32</span><span class="sxs-lookup"><span data-stu-id="3a540-242">Int32</span></span>|<span data-ttu-id="3a540-243">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="3a540-243">Minimum length of passwords.</span></span> <span data-ttu-id="3a540-244">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="3a540-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3a540-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3a540-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3a540-246">Int32</span><span class="sxs-lookup"><span data-stu-id="3a540-246">Int32</span></span>|<span data-ttu-id="3a540-247">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="3a540-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3a540-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3a540-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3a540-249">Int32</span><span class="sxs-lookup"><span data-stu-id="3a540-249">Int32</span></span>|<span data-ttu-id="3a540-250">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="3a540-250">Number of previous passwords to block.</span></span> <span data-ttu-id="3a540-251">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="3a540-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3a540-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3a540-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3a540-253">Int32</span><span class="sxs-lookup"><span data-stu-id="3a540-253">Int32</span></span>|<span data-ttu-id="3a540-254">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="3a540-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="3a540-255">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="3a540-255">Valid values 4 to 11</span></span>|
|<span data-ttu-id="3a540-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3a540-256">passwordRequiredType</span></span>|[<span data-ttu-id="3a540-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3a540-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="3a540-258">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3a540-258">Type of password that is required.</span></span> <span data-ttu-id="3a540-259">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="3a540-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="3a540-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3a540-260">passwordRequired</span></span>|<span data-ttu-id="3a540-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-261">Boolean</span></span>|<span data-ttu-id="3a540-262">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="3a540-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="3a540-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-263">powerOffBlocked</span></span>|<span data-ttu-id="3a540-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-264">Boolean</span></span>|<span data-ttu-id="3a540-265">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="3a540-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="3a540-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-266">factoryResetBlocked</span></span>|<span data-ttu-id="3a540-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-267">Boolean</span></span>|<span data-ttu-id="3a540-268">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="3a540-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="3a540-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-269">screenCaptureBlocked</span></span>|<span data-ttu-id="3a540-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-270">Boolean</span></span>|<span data-ttu-id="3a540-271">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="3a540-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="3a540-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="3a540-272">deviceSharingAllowed</span></span>|<span data-ttu-id="3a540-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-273">Boolean</span></span>|<span data-ttu-id="3a540-274">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="3a540-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="3a540-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="3a540-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="3a540-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-276">Boolean</span></span>|<span data-ttu-id="3a540-277">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="3a540-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="3a540-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="3a540-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="3a540-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-279">Boolean</span></span>|<span data-ttu-id="3a540-280">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="3a540-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="3a540-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="3a540-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="3a540-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-282">Boolean</span></span>|<span data-ttu-id="3a540-283">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="3a540-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="3a540-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="3a540-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="3a540-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-285">Boolean</span></span>|<span data-ttu-id="3a540-286">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="3a540-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="3a540-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="3a540-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-288">Boolean</span></span>|<span data-ttu-id="3a540-289">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="3a540-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="3a540-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-290">voiceDialingBlocked</span></span>|<span data-ttu-id="3a540-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-291">Boolean</span></span>|<span data-ttu-id="3a540-292">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="3a540-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="3a540-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="3a540-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="3a540-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-294">Boolean</span></span>|<span data-ttu-id="3a540-295">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="3a540-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="3a540-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="3a540-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="3a540-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-297">Boolean</span></span>|<span data-ttu-id="3a540-298">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="3a540-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="3a540-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="3a540-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="3a540-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-300">Boolean</span></span>|<span data-ttu-id="3a540-301">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="3a540-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="3a540-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-302">webBrowserBlocked</span></span>|<span data-ttu-id="3a540-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-303">Boolean</span></span>|<span data-ttu-id="3a540-304">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="3a540-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="3a540-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="3a540-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="3a540-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="3a540-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="3a540-307">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="3a540-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="3a540-308">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="3a540-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="3a540-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="3a540-309">wiFiBlocked</span></span>|<span data-ttu-id="3a540-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-310">Boolean</span></span>|<span data-ttu-id="3a540-311">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="3a540-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="3a540-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="3a540-312">appsInstallAllowList</span></span>|<span data-ttu-id="3a540-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a540-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3a540-314">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3a540-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="3a540-315">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3a540-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3a540-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="3a540-316">appsLaunchBlockList</span></span>|<span data-ttu-id="3a540-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a540-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3a540-318">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3a540-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="3a540-319">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3a540-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3a540-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="3a540-320">appsHideList</span></span>|<span data-ttu-id="3a540-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a540-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3a540-322">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="3a540-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="3a540-323">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3a540-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3a540-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3a540-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="3a540-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a540-325">Boolean</span></span>|<span data-ttu-id="3a540-326">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="3a540-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="3a540-327">响应</span><span class="sxs-lookup"><span data-stu-id="3a540-327">Response</span></span>
<span data-ttu-id="3a540-328">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a540-328">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a540-329">示例</span><span class="sxs-lookup"><span data-stu-id="3a540-329">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a540-330">请求</span><span class="sxs-lookup"><span data-stu-id="3a540-330">Request</span></span>
<span data-ttu-id="3a540-331">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a540-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3225

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="3a540-332">响应</span><span class="sxs-lookup"><span data-stu-id="3a540-332">Response</span></span>
<span data-ttu-id="3a540-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a540-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





