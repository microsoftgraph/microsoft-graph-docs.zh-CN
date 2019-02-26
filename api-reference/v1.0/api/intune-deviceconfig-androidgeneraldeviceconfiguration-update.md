---
title: 更新 androidGeneralDeviceConfiguration
description: 更新 androidGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a134a6b501859b1ec6e10ec54c00b590dc5808fd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256159"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="37909-103">更新 androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="37909-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="37909-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37909-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37909-105">更新 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="37909-105">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37909-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="37909-106">Prerequisites</span></span>
<span data-ttu-id="37909-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="37909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37909-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="37909-109">Permission type</span></span>|<span data-ttu-id="37909-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37909-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37909-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37909-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37909-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37909-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37909-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37909-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37909-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="37909-114">Not supported.</span></span>|
|<span data-ttu-id="37909-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="37909-115">Application</span></span>|<span data-ttu-id="37909-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37909-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37909-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37909-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="37909-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="37909-118">Request headers</span></span>
|<span data-ttu-id="37909-119">标头</span><span class="sxs-lookup"><span data-stu-id="37909-119">Header</span></span>|<span data-ttu-id="37909-120">值</span><span class="sxs-lookup"><span data-stu-id="37909-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37909-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37909-121">Authorization</span></span>|<span data-ttu-id="37909-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37909-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37909-123">Accept</span><span class="sxs-lookup"><span data-stu-id="37909-123">Accept</span></span>|<span data-ttu-id="37909-124">application/json</span><span class="sxs-lookup"><span data-stu-id="37909-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37909-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="37909-125">Request body</span></span>
<span data-ttu-id="37909-126">在请求正文中，提供 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37909-126">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="37909-127">下表显示创建 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="37909-127">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="37909-128">属性</span><span class="sxs-lookup"><span data-stu-id="37909-128">Property</span></span>|<span data-ttu-id="37909-129">类型</span><span class="sxs-lookup"><span data-stu-id="37909-129">Type</span></span>|<span data-ttu-id="37909-130">说明</span><span class="sxs-lookup"><span data-stu-id="37909-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37909-131">id</span><span class="sxs-lookup"><span data-stu-id="37909-131">id</span></span>|<span data-ttu-id="37909-132">String</span><span class="sxs-lookup"><span data-stu-id="37909-132">String</span></span>|<span data-ttu-id="37909-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="37909-133">Key of the entity.</span></span> <span data-ttu-id="37909-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37909-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37909-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37909-135">lastModifiedDateTime</span></span>|<span data-ttu-id="37909-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37909-136">DateTimeOffset</span></span>|<span data-ttu-id="37909-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="37909-137">DateTime the object was last modified.</span></span> <span data-ttu-id="37909-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37909-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37909-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37909-139">createdDateTime</span></span>|<span data-ttu-id="37909-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37909-140">DateTimeOffset</span></span>|<span data-ttu-id="37909-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="37909-141">DateTime the object was created.</span></span> <span data-ttu-id="37909-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37909-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37909-143">description</span><span class="sxs-lookup"><span data-stu-id="37909-143">description</span></span>|<span data-ttu-id="37909-144">String</span><span class="sxs-lookup"><span data-stu-id="37909-144">String</span></span>|<span data-ttu-id="37909-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="37909-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37909-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37909-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37909-147">displayName</span><span class="sxs-lookup"><span data-stu-id="37909-147">displayName</span></span>|<span data-ttu-id="37909-148">String</span><span class="sxs-lookup"><span data-stu-id="37909-148">String</span></span>|<span data-ttu-id="37909-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="37909-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37909-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37909-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37909-151">version</span><span class="sxs-lookup"><span data-stu-id="37909-151">version</span></span>|<span data-ttu-id="37909-152">Int32</span><span class="sxs-lookup"><span data-stu-id="37909-152">Int32</span></span>|<span data-ttu-id="37909-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="37909-153">Version of the device configuration.</span></span> <span data-ttu-id="37909-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37909-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37909-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="37909-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="37909-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-156">Boolean</span></span>|<span data-ttu-id="37909-157">指示是否阻止剪贴板共享以在应用程序之间复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="37909-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="37909-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="37909-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="37909-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-159">Boolean</span></span>|<span data-ttu-id="37909-160">指示是否阻止在应用程序内复制和粘贴。</span><span class="sxs-lookup"><span data-stu-id="37909-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="37909-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="37909-161">appsBlockYouTube</span></span>|<span data-ttu-id="37909-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-162">Boolean</span></span>|<span data-ttu-id="37909-163">指示是否阻止 YouTube 应用。</span><span class="sxs-lookup"><span data-stu-id="37909-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="37909-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-164">bluetoothBlocked</span></span>|<span data-ttu-id="37909-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-165">Boolean</span></span>|<span data-ttu-id="37909-166">指示是否阻止蓝牙。</span><span class="sxs-lookup"><span data-stu-id="37909-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="37909-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-167">cameraBlocked</span></span>|<span data-ttu-id="37909-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-168">Boolean</span></span>|<span data-ttu-id="37909-169">指示是否阻止照相机的使用。</span><span class="sxs-lookup"><span data-stu-id="37909-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="37909-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="37909-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="37909-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-171">Boolean</span></span>|<span data-ttu-id="37909-172">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="37909-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="37909-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="37909-173">cellularBlockMessaging</span></span>|<span data-ttu-id="37909-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-174">Boolean</span></span>|<span data-ttu-id="37909-175">指示是否阻止 SMS/MMS 消息。</span><span class="sxs-lookup"><span data-stu-id="37909-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="37909-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="37909-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="37909-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-177">Boolean</span></span>|<span data-ttu-id="37909-178">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="37909-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="37909-179">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="37909-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="37909-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-180">Boolean</span></span>|<span data-ttu-id="37909-181">指示是否阻止同步 Wi-Fi 网络共享。</span><span class="sxs-lookup"><span data-stu-id="37909-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="37909-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="37909-182">compliantAppsList</span></span>|<span data-ttu-id="37909-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37909-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="37909-184">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="37909-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="37909-185">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="37909-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="37909-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="37909-186">compliantAppListType</span></span>|[<span data-ttu-id="37909-187">appListType</span><span class="sxs-lookup"><span data-stu-id="37909-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="37909-188">位于 CompliantAppsList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="37909-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="37909-189">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="37909-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="37909-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="37909-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="37909-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-191">Boolean</span></span>|<span data-ttu-id="37909-192">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="37909-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="37909-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-193">locationServicesBlocked</span></span>|<span data-ttu-id="37909-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-194">Boolean</span></span>|<span data-ttu-id="37909-195">指示是否阻止位置服务。</span><span class="sxs-lookup"><span data-stu-id="37909-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="37909-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="37909-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="37909-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-197">Boolean</span></span>|<span data-ttu-id="37909-198">指示是否阻止 Google 帐户自动同步。</span><span class="sxs-lookup"><span data-stu-id="37909-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="37909-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="37909-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-200">Boolean</span></span>|<span data-ttu-id="37909-201">指示是否阻止 Google Play 商店。</span><span class="sxs-lookup"><span data-stu-id="37909-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="37909-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="37909-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="37909-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-203">Boolean</span></span>|<span data-ttu-id="37909-204">指示在展台模式下是否阻止屏幕睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="37909-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="37909-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="37909-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="37909-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-206">Boolean</span></span>|<span data-ttu-id="37909-207">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="37909-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="37909-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="37909-208">kioskModeApps</span></span>|<span data-ttu-id="37909-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37909-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="37909-210">设备处于展台模式时将允许运行的应用列表。</span><span class="sxs-lookup"><span data-stu-id="37909-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="37909-211">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="37909-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37909-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-212">nfcBlocked</span></span>|<span data-ttu-id="37909-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-213">Boolean</span></span>|<span data-ttu-id="37909-214">指示是否阻止近场通信。</span><span class="sxs-lookup"><span data-stu-id="37909-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="37909-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="37909-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="37909-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-216">Boolean</span></span>|<span data-ttu-id="37909-217">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="37909-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="37909-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="37909-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="37909-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-219">Boolean</span></span>|<span data-ttu-id="37909-220">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="37909-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="37909-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="37909-221">passwordExpirationDays</span></span>|<span data-ttu-id="37909-222">Int32</span><span class="sxs-lookup"><span data-stu-id="37909-222">Int32</span></span>|<span data-ttu-id="37909-223">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="37909-223">Number of days before the password expires.</span></span> <span data-ttu-id="37909-224">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="37909-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="37909-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="37909-225">passwordMinimumLength</span></span>|<span data-ttu-id="37909-226">Int32</span><span class="sxs-lookup"><span data-stu-id="37909-226">Int32</span></span>|<span data-ttu-id="37909-227">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="37909-227">Minimum length of passwords.</span></span> <span data-ttu-id="37909-228">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="37909-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="37909-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="37909-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="37909-230">Int32</span><span class="sxs-lookup"><span data-stu-id="37909-230">Int32</span></span>|<span data-ttu-id="37909-231">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="37909-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="37909-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="37909-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="37909-233">Int32</span><span class="sxs-lookup"><span data-stu-id="37909-233">Int32</span></span>|<span data-ttu-id="37909-234">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="37909-234">Number of previous passwords to block.</span></span> <span data-ttu-id="37909-235">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="37909-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="37909-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="37909-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="37909-237">Int32</span><span class="sxs-lookup"><span data-stu-id="37909-237">Int32</span></span>|<span data-ttu-id="37909-238">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="37909-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="37909-239">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="37909-239">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37909-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="37909-240">passwordRequiredType</span></span>|[<span data-ttu-id="37909-241">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="37909-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="37909-242">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="37909-242">Type of password that is required.</span></span> <span data-ttu-id="37909-243">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="37909-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="37909-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="37909-244">passwordRequired</span></span>|<span data-ttu-id="37909-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-245">Boolean</span></span>|<span data-ttu-id="37909-246">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="37909-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="37909-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-247">powerOffBlocked</span></span>|<span data-ttu-id="37909-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-248">Boolean</span></span>|<span data-ttu-id="37909-249">指示是否阻止关闭设备。</span><span class="sxs-lookup"><span data-stu-id="37909-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="37909-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-250">factoryResetBlocked</span></span>|<span data-ttu-id="37909-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-251">Boolean</span></span>|<span data-ttu-id="37909-252">指示是否阻止用户执行恢复出厂设置。</span><span class="sxs-lookup"><span data-stu-id="37909-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="37909-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-253">screenCaptureBlocked</span></span>|<span data-ttu-id="37909-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-254">Boolean</span></span>|<span data-ttu-id="37909-255">指示是否阻止屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="37909-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="37909-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="37909-256">deviceSharingAllowed</span></span>|<span data-ttu-id="37909-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-257">Boolean</span></span>|<span data-ttu-id="37909-258">指示是否允许设备共享模式。</span><span class="sxs-lookup"><span data-stu-id="37909-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="37909-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="37909-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="37909-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-260">Boolean</span></span>|<span data-ttu-id="37909-261">指示是否阻止 Google 备份。</span><span class="sxs-lookup"><span data-stu-id="37909-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="37909-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="37909-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="37909-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-263">Boolean</span></span>|<span data-ttu-id="37909-264">指示是否阻止可移动存储使用。</span><span class="sxs-lookup"><span data-stu-id="37909-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="37909-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="37909-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="37909-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-266">Boolean</span></span>|<span data-ttu-id="37909-267">指示是否需要设备加密。</span><span class="sxs-lookup"><span data-stu-id="37909-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="37909-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="37909-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="37909-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-269">Boolean</span></span>|<span data-ttu-id="37909-270">指示是否需要可移动存储加密。</span><span class="sxs-lookup"><span data-stu-id="37909-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="37909-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="37909-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-272">Boolean</span></span>|<span data-ttu-id="37909-273">指示是否阻止使用语音助手。</span><span class="sxs-lookup"><span data-stu-id="37909-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="37909-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-274">voiceDialingBlocked</span></span>|<span data-ttu-id="37909-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-275">Boolean</span></span>|<span data-ttu-id="37909-276">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="37909-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="37909-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="37909-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="37909-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-278">Boolean</span></span>|<span data-ttu-id="37909-279">指示是否阻止 Web 浏览器内的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="37909-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="37909-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="37909-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="37909-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-281">Boolean</span></span>|<span data-ttu-id="37909-282">指示是否阻止 Web 浏览器的自动填充功能。</span><span class="sxs-lookup"><span data-stu-id="37909-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="37909-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="37909-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="37909-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-284">Boolean</span></span>|<span data-ttu-id="37909-285">指示是否阻止 Web 浏览器内的 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="37909-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="37909-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-286">webBrowserBlocked</span></span>|<span data-ttu-id="37909-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-287">Boolean</span></span>|<span data-ttu-id="37909-288">指示是否阻止 Web 浏览器。</span><span class="sxs-lookup"><span data-stu-id="37909-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="37909-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="37909-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="37909-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="37909-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="37909-291">Web 浏览器内的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="37909-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="37909-292">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="37909-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="37909-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="37909-293">wiFiBlocked</span></span>|<span data-ttu-id="37909-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-294">Boolean</span></span>|<span data-ttu-id="37909-295">指示是否阻止同步 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="37909-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="37909-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="37909-296">appsInstallAllowList</span></span>|<span data-ttu-id="37909-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37909-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="37909-298">可以在 KNOX 设备上安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="37909-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="37909-299">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="37909-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37909-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="37909-300">appsLaunchBlockList</span></span>|<span data-ttu-id="37909-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37909-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="37909-302">阻止在 KNOX 设备上启动的应用列表。</span><span class="sxs-lookup"><span data-stu-id="37909-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="37909-303">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="37909-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37909-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="37909-304">appsHideList</span></span>|<span data-ttu-id="37909-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37909-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="37909-306">要在 KNOX 设备上隐藏的应用列表。</span><span class="sxs-lookup"><span data-stu-id="37909-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="37909-307">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="37909-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37909-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="37909-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="37909-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="37909-309">Boolean</span></span>|<span data-ttu-id="37909-310">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="37909-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="37909-311">响应</span><span class="sxs-lookup"><span data-stu-id="37909-311">Response</span></span>
<span data-ttu-id="37909-312">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37909-312">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37909-313">示例</span><span class="sxs-lookup"><span data-stu-id="37909-313">Example</span></span>

### <a name="request"></a><span data-ttu-id="37909-314">请求</span><span class="sxs-lookup"><span data-stu-id="37909-314">Request</span></span>
<span data-ttu-id="37909-315">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37909-315">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37909-316">响应</span><span class="sxs-lookup"><span data-stu-id="37909-316">Response</span></span>
<span data-ttu-id="37909-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37909-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



