---
title: 创建 androidGeneralDeviceConfiguration
description: 创建新的 androidGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 942fb299ca42a5d60947bb6b2261950b4a21dd2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474654"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="7c307-103">创建 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c307-103">Create androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="7c307-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c307-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c307-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c307-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c307-106">创建新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c307-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c307-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7c307-107">Prerequisites</span></span>
<span data-ttu-id="7c307-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c307-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c307-110">Permission type</span></span>|<span data-ttu-id="7c307-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7c307-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c307-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c307-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c307-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c307-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c307-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c307-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c307-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c307-115">Not supported.</span></span>|
|<span data-ttu-id="7c307-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c307-116">Application</span></span>|<span data-ttu-id="7c307-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c307-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c307-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c307-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c307-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c307-119">Request headers</span></span>
|<span data-ttu-id="7c307-120">标头</span><span class="sxs-lookup"><span data-stu-id="7c307-120">Header</span></span>|<span data-ttu-id="7c307-121">值</span><span class="sxs-lookup"><span data-stu-id="7c307-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c307-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c307-122">Authorization</span></span>|<span data-ttu-id="7c307-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7c307-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c307-124">接受</span><span class="sxs-lookup"><span data-stu-id="7c307-124">Accept</span></span>|<span data-ttu-id="7c307-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c307-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c307-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c307-126">Request body</span></span>
<span data-ttu-id="7c307-127">在请求正文中，提供 androidGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c307-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="7c307-128">下表显示创建 androidGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7c307-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="7c307-129">属性</span><span class="sxs-lookup"><span data-stu-id="7c307-129">Property</span></span>|<span data-ttu-id="7c307-130">类型</span><span class="sxs-lookup"><span data-stu-id="7c307-130">Type</span></span>|<span data-ttu-id="7c307-131">说明</span><span class="sxs-lookup"><span data-stu-id="7c307-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c307-132">id</span><span class="sxs-lookup"><span data-stu-id="7c307-132">id</span></span>|<span data-ttu-id="7c307-133">字符串</span><span class="sxs-lookup"><span data-stu-id="7c307-133">String</span></span>|<span data-ttu-id="7c307-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7c307-134">Key of the entity.</span></span> <span data-ttu-id="7c307-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c307-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c307-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c307-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7c307-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c307-137">DateTimeOffset</span></span>|<span data-ttu-id="7c307-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7c307-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7c307-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c307-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c307-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c307-140">createdDateTime</span></span>|<span data-ttu-id="7c307-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c307-141">DateTimeOffset</span></span>|<span data-ttu-id="7c307-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7c307-142">DateTime the object was created.</span></span> <span data-ttu-id="7c307-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c307-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c307-144">description</span><span class="sxs-lookup"><span data-stu-id="7c307-144">description</span></span>|<span data-ttu-id="7c307-145">String</span><span class="sxs-lookup"><span data-stu-id="7c307-145">String</span></span>|<span data-ttu-id="7c307-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7c307-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7c307-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c307-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c307-148">displayName</span><span class="sxs-lookup"><span data-stu-id="7c307-148">displayName</span></span>|<span data-ttu-id="7c307-149">String</span><span class="sxs-lookup"><span data-stu-id="7c307-149">String</span></span>|<span data-ttu-id="7c307-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7c307-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7c307-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c307-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c307-152">version</span><span class="sxs-lookup"><span data-stu-id="7c307-152">version</span></span>|<span data-ttu-id="7c307-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7c307-153">Int32</span></span>|<span data-ttu-id="7c307-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7c307-154">Version of the device configuration.</span></span> <span data-ttu-id="7c307-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c307-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c307-156">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="7c307-156">appsBlockClipboardSharing</span></span>|<span data-ttu-id="7c307-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-157">Boolean</span></span>|<span data-ttu-id="7c307-158">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="7c307-158">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="7c307-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="7c307-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="7c307-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-160">Boolean</span></span>|<span data-ttu-id="7c307-161">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="7c307-161">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="7c307-162">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="7c307-162">appsBlockYouTube</span></span>|<span data-ttu-id="7c307-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-163">Boolean</span></span>|<span data-ttu-id="7c307-164">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="7c307-164">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="7c307-165">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-165">bluetoothBlocked</span></span>|<span data-ttu-id="7c307-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-166">Boolean</span></span>|<span data-ttu-id="7c307-167">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="7c307-167">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="7c307-168">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-168">cameraBlocked</span></span>|<span data-ttu-id="7c307-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-169">Boolean</span></span>|<span data-ttu-id="7c307-170">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="7c307-170">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="7c307-171">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="7c307-171">cellularBlockDataRoaming</span></span>|<span data-ttu-id="7c307-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-172">Boolean</span></span>|<span data-ttu-id="7c307-173">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="7c307-173">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="7c307-174">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="7c307-174">cellularBlockMessaging</span></span>|<span data-ttu-id="7c307-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-175">Boolean</span></span>|<span data-ttu-id="7c307-176">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="7c307-176">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="7c307-177">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="7c307-177">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="7c307-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-178">Boolean</span></span>|<span data-ttu-id="7c307-179">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="7c307-179">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="7c307-180">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="7c307-180">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="7c307-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-181">Boolean</span></span>|<span data-ttu-id="7c307-182">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="7c307-182">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="7c307-183">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="7c307-183">compliantAppsList</span></span>|<span data-ttu-id="7c307-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c307-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7c307-185">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="7c307-185">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="7c307-186">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="7c307-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7c307-187">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="7c307-187">compliantAppListType</span></span>|[<span data-ttu-id="7c307-188">appListType</span><span class="sxs-lookup"><span data-stu-id="7c307-188">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="7c307-189">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="7c307-189">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="7c307-190">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="7c307-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7c307-191">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="7c307-191">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="7c307-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-192">Boolean</span></span>|<span data-ttu-id="7c307-193">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="7c307-193">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="7c307-194">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-194">locationServicesBlocked</span></span>|<span data-ttu-id="7c307-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-195">Boolean</span></span>|<span data-ttu-id="7c307-196">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="7c307-196">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="7c307-197">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="7c307-197">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="7c307-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-198">Boolean</span></span>|<span data-ttu-id="7c307-199">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="7c307-199">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="7c307-200">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-200">googlePlayStoreBlocked</span></span>|<span data-ttu-id="7c307-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-201">Boolean</span></span>|<span data-ttu-id="7c307-202">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="7c307-202">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="7c307-203">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="7c307-203">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="7c307-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-204">Boolean</span></span>|<span data-ttu-id="7c307-205">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="7c307-205">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="7c307-206">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="7c307-206">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="7c307-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-207">Boolean</span></span>|<span data-ttu-id="7c307-208">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="7c307-208">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="7c307-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="7c307-209">kioskModeApps</span></span>|<span data-ttu-id="7c307-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c307-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7c307-211">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="7c307-211">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="7c307-212">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7c307-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7c307-213">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-213">nfcBlocked</span></span>|<span data-ttu-id="7c307-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-214">Boolean</span></span>|<span data-ttu-id="7c307-215">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="7c307-215">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="7c307-216">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="7c307-216">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="7c307-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-217">Boolean</span></span>|<span data-ttu-id="7c307-218">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="7c307-218">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="7c307-219">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="7c307-219">passwordBlockTrustAgents</span></span>|<span data-ttu-id="7c307-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-220">Boolean</span></span>|<span data-ttu-id="7c307-221">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="7c307-221">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="7c307-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7c307-222">passwordExpirationDays</span></span>|<span data-ttu-id="7c307-223">Int32</span><span class="sxs-lookup"><span data-stu-id="7c307-223">Int32</span></span>|<span data-ttu-id="7c307-224">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="7c307-224">Number of days before the password expires.</span></span> <span data-ttu-id="7c307-225">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="7c307-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7c307-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7c307-226">passwordMinimumLength</span></span>|<span data-ttu-id="7c307-227">Int32</span><span class="sxs-lookup"><span data-stu-id="7c307-227">Int32</span></span>|<span data-ttu-id="7c307-228">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="7c307-228">Minimum length of passwords.</span></span> <span data-ttu-id="7c307-229">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="7c307-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7c307-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7c307-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7c307-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7c307-231">Int32</span></span>|<span data-ttu-id="7c307-232">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="7c307-232">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7c307-233">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7c307-233">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7c307-234">Int32</span><span class="sxs-lookup"><span data-stu-id="7c307-234">Int32</span></span>|<span data-ttu-id="7c307-235">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="7c307-235">Number of previous passwords to block.</span></span> <span data-ttu-id="7c307-236">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="7c307-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7c307-237">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7c307-237">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7c307-238">Int32</span><span class="sxs-lookup"><span data-stu-id="7c307-238">Int32</span></span>|<span data-ttu-id="7c307-239">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="7c307-239">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="7c307-240">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="7c307-240">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7c307-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7c307-241">passwordRequiredType</span></span>|[<span data-ttu-id="7c307-242">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7c307-242">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="7c307-243">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="7c307-243">Type of password that is required.</span></span> <span data-ttu-id="7c307-244">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="7c307-244">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="7c307-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7c307-245">passwordRequired</span></span>|<span data-ttu-id="7c307-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-246">Boolean</span></span>|<span data-ttu-id="7c307-247">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="7c307-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="7c307-248">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-248">powerOffBlocked</span></span>|<span data-ttu-id="7c307-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-249">Boolean</span></span>|<span data-ttu-id="7c307-250">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="7c307-250">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="7c307-251">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-251">factoryResetBlocked</span></span>|<span data-ttu-id="7c307-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-252">Boolean</span></span>|<span data-ttu-id="7c307-253">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="7c307-253">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="7c307-254">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-254">screenCaptureBlocked</span></span>|<span data-ttu-id="7c307-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-255">Boolean</span></span>|<span data-ttu-id="7c307-256">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="7c307-256">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="7c307-257">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="7c307-257">deviceSharingAllowed</span></span>|<span data-ttu-id="7c307-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-258">Boolean</span></span>|<span data-ttu-id="7c307-259">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="7c307-259">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="7c307-260">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="7c307-260">storageBlockGoogleBackup</span></span>|<span data-ttu-id="7c307-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-261">Boolean</span></span>|<span data-ttu-id="7c307-262">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="7c307-262">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="7c307-263">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="7c307-263">storageBlockRemovableStorage</span></span>|<span data-ttu-id="7c307-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-264">Boolean</span></span>|<span data-ttu-id="7c307-265">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="7c307-265">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="7c307-266">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="7c307-266">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="7c307-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-267">Boolean</span></span>|<span data-ttu-id="7c307-268">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="7c307-268">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="7c307-269">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="7c307-269">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="7c307-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-270">Boolean</span></span>|<span data-ttu-id="7c307-271">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="7c307-271">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="7c307-272">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-272">voiceAssistantBlocked</span></span>|<span data-ttu-id="7c307-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-273">Boolean</span></span>|<span data-ttu-id="7c307-274">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="7c307-274">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="7c307-275">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-275">voiceDialingBlocked</span></span>|<span data-ttu-id="7c307-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-276">Boolean</span></span>|<span data-ttu-id="7c307-277">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="7c307-277">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="7c307-278">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="7c307-278">webBrowserBlockPopups</span></span>|<span data-ttu-id="7c307-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-279">Boolean</span></span>|<span data-ttu-id="7c307-280">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="7c307-280">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="7c307-281">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7c307-281">webBrowserBlockAutofill</span></span>|<span data-ttu-id="7c307-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-282">Boolean</span></span>|<span data-ttu-id="7c307-283">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="7c307-283">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="7c307-284">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="7c307-284">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="7c307-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-285">Boolean</span></span>|<span data-ttu-id="7c307-286">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="7c307-286">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="7c307-287">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-287">webBrowserBlocked</span></span>|<span data-ttu-id="7c307-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-288">Boolean</span></span>|<span data-ttu-id="7c307-289">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="7c307-289">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="7c307-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7c307-290">webBrowserCookieSettings</span></span>|[<span data-ttu-id="7c307-291">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7c307-291">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="7c307-292">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="7c307-292">Cookie settings within the web browser.</span></span> <span data-ttu-id="7c307-293">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="7c307-293">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="7c307-294">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="7c307-294">wiFiBlocked</span></span>|<span data-ttu-id="7c307-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-295">Boolean</span></span>|<span data-ttu-id="7c307-296">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="7c307-296">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="7c307-297">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="7c307-297">appsInstallAllowList</span></span>|<span data-ttu-id="7c307-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c307-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7c307-299">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="7c307-299">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="7c307-300">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7c307-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7c307-301">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="7c307-301">appsLaunchBlockList</span></span>|<span data-ttu-id="7c307-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c307-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7c307-303">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="7c307-303">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="7c307-304">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7c307-304">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7c307-305">appsHideList</span><span class="sxs-lookup"><span data-stu-id="7c307-305">appsHideList</span></span>|<span data-ttu-id="7c307-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c307-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7c307-307">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="7c307-307">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="7c307-308">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7c307-308">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7c307-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7c307-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="7c307-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c307-310">Boolean</span></span>|<span data-ttu-id="7c307-311">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="7c307-311">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="7c307-312">响应</span><span class="sxs-lookup"><span data-stu-id="7c307-312">Response</span></span>
<span data-ttu-id="7c307-313">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c307-313">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c307-314">示例</span><span class="sxs-lookup"><span data-stu-id="7c307-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c307-315">请求</span><span class="sxs-lookup"><span data-stu-id="7c307-315">Request</span></span>
<span data-ttu-id="7c307-316">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c307-316">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="7c307-317">响应</span><span class="sxs-lookup"><span data-stu-id="7c307-317">Response</span></span>
<span data-ttu-id="7c307-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c307-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






