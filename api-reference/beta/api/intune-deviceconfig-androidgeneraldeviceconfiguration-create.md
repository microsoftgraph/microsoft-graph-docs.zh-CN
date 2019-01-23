---
title: 创建 androidGeneralDeviceConfiguration
description: 创建新的 androidGeneralDeviceConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 22e5ab9278bd5771f50e4c8eb4dc476e71fb4a21
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413582"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="72fa5-103">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="72fa5-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="72fa5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="72fa5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72fa5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="72fa5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72fa5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72fa5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72fa5-107">创建新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72fa5-107">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72fa5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="72fa5-108">Prerequisites</span></span>
<span data-ttu-id="72fa5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="72fa5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="72fa5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="72fa5-111">Permission type</span></span>|<span data-ttu-id="72fa5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="72fa5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72fa5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72fa5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72fa5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72fa5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72fa5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72fa5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72fa5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="72fa5-116">Not supported.</span></span>|
|<span data-ttu-id="72fa5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="72fa5-117">Application</span></span>|<span data-ttu-id="72fa5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="72fa5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72fa5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72fa5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="72fa5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="72fa5-120">Request headers</span></span>
|<span data-ttu-id="72fa5-121">标头</span><span class="sxs-lookup"><span data-stu-id="72fa5-121">Header</span></span>|<span data-ttu-id="72fa5-122">值</span><span class="sxs-lookup"><span data-stu-id="72fa5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72fa5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72fa5-123">Authorization</span></span>|<span data-ttu-id="72fa5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="72fa5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72fa5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72fa5-125">Accept</span></span>|<span data-ttu-id="72fa5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72fa5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72fa5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="72fa5-127">Request body</span></span>
<span data-ttu-id="72fa5-128">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72fa5-128">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="72fa5-129">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="72fa5-129">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="72fa5-130">属性</span><span class="sxs-lookup"><span data-stu-id="72fa5-130">Property</span></span>|<span data-ttu-id="72fa5-131">类型</span><span class="sxs-lookup"><span data-stu-id="72fa5-131">Type</span></span>|<span data-ttu-id="72fa5-132">说明</span><span class="sxs-lookup"><span data-stu-id="72fa5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72fa5-133">id</span><span class="sxs-lookup"><span data-stu-id="72fa5-133">id</span></span>|<span data-ttu-id="72fa5-134">String</span><span class="sxs-lookup"><span data-stu-id="72fa5-134">String</span></span>|<span data-ttu-id="72fa5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="72fa5-135">Key of the entity.</span></span> <span data-ttu-id="72fa5-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72fa5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="72fa5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72fa5-138">DateTimeOffset</span></span>|<span data-ttu-id="72fa5-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72fa5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="72fa5-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="72fa5-141">roleScopeTagIds</span></span>|<span data-ttu-id="72fa5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="72fa5-142">String collection</span></span>|<span data-ttu-id="72fa5-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="72fa5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="72fa5-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="72fa5-145">supportsScopeTags</span></span>|<span data-ttu-id="72fa5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-146">Boolean</span></span>|<span data-ttu-id="72fa5-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="72fa5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="72fa5-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="72fa5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="72fa5-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="72fa5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="72fa5-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="72fa5-150">This property is read-only.</span></span> <span data-ttu-id="72fa5-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72fa5-152">createdDateTime</span></span>|<span data-ttu-id="72fa5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72fa5-153">DateTimeOffset</span></span>|<span data-ttu-id="72fa5-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72fa5-154">DateTime the object was created.</span></span> <span data-ttu-id="72fa5-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-156">description</span><span class="sxs-lookup"><span data-stu-id="72fa5-156">description</span></span>|<span data-ttu-id="72fa5-157">String</span><span class="sxs-lookup"><span data-stu-id="72fa5-157">String</span></span>|<span data-ttu-id="72fa5-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="72fa5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72fa5-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="72fa5-160">displayName</span></span>|<span data-ttu-id="72fa5-161">String</span><span class="sxs-lookup"><span data-stu-id="72fa5-161">String</span></span>|<span data-ttu-id="72fa5-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="72fa5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72fa5-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-164">version</span><span class="sxs-lookup"><span data-stu-id="72fa5-164">version</span></span>|<span data-ttu-id="72fa5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="72fa5-165">Int32</span></span>|<span data-ttu-id="72fa5-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="72fa5-166">Version of the device configuration.</span></span> <span data-ttu-id="72fa5-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72fa5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72fa5-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="72fa5-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="72fa5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-169">Boolean</span></span>|<span data-ttu-id="72fa5-170">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="72fa5-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="72fa5-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="72fa5-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="72fa5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-172">Boolean</span></span>|<span data-ttu-id="72fa5-173">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="72fa5-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="72fa5-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="72fa5-174">appsBlockYouTube</span></span>|<span data-ttu-id="72fa5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-175">Boolean</span></span>|<span data-ttu-id="72fa5-176">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="72fa5-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="72fa5-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-177">bluetoothBlocked</span></span>|<span data-ttu-id="72fa5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-178">Boolean</span></span>|<span data-ttu-id="72fa5-179">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="72fa5-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="72fa5-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-180">cameraBlocked</span></span>|<span data-ttu-id="72fa5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-181">Boolean</span></span>|<span data-ttu-id="72fa5-182">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="72fa5-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="72fa5-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="72fa5-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="72fa5-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-184">Boolean</span></span>|<span data-ttu-id="72fa5-185">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="72fa5-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="72fa5-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="72fa5-186">cellularBlockMessaging</span></span>|<span data-ttu-id="72fa5-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-187">Boolean</span></span>|<span data-ttu-id="72fa5-188">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="72fa5-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="72fa5-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="72fa5-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="72fa5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-190">Boolean</span></span>|<span data-ttu-id="72fa5-191">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="72fa5-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="72fa5-192">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="72fa5-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="72fa5-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-193">Boolean</span></span>|<span data-ttu-id="72fa5-194">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="72fa5-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="72fa5-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="72fa5-195">compliantAppsList</span></span>|<span data-ttu-id="72fa5-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fa5-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72fa5-197">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="72fa5-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="72fa5-198">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="72fa5-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="72fa5-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="72fa5-199">compliantAppListType</span></span>|[<span data-ttu-id="72fa5-200">appListType</span><span class="sxs-lookup"><span data-stu-id="72fa5-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="72fa5-201">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="72fa5-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="72fa5-202">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="72fa5-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="72fa5-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="72fa5-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="72fa5-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-204">Boolean</span></span>|<span data-ttu-id="72fa5-205">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="72fa5-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="72fa5-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-206">locationServicesBlocked</span></span>|<span data-ttu-id="72fa5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-207">Boolean</span></span>|<span data-ttu-id="72fa5-208">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="72fa5-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="72fa5-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="72fa5-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="72fa5-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-210">Boolean</span></span>|<span data-ttu-id="72fa5-211">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="72fa5-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="72fa5-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="72fa5-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-213">Boolean</span></span>|<span data-ttu-id="72fa5-214">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="72fa5-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="72fa5-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="72fa5-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="72fa5-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-216">Boolean</span></span>|<span data-ttu-id="72fa5-217">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="72fa5-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="72fa5-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="72fa5-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="72fa5-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-219">Boolean</span></span>|<span data-ttu-id="72fa5-220">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="72fa5-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="72fa5-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="72fa5-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="72fa5-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-222">Boolean</span></span>|<span data-ttu-id="72fa5-223">指示阻止不断变化的日期和时间在 KNOX 模式下。</span><span class="sxs-lookup"><span data-stu-id="72fa5-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="72fa5-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="72fa5-224">kioskModeApps</span></span>|<span data-ttu-id="72fa5-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fa5-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72fa5-226">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="72fa5-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="72fa5-227">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="72fa5-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="72fa5-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-228">nfcBlocked</span></span>|<span data-ttu-id="72fa5-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-229">Boolean</span></span>|<span data-ttu-id="72fa5-230">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="72fa5-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="72fa5-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="72fa5-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="72fa5-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-232">Boolean</span></span>|<span data-ttu-id="72fa5-233">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="72fa5-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="72fa5-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="72fa5-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="72fa5-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-235">Boolean</span></span>|<span data-ttu-id="72fa5-236">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="72fa5-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="72fa5-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="72fa5-237">passwordExpirationDays</span></span>|<span data-ttu-id="72fa5-238">Int32</span><span class="sxs-lookup"><span data-stu-id="72fa5-238">Int32</span></span>|<span data-ttu-id="72fa5-239">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="72fa5-239">Number of days before the password expires.</span></span> <span data-ttu-id="72fa5-240">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="72fa5-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="72fa5-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="72fa5-241">passwordMinimumLength</span></span>|<span data-ttu-id="72fa5-242">Int32</span><span class="sxs-lookup"><span data-stu-id="72fa5-242">Int32</span></span>|<span data-ttu-id="72fa5-243">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="72fa5-243">Minimum length of passwords.</span></span> <span data-ttu-id="72fa5-244">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="72fa5-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="72fa5-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="72fa5-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="72fa5-246">Int32</span><span class="sxs-lookup"><span data-stu-id="72fa5-246">Int32</span></span>|<span data-ttu-id="72fa5-247">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="72fa5-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="72fa5-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="72fa5-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="72fa5-249">Int32</span><span class="sxs-lookup"><span data-stu-id="72fa5-249">Int32</span></span>|<span data-ttu-id="72fa5-250">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="72fa5-250">Number of previous passwords to block.</span></span> <span data-ttu-id="72fa5-251">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="72fa5-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="72fa5-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="72fa5-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="72fa5-253">Int32</span><span class="sxs-lookup"><span data-stu-id="72fa5-253">Int32</span></span>|<span data-ttu-id="72fa5-254">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="72fa5-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="72fa5-255">有效的值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="72fa5-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="72fa5-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="72fa5-256">passwordRequiredType</span></span>|[<span data-ttu-id="72fa5-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="72fa5-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="72fa5-258">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="72fa5-258">Type of password that is required.</span></span> <span data-ttu-id="72fa5-259">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="72fa5-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="72fa5-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="72fa5-260">passwordRequired</span></span>|<span data-ttu-id="72fa5-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-261">Boolean</span></span>|<span data-ttu-id="72fa5-262">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="72fa5-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="72fa5-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-263">powerOffBlocked</span></span>|<span data-ttu-id="72fa5-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-264">Boolean</span></span>|<span data-ttu-id="72fa5-265">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="72fa5-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="72fa5-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-266">factoryResetBlocked</span></span>|<span data-ttu-id="72fa5-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-267">Boolean</span></span>|<span data-ttu-id="72fa5-268">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="72fa5-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="72fa5-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-269">screenCaptureBlocked</span></span>|<span data-ttu-id="72fa5-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-270">Boolean</span></span>|<span data-ttu-id="72fa5-271">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="72fa5-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="72fa5-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="72fa5-272">deviceSharingAllowed</span></span>|<span data-ttu-id="72fa5-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-273">Boolean</span></span>|<span data-ttu-id="72fa5-274">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="72fa5-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="72fa5-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="72fa5-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="72fa5-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-276">Boolean</span></span>|<span data-ttu-id="72fa5-277">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="72fa5-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="72fa5-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="72fa5-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="72fa5-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-279">Boolean</span></span>|<span data-ttu-id="72fa5-280">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="72fa5-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="72fa5-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="72fa5-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="72fa5-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-282">Boolean</span></span>|<span data-ttu-id="72fa5-283">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="72fa5-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="72fa5-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="72fa5-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="72fa5-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-285">Boolean</span></span>|<span data-ttu-id="72fa5-286">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="72fa5-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="72fa5-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="72fa5-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-288">Boolean</span></span>|<span data-ttu-id="72fa5-289">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="72fa5-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="72fa5-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-290">voiceDialingBlocked</span></span>|<span data-ttu-id="72fa5-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-291">Boolean</span></span>|<span data-ttu-id="72fa5-292">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="72fa5-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="72fa5-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="72fa5-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="72fa5-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-294">Boolean</span></span>|<span data-ttu-id="72fa5-295">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="72fa5-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="72fa5-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="72fa5-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="72fa5-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-297">Boolean</span></span>|<span data-ttu-id="72fa5-298">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="72fa5-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="72fa5-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="72fa5-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="72fa5-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-300">Boolean</span></span>|<span data-ttu-id="72fa5-301">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="72fa5-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="72fa5-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-302">webBrowserBlocked</span></span>|<span data-ttu-id="72fa5-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-303">Boolean</span></span>|<span data-ttu-id="72fa5-304">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="72fa5-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="72fa5-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="72fa5-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="72fa5-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="72fa5-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="72fa5-307">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="72fa5-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="72fa5-308">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="72fa5-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="72fa5-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="72fa5-309">wiFiBlocked</span></span>|<span data-ttu-id="72fa5-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-310">Boolean</span></span>|<span data-ttu-id="72fa5-311">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="72fa5-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="72fa5-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="72fa5-312">appsInstallAllowList</span></span>|<span data-ttu-id="72fa5-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fa5-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72fa5-314">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="72fa5-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="72fa5-315">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="72fa5-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="72fa5-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="72fa5-316">appsLaunchBlockList</span></span>|<span data-ttu-id="72fa5-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fa5-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72fa5-318">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="72fa5-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="72fa5-319">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="72fa5-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="72fa5-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="72fa5-320">appsHideList</span></span>|<span data-ttu-id="72fa5-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fa5-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72fa5-322">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="72fa5-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="72fa5-323">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="72fa5-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="72fa5-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="72fa5-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="72fa5-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="72fa5-325">Boolean</span></span>|<span data-ttu-id="72fa5-326">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="72fa5-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="72fa5-327">响应</span><span class="sxs-lookup"><span data-stu-id="72fa5-327">Response</span></span>
<span data-ttu-id="72fa5-328">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72fa5-328">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72fa5-329">示例</span><span class="sxs-lookup"><span data-stu-id="72fa5-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="72fa5-330">请求</span><span class="sxs-lookup"><span data-stu-id="72fa5-330">Request</span></span>
<span data-ttu-id="72fa5-331">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72fa5-331">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72fa5-332">响应</span><span class="sxs-lookup"><span data-stu-id="72fa5-332">Response</span></span>
<span data-ttu-id="72fa5-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72fa5-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




