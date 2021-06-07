---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce4bbbe2074bba753d32a7aa8d293282cd320ded
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757218"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="922b5-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="922b5-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="922b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="922b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="922b5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="922b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="922b5-106">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="922b5-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="922b5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="922b5-107">Prerequisites</span></span>
<span data-ttu-id="922b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="922b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="922b5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="922b5-110">Permission type</span></span>|<span data-ttu-id="922b5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="922b5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="922b5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="922b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="922b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="922b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="922b5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="922b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="922b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="922b5-115">Not supported.</span></span>|
|<span data-ttu-id="922b5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="922b5-116">Application</span></span>|<span data-ttu-id="922b5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="922b5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="922b5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="922b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="922b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="922b5-119">Request headers</span></span>
|<span data-ttu-id="922b5-120">标头</span><span class="sxs-lookup"><span data-stu-id="922b5-120">Header</span></span>|<span data-ttu-id="922b5-121">值</span><span class="sxs-lookup"><span data-stu-id="922b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="922b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="922b5-122">Authorization</span></span>|<span data-ttu-id="922b5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="922b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="922b5-124">接受</span><span class="sxs-lookup"><span data-stu-id="922b5-124">Accept</span></span>|<span data-ttu-id="922b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="922b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="922b5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="922b5-126">Request body</span></span>
<span data-ttu-id="922b5-127">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="922b5-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="922b5-128">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="922b5-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="922b5-129">属性</span><span class="sxs-lookup"><span data-stu-id="922b5-129">Property</span></span>|<span data-ttu-id="922b5-130">类型</span><span class="sxs-lookup"><span data-stu-id="922b5-130">Type</span></span>|<span data-ttu-id="922b5-131">说明</span><span class="sxs-lookup"><span data-stu-id="922b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="922b5-132">id</span><span class="sxs-lookup"><span data-stu-id="922b5-132">id</span></span>|<span data-ttu-id="922b5-133">String</span><span class="sxs-lookup"><span data-stu-id="922b5-133">String</span></span>|<span data-ttu-id="922b5-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="922b5-134">Key of the entity.</span></span> <span data-ttu-id="922b5-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="922b5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="922b5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="922b5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="922b5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="922b5-137">DateTimeOffset</span></span>|<span data-ttu-id="922b5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="922b5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="922b5-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="922b5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="922b5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="922b5-140">createdDateTime</span></span>|<span data-ttu-id="922b5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="922b5-141">DateTimeOffset</span></span>|<span data-ttu-id="922b5-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="922b5-142">DateTime the object was created.</span></span> <span data-ttu-id="922b5-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="922b5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="922b5-144">说明</span><span class="sxs-lookup"><span data-stu-id="922b5-144">description</span></span>|<span data-ttu-id="922b5-145">String</span><span class="sxs-lookup"><span data-stu-id="922b5-145">String</span></span>|<span data-ttu-id="922b5-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="922b5-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="922b5-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="922b5-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="922b5-148">displayName</span><span class="sxs-lookup"><span data-stu-id="922b5-148">displayName</span></span>|<span data-ttu-id="922b5-149">String</span><span class="sxs-lookup"><span data-stu-id="922b5-149">String</span></span>|<span data-ttu-id="922b5-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="922b5-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="922b5-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="922b5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="922b5-152">version</span><span class="sxs-lookup"><span data-stu-id="922b5-152">version</span></span>|<span data-ttu-id="922b5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="922b5-153">Int32</span></span>|<span data-ttu-id="922b5-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="922b5-154">Version of the device configuration.</span></span> <span data-ttu-id="922b5-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="922b5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="922b5-156">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="922b5-156">appsBlockClipboardSharing</span></span>|<span data-ttu-id="922b5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-157">Boolean</span></span>|<span data-ttu-id="922b5-158">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="922b5-158">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="922b5-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="922b5-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="922b5-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-160">Boolean</span></span>|<span data-ttu-id="922b5-161">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="922b5-161">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="922b5-162">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="922b5-162">appsBlockYouTube</span></span>|<span data-ttu-id="922b5-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-163">Boolean</span></span>|<span data-ttu-id="922b5-164">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="922b5-164">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="922b5-165">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-165">bluetoothBlocked</span></span>|<span data-ttu-id="922b5-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-166">Boolean</span></span>|<span data-ttu-id="922b5-167">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="922b5-167">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="922b5-168">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-168">cameraBlocked</span></span>|<span data-ttu-id="922b5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-169">Boolean</span></span>|<span data-ttu-id="922b5-170">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="922b5-170">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="922b5-171">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="922b5-171">cellularBlockDataRoaming</span></span>|<span data-ttu-id="922b5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-172">Boolean</span></span>|<span data-ttu-id="922b5-173">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="922b5-173">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="922b5-174">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="922b5-174">cellularBlockMessaging</span></span>|<span data-ttu-id="922b5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-175">Boolean</span></span>|<span data-ttu-id="922b5-176">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="922b5-176">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="922b5-177">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="922b5-177">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="922b5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-178">Boolean</span></span>|<span data-ttu-id="922b5-179">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="922b5-179">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="922b5-180">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="922b5-180">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="922b5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-181">Boolean</span></span>|<span data-ttu-id="922b5-182">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="922b5-182">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="922b5-183">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="922b5-183">compliantAppsList</span></span>|<span data-ttu-id="922b5-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="922b5-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="922b5-185">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="922b5-185">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="922b5-186">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="922b5-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="922b5-187">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="922b5-187">compliantAppListType</span></span>|[<span data-ttu-id="922b5-188">appListType</span><span class="sxs-lookup"><span data-stu-id="922b5-188">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="922b5-189">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="922b5-189">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="922b5-190">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="922b5-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="922b5-191">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="922b5-191">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="922b5-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-192">Boolean</span></span>|<span data-ttu-id="922b5-193">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="922b5-193">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="922b5-194">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-194">locationServicesBlocked</span></span>|<span data-ttu-id="922b5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-195">Boolean</span></span>|<span data-ttu-id="922b5-196">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="922b5-196">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="922b5-197">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="922b5-197">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="922b5-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-198">Boolean</span></span>|<span data-ttu-id="922b5-199">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="922b5-199">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="922b5-200">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-200">googlePlayStoreBlocked</span></span>|<span data-ttu-id="922b5-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-201">Boolean</span></span>|<span data-ttu-id="922b5-202">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="922b5-202">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="922b5-203">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="922b5-203">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="922b5-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-204">Boolean</span></span>|<span data-ttu-id="922b5-205">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="922b5-205">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="922b5-206">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="922b5-206">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="922b5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-207">Boolean</span></span>|<span data-ttu-id="922b5-208">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="922b5-208">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="922b5-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="922b5-209">kioskModeApps</span></span>|<span data-ttu-id="922b5-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="922b5-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="922b5-211">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="922b5-211">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="922b5-212">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="922b5-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="922b5-213">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-213">nfcBlocked</span></span>|<span data-ttu-id="922b5-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-214">Boolean</span></span>|<span data-ttu-id="922b5-215">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="922b5-215">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="922b5-216">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="922b5-216">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="922b5-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-217">Boolean</span></span>|<span data-ttu-id="922b5-218">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="922b5-218">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="922b5-219">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="922b5-219">passwordBlockTrustAgents</span></span>|<span data-ttu-id="922b5-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-220">Boolean</span></span>|<span data-ttu-id="922b5-221">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="922b5-221">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="922b5-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="922b5-222">passwordExpirationDays</span></span>|<span data-ttu-id="922b5-223">Int32</span><span class="sxs-lookup"><span data-stu-id="922b5-223">Int32</span></span>|<span data-ttu-id="922b5-224">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="922b5-224">Number of days before the password expires.</span></span> <span data-ttu-id="922b5-225">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="922b5-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="922b5-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="922b5-226">passwordMinimumLength</span></span>|<span data-ttu-id="922b5-227">Int32</span><span class="sxs-lookup"><span data-stu-id="922b5-227">Int32</span></span>|<span data-ttu-id="922b5-228">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="922b5-228">Minimum length of passwords.</span></span> <span data-ttu-id="922b5-229">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="922b5-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="922b5-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="922b5-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="922b5-231">Int32</span><span class="sxs-lookup"><span data-stu-id="922b5-231">Int32</span></span>|<span data-ttu-id="922b5-232">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="922b5-232">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="922b5-233">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="922b5-233">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="922b5-234">Int32</span><span class="sxs-lookup"><span data-stu-id="922b5-234">Int32</span></span>|<span data-ttu-id="922b5-235">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="922b5-235">Number of previous passwords to block.</span></span> <span data-ttu-id="922b5-236">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="922b5-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="922b5-237">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="922b5-237">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="922b5-238">Int32</span><span class="sxs-lookup"><span data-stu-id="922b5-238">Int32</span></span>|<span data-ttu-id="922b5-239">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="922b5-239">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="922b5-240">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="922b5-240">Valid values 1 to 16</span></span>|
|<span data-ttu-id="922b5-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="922b5-241">passwordRequiredType</span></span>|[<span data-ttu-id="922b5-242">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="922b5-242">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="922b5-243">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="922b5-243">Type of password that is required.</span></span> <span data-ttu-id="922b5-244">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="922b5-244">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="922b5-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="922b5-245">passwordRequired</span></span>|<span data-ttu-id="922b5-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-246">Boolean</span></span>|<span data-ttu-id="922b5-247">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="922b5-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="922b5-248">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-248">powerOffBlocked</span></span>|<span data-ttu-id="922b5-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-249">Boolean</span></span>|<span data-ttu-id="922b5-250">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="922b5-250">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="922b5-251">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-251">factoryResetBlocked</span></span>|<span data-ttu-id="922b5-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-252">Boolean</span></span>|<span data-ttu-id="922b5-253">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="922b5-253">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="922b5-254">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-254">screenCaptureBlocked</span></span>|<span data-ttu-id="922b5-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-255">Boolean</span></span>|<span data-ttu-id="922b5-256">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="922b5-256">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="922b5-257">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="922b5-257">deviceSharingAllowed</span></span>|<span data-ttu-id="922b5-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-258">Boolean</span></span>|<span data-ttu-id="922b5-259">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="922b5-259">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="922b5-260">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="922b5-260">storageBlockGoogleBackup</span></span>|<span data-ttu-id="922b5-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-261">Boolean</span></span>|<span data-ttu-id="922b5-262">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="922b5-262">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="922b5-263">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="922b5-263">storageBlockRemovableStorage</span></span>|<span data-ttu-id="922b5-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-264">Boolean</span></span>|<span data-ttu-id="922b5-265">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="922b5-265">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="922b5-266">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="922b5-266">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="922b5-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-267">Boolean</span></span>|<span data-ttu-id="922b5-268">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="922b5-268">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="922b5-269">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="922b5-269">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="922b5-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-270">Boolean</span></span>|<span data-ttu-id="922b5-271">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="922b5-271">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="922b5-272">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-272">voiceAssistantBlocked</span></span>|<span data-ttu-id="922b5-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-273">Boolean</span></span>|<span data-ttu-id="922b5-274">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="922b5-274">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="922b5-275">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-275">voiceDialingBlocked</span></span>|<span data-ttu-id="922b5-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-276">Boolean</span></span>|<span data-ttu-id="922b5-277">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="922b5-277">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="922b5-278">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="922b5-278">webBrowserBlockPopups</span></span>|<span data-ttu-id="922b5-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-279">Boolean</span></span>|<span data-ttu-id="922b5-280">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="922b5-280">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="922b5-281">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="922b5-281">webBrowserBlockAutofill</span></span>|<span data-ttu-id="922b5-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-282">Boolean</span></span>|<span data-ttu-id="922b5-283">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="922b5-283">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="922b5-284">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="922b5-284">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="922b5-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-285">Boolean</span></span>|<span data-ttu-id="922b5-286">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="922b5-286">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="922b5-287">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-287">webBrowserBlocked</span></span>|<span data-ttu-id="922b5-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-288">Boolean</span></span>|<span data-ttu-id="922b5-289">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="922b5-289">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="922b5-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="922b5-290">webBrowserCookieSettings</span></span>|[<span data-ttu-id="922b5-291">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="922b5-291">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="922b5-292">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="922b5-292">Cookie settings within the web browser.</span></span> <span data-ttu-id="922b5-293">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="922b5-293">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="922b5-294">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="922b5-294">wiFiBlocked</span></span>|<span data-ttu-id="922b5-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-295">Boolean</span></span>|<span data-ttu-id="922b5-296">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="922b5-296">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="922b5-297">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="922b5-297">appsInstallAllowList</span></span>|<span data-ttu-id="922b5-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="922b5-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="922b5-299">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="922b5-299">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="922b5-300">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="922b5-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="922b5-301">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="922b5-301">appsLaunchBlockList</span></span>|<span data-ttu-id="922b5-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="922b5-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="922b5-303">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="922b5-303">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="922b5-304">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="922b5-304">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="922b5-305">appsHideList</span><span class="sxs-lookup"><span data-stu-id="922b5-305">appsHideList</span></span>|<span data-ttu-id="922b5-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="922b5-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="922b5-307">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="922b5-307">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="922b5-308">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="922b5-308">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="922b5-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="922b5-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="922b5-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="922b5-310">Boolean</span></span>|<span data-ttu-id="922b5-311">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="922b5-311">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="922b5-312">响应</span><span class="sxs-lookup"><span data-stu-id="922b5-312">Response</span></span>
<span data-ttu-id="922b5-313">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="922b5-313">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="922b5-314">示例</span><span class="sxs-lookup"><span data-stu-id="922b5-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="922b5-315">请求</span><span class="sxs-lookup"><span data-stu-id="922b5-315">Request</span></span>
<span data-ttu-id="922b5-316">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="922b5-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3033

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="922b5-317">响应</span><span class="sxs-lookup"><span data-stu-id="922b5-317">Response</span></span>
<span data-ttu-id="922b5-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="922b5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




