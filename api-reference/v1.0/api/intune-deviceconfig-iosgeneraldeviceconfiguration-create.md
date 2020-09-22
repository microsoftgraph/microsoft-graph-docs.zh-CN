---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb12b8650123860ce2586f5027f44d4ccecdc797
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979131"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="97f1f-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="97f1f-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="97f1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97f1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97f1f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97f1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97f1f-106">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97f1f-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97f1f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="97f1f-107">Prerequisites</span></span>
<span data-ttu-id="97f1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97f1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97f1f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97f1f-110">Permission type</span></span>|<span data-ttu-id="97f1f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="97f1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97f1f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97f1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97f1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97f1f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97f1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97f1f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="97f1f-115">Not supported.</span></span>|
|<span data-ttu-id="97f1f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="97f1f-116">Application</span></span>|<span data-ttu-id="97f1f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="97f1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97f1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97f1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="97f1f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="97f1f-119">Request headers</span></span>
|<span data-ttu-id="97f1f-120">标头</span><span class="sxs-lookup"><span data-stu-id="97f1f-120">Header</span></span>|<span data-ttu-id="97f1f-121">值</span><span class="sxs-lookup"><span data-stu-id="97f1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97f1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97f1f-122">Authorization</span></span>|<span data-ttu-id="97f1f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="97f1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97f1f-124">接受</span><span class="sxs-lookup"><span data-stu-id="97f1f-124">Accept</span></span>|<span data-ttu-id="97f1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97f1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97f1f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="97f1f-126">Request body</span></span>
<span data-ttu-id="97f1f-127">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97f1f-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="97f1f-128">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="97f1f-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="97f1f-129">属性</span><span class="sxs-lookup"><span data-stu-id="97f1f-129">Property</span></span>|<span data-ttu-id="97f1f-130">类型</span><span class="sxs-lookup"><span data-stu-id="97f1f-130">Type</span></span>|<span data-ttu-id="97f1f-131">说明</span><span class="sxs-lookup"><span data-stu-id="97f1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97f1f-132">id</span><span class="sxs-lookup"><span data-stu-id="97f1f-132">id</span></span>|<span data-ttu-id="97f1f-133">String</span><span class="sxs-lookup"><span data-stu-id="97f1f-133">String</span></span>|<span data-ttu-id="97f1f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="97f1f-134">Key of the entity.</span></span> <span data-ttu-id="97f1f-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97f1f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97f1f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97f1f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="97f1f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97f1f-137">DateTimeOffset</span></span>|<span data-ttu-id="97f1f-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97f1f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="97f1f-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97f1f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97f1f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97f1f-140">createdDateTime</span></span>|<span data-ttu-id="97f1f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97f1f-141">DateTimeOffset</span></span>|<span data-ttu-id="97f1f-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="97f1f-142">DateTime the object was created.</span></span> <span data-ttu-id="97f1f-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97f1f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97f1f-144">description</span><span class="sxs-lookup"><span data-stu-id="97f1f-144">description</span></span>|<span data-ttu-id="97f1f-145">String</span><span class="sxs-lookup"><span data-stu-id="97f1f-145">String</span></span>|<span data-ttu-id="97f1f-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="97f1f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97f1f-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97f1f-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97f1f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="97f1f-148">displayName</span></span>|<span data-ttu-id="97f1f-149">String</span><span class="sxs-lookup"><span data-stu-id="97f1f-149">String</span></span>|<span data-ttu-id="97f1f-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="97f1f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97f1f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97f1f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97f1f-152">version</span><span class="sxs-lookup"><span data-stu-id="97f1f-152">version</span></span>|<span data-ttu-id="97f1f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-153">Int32</span></span>|<span data-ttu-id="97f1f-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="97f1f-154">Version of the device configuration.</span></span> <span data-ttu-id="97f1f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97f1f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97f1f-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-156">accountBlockModification</span></span>|<span data-ttu-id="97f1f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-157">Boolean</span></span>|<span data-ttu-id="97f1f-158">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="97f1f-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="97f1f-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="97f1f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-160">Boolean</span></span>|<span data-ttu-id="97f1f-161">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="97f1f-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="97f1f-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-162">airDropBlocked</span></span>|<span data-ttu-id="97f1f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-163">Boolean</span></span>|<span data-ttu-id="97f1f-164">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="97f1f-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="97f1f-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="97f1f-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-166">Boolean</span></span>|<span data-ttu-id="97f1f-167">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="97f1f-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="97f1f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-169">Boolean</span></span>|<span data-ttu-id="97f1f-170">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="97f1f-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="97f1f-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="97f1f-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="97f1f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-172">Boolean</span></span>|<span data-ttu-id="97f1f-173">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="97f1f-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="97f1f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-175">Boolean</span></span>|<span data-ttu-id="97f1f-176">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="97f1f-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-177">appleNewsBlocked</span></span>|<span data-ttu-id="97f1f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-178">Boolean</span></span>|<span data-ttu-id="97f1f-179">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="97f1f-180">appsSingleAppModeList</span></span>|<span data-ttu-id="97f1f-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="97f1f-182">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="97f1f-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="97f1f-183">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="97f1f-183">Supervised only.</span></span> <span data-ttu-id="97f1f-184">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="97f1f-184">iOS 7.0 and later.</span></span> <span data-ttu-id="97f1f-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="97f1f-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="97f1f-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="97f1f-186">appsVisibilityList</span></span>|<span data-ttu-id="97f1f-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="97f1f-188">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="97f1f-189">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="97f1f-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="97f1f-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="97f1f-190">appsVisibilityListType</span></span>|[<span data-ttu-id="97f1f-191">appListType</span><span class="sxs-lookup"><span data-stu-id="97f1f-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="97f1f-192">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="97f1f-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="97f1f-193">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="97f1f-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="97f1f-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="97f1f-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="97f1f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-195">Boolean</span></span>|<span data-ttu-id="97f1f-196">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-197">appStoreBlocked</span></span>|<span data-ttu-id="97f1f-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-198">Boolean</span></span>|<span data-ttu-id="97f1f-199">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="97f1f-199">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="97f1f-200">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="97f1f-200">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="97f1f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-201">Boolean</span></span>|<span data-ttu-id="97f1f-202">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="97f1f-202">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="97f1f-203">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="97f1f-203">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="97f1f-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-204">Boolean</span></span>|<span data-ttu-id="97f1f-205">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="97f1f-205">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="97f1f-206">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-206">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-207">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="97f1f-207">appStoreRequirePassword</span></span>|<span data-ttu-id="97f1f-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-208">Boolean</span></span>|<span data-ttu-id="97f1f-209">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="97f1f-209">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="97f1f-210">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-210">bluetoothBlockModification</span></span>|<span data-ttu-id="97f1f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-211">Boolean</span></span>|<span data-ttu-id="97f1f-212">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-212">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="97f1f-213">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-213">cameraBlocked</span></span>|<span data-ttu-id="97f1f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-214">Boolean</span></span>|<span data-ttu-id="97f1f-215">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="97f1f-215">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="97f1f-216">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="97f1f-216">cellularBlockDataRoaming</span></span>|<span data-ttu-id="97f1f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-217">Boolean</span></span>|<span data-ttu-id="97f1f-218">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="97f1f-218">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="97f1f-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="97f1f-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="97f1f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-220">Boolean</span></span>|<span data-ttu-id="97f1f-221">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="97f1f-221">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="97f1f-222">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-222">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="97f1f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-223">Boolean</span></span>|<span data-ttu-id="97f1f-224">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-224">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-225">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="97f1f-225">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="97f1f-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-226">Boolean</span></span>|<span data-ttu-id="97f1f-227">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="97f1f-227">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="97f1f-228">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="97f1f-228">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="97f1f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-229">Boolean</span></span>|<span data-ttu-id="97f1f-230">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="97f1f-230">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="97f1f-231">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="97f1f-231">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="97f1f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-232">Boolean</span></span>|<span data-ttu-id="97f1f-233">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="97f1f-233">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="97f1f-234">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="97f1f-234">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="97f1f-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-235">Boolean</span></span>|<span data-ttu-id="97f1f-236">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-236">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="97f1f-237">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="97f1f-237">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="97f1f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-238">Boolean</span></span>|<span data-ttu-id="97f1f-239">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="97f1f-239">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-240">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="97f1f-240">compliantAppsList</span></span>|<span data-ttu-id="97f1f-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="97f1f-242">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-242">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="97f1f-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="97f1f-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="97f1f-244">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="97f1f-244">compliantAppListType</span></span>|[<span data-ttu-id="97f1f-245">appListType</span><span class="sxs-lookup"><span data-stu-id="97f1f-245">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="97f1f-246">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="97f1f-246">List that is in the AppComplianceList.</span></span> <span data-ttu-id="97f1f-247">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="97f1f-247">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="97f1f-248">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="97f1f-248">configurationProfileBlockChanges</span></span>|<span data-ttu-id="97f1f-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-249">Boolean</span></span>|<span data-ttu-id="97f1f-250">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="97f1f-250">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-251">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-251">definitionLookupBlocked</span></span>|<span data-ttu-id="97f1f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-252">Boolean</span></span>|<span data-ttu-id="97f1f-253">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-253">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="97f1f-254">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="97f1f-254">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="97f1f-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-255">Boolean</span></span>|<span data-ttu-id="97f1f-256">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="97f1f-256">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-257">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-257">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="97f1f-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-258">Boolean</span></span>|<span data-ttu-id="97f1f-259">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="97f1f-259">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-260">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-260">deviceBlockNameModification</span></span>|<span data-ttu-id="97f1f-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-261">Boolean</span></span>|<span data-ttu-id="97f1f-262">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-262">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-263">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="97f1f-263">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="97f1f-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-264">Boolean</span></span>|<span data-ttu-id="97f1f-265">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="97f1f-265">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="97f1f-266">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-266">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="97f1f-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-267">Boolean</span></span>|<span data-ttu-id="97f1f-268">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-268">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="97f1f-269">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="97f1f-269">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="97f1f-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-270">Boolean</span></span>|<span data-ttu-id="97f1f-271">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="97f1f-271">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="97f1f-272">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="97f1f-272">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="97f1f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-273">Boolean</span></span>|<span data-ttu-id="97f1f-274">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="97f1f-274">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="97f1f-275">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="97f1f-275">emailInDomainSuffixes</span></span>|<span data-ttu-id="97f1f-276">String 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-276">String collection</span></span>|<span data-ttu-id="97f1f-277">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="97f1f-277">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="97f1f-278">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="97f1f-278">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="97f1f-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-279">Boolean</span></span>|<span data-ttu-id="97f1f-280">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="97f1f-280">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="97f1f-281">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-281">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="97f1f-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-282">Boolean</span></span>|<span data-ttu-id="97f1f-283">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-283">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="97f1f-284">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-284">faceTimeBlocked</span></span>|<span data-ttu-id="97f1f-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-285">Boolean</span></span>|<span data-ttu-id="97f1f-286">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="97f1f-286">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="97f1f-287">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-287">findMyFriendsBlocked</span></span>|<span data-ttu-id="97f1f-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-288">Boolean</span></span>|<span data-ttu-id="97f1f-289">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="97f1f-289">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-290">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="97f1f-290">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="97f1f-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-291">Boolean</span></span>|<span data-ttu-id="97f1f-292">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="97f1f-292">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="97f1f-293">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="97f1f-293">gamingBlockMultiplayer</span></span>|<span data-ttu-id="97f1f-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-294">Boolean</span></span>|<span data-ttu-id="97f1f-295">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="97f1f-295">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="97f1f-296">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-296">gameCenterBlocked</span></span>|<span data-ttu-id="97f1f-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-297">Boolean</span></span>|<span data-ttu-id="97f1f-298">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="97f1f-298">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-299">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-299">hostPairingBlocked</span></span>|<span data-ttu-id="97f1f-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-300">Boolean</span></span>|<span data-ttu-id="97f1f-301">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="97f1f-301">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-302">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-302">iBooksStoreBlocked</span></span>|<span data-ttu-id="97f1f-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-303">Boolean</span></span>|<span data-ttu-id="97f1f-304">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="97f1f-304">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-305">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="97f1f-305">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="97f1f-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-306">Boolean</span></span>|<span data-ttu-id="97f1f-307">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="97f1f-307">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="97f1f-308">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="97f1f-308">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="97f1f-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-309">Boolean</span></span>|<span data-ttu-id="97f1f-310">指示是否阻止用户将其在 iOS 设备上启动的工作继续到另一个 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="97f1f-310">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="97f1f-311">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="97f1f-311">iCloudBlockBackup</span></span>|<span data-ttu-id="97f1f-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-312">Boolean</span></span>|<span data-ttu-id="97f1f-313">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="97f1f-313">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="97f1f-314">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="97f1f-314">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="97f1f-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-315">Boolean</span></span>|<span data-ttu-id="97f1f-316">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="97f1f-316">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="97f1f-317">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="97f1f-317">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="97f1f-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-318">Boolean</span></span>|<span data-ttu-id="97f1f-319">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="97f1f-319">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="97f1f-320">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="97f1f-320">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="97f1f-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-321">Boolean</span></span>|<span data-ttu-id="97f1f-322">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="97f1f-322">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="97f1f-323">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="97f1f-323">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="97f1f-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-324">Boolean</span></span>|<span data-ttu-id="97f1f-325">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="97f1f-325">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="97f1f-326">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="97f1f-326">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="97f1f-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-327">Boolean</span></span>|<span data-ttu-id="97f1f-328">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="97f1f-328">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="97f1f-329">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="97f1f-329">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="97f1f-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-330">Boolean</span></span>|<span data-ttu-id="97f1f-331">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="97f1f-331">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="97f1f-332">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="97f1f-332">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="97f1f-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-333">Boolean</span></span>|<span data-ttu-id="97f1f-334">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="97f1f-334">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="97f1f-335">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="97f1f-335">iTunesBlockMusicService</span></span>|<span data-ttu-id="97f1f-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-336">Boolean</span></span>|<span data-ttu-id="97f1f-337">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-337">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="97f1f-338">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="97f1f-338">iTunesBlockRadio</span></span>|<span data-ttu-id="97f1f-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-339">Boolean</span></span>|<span data-ttu-id="97f1f-340">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-340">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="97f1f-341">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="97f1f-341">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="97f1f-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-342">Boolean</span></span>|<span data-ttu-id="97f1f-343">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-343">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="97f1f-344">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="97f1f-344">keyboardBlockDictation</span></span>|<span data-ttu-id="97f1f-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-345">Boolean</span></span>|<span data-ttu-id="97f1f-346">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="97f1f-346">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-347">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="97f1f-347">keyboardBlockPredictive</span></span>|<span data-ttu-id="97f1f-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-348">Boolean</span></span>|<span data-ttu-id="97f1f-349">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-349">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="97f1f-350">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="97f1f-350">keyboardBlockShortcuts</span></span>|<span data-ttu-id="97f1f-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-351">Boolean</span></span>|<span data-ttu-id="97f1f-352">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-352">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-353">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="97f1f-353">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="97f1f-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-354">Boolean</span></span>|<span data-ttu-id="97f1f-355">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-355">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="97f1f-356">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="97f1f-356">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="97f1f-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-357">Boolean</span></span>|<span data-ttu-id="97f1f-358">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="97f1f-358">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-359">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-359">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="97f1f-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-360">Boolean</span></span>|<span data-ttu-id="97f1f-361">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-361">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-362">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="97f1f-362">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="97f1f-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-363">Boolean</span></span>|<span data-ttu-id="97f1f-364">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="97f1f-364">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-365">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-365">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="97f1f-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-366">Boolean</span></span>|<span data-ttu-id="97f1f-367">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-367">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-368">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="97f1f-368">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="97f1f-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-369">Boolean</span></span>|<span data-ttu-id="97f1f-370">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="97f1f-370">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-371">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="97f1f-371">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="97f1f-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-372">Boolean</span></span>|<span data-ttu-id="97f1f-373">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="97f1f-373">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-374">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="97f1f-374">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="97f1f-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-375">Boolean</span></span>|<span data-ttu-id="97f1f-376">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="97f1f-376">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-377">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="97f1f-377">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="97f1f-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-378">Boolean</span></span>|<span data-ttu-id="97f1f-379">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="97f1f-379">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-380">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-380">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="97f1f-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-381">Boolean</span></span>|<span data-ttu-id="97f1f-382">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-382">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-383">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="97f1f-383">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="97f1f-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-384">Boolean</span></span>|<span data-ttu-id="97f1f-385">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="97f1f-385">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-386">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-386">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="97f1f-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-387">Boolean</span></span>|<span data-ttu-id="97f1f-388">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-388">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-389">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="97f1f-389">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="97f1f-390">String</span><span class="sxs-lookup"><span data-stu-id="97f1f-390">String</span></span>|<span data-ttu-id="97f1f-391">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="97f1f-391">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="97f1f-392">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="97f1f-392">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="97f1f-393">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="97f1f-393">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="97f1f-394">String</span><span class="sxs-lookup"><span data-stu-id="97f1f-394">String</span></span>|<span data-ttu-id="97f1f-395">用于展台模式的内置应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="97f1f-395">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="97f1f-396">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="97f1f-396">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="97f1f-397">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="97f1f-397">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="97f1f-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-398">Boolean</span></span>|<span data-ttu-id="97f1f-399">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="97f1f-399">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-400">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="97f1f-400">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="97f1f-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-401">Boolean</span></span>|<span data-ttu-id="97f1f-402">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="97f1f-402">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-403">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="97f1f-403">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="97f1f-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-404">Boolean</span></span>|<span data-ttu-id="97f1f-405">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="97f1f-405">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-406">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="97f1f-406">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="97f1f-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-407">Boolean</span></span>|<span data-ttu-id="97f1f-408">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="97f1f-408">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-409">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="97f1f-409">kioskModeRequireZoom</span></span>|<span data-ttu-id="97f1f-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-410">Boolean</span></span>|<span data-ttu-id="97f1f-411">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="97f1f-411">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="97f1f-412">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="97f1f-412">kioskModeManagedAppId</span></span>|<span data-ttu-id="97f1f-413">String</span><span class="sxs-lookup"><span data-stu-id="97f1f-413">String</span></span>|<span data-ttu-id="97f1f-414">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="97f1f-414">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="97f1f-415">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="97f1f-415">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="97f1f-416">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="97f1f-416">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="97f1f-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-417">Boolean</span></span>|<span data-ttu-id="97f1f-418">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="97f1f-418">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="97f1f-419">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="97f1f-419">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="97f1f-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-420">Boolean</span></span>|<span data-ttu-id="97f1f-421">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="97f1f-421">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="97f1f-422">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="97f1f-422">lockScreenBlockPassbook</span></span>|<span data-ttu-id="97f1f-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-423">Boolean</span></span>|<span data-ttu-id="97f1f-424">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="97f1f-424">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="97f1f-425">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="97f1f-425">lockScreenBlockTodayView</span></span>|<span data-ttu-id="97f1f-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-426">Boolean</span></span>|<span data-ttu-id="97f1f-427">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="97f1f-427">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="97f1f-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="97f1f-428">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="97f1f-429">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="97f1f-429">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="97f1f-430">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-430">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="97f1f-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="97f1f-431">mediaContentRatingCanada</span></span>|[<span data-ttu-id="97f1f-432">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="97f1f-432">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="97f1f-433">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-433">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="97f1f-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="97f1f-434">mediaContentRatingFrance</span></span>|[<span data-ttu-id="97f1f-435">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="97f1f-435">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="97f1f-436">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-436">Media content rating settings for France</span></span>|
|<span data-ttu-id="97f1f-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="97f1f-437">mediaContentRatingGermany</span></span>|[<span data-ttu-id="97f1f-438">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="97f1f-438">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="97f1f-439">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-439">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="97f1f-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="97f1f-440">mediaContentRatingIreland</span></span>|[<span data-ttu-id="97f1f-441">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="97f1f-441">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="97f1f-442">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-442">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="97f1f-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="97f1f-443">mediaContentRatingJapan</span></span>|[<span data-ttu-id="97f1f-444">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="97f1f-444">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="97f1f-445">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-445">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="97f1f-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="97f1f-446">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="97f1f-447">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="97f1f-447">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="97f1f-448">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-448">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="97f1f-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="97f1f-449">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="97f1f-450">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="97f1f-450">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="97f1f-451">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-451">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="97f1f-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="97f1f-452">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="97f1f-453">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="97f1f-453">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="97f1f-454">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="97f1f-454">Media content rating settings for United States</span></span>|
|<span data-ttu-id="97f1f-455">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="97f1f-455">networkUsageRules</span></span>|<span data-ttu-id="97f1f-456">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-456">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="97f1f-457">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="97f1f-457">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="97f1f-458">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="97f1f-458">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="97f1f-459">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="97f1f-459">mediaContentRatingApps</span></span>|[<span data-ttu-id="97f1f-460">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="97f1f-460">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="97f1f-461">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-461">Media content rating settings for Apps.</span></span> <span data-ttu-id="97f1f-462">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="97f1f-462">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="97f1f-463">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-463">messagesBlocked</span></span>|<span data-ttu-id="97f1f-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-464">Boolean</span></span>|<span data-ttu-id="97f1f-465">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="97f1f-465">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="97f1f-466">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-466">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="97f1f-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-467">Boolean</span></span>|<span data-ttu-id="97f1f-468">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-468">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="97f1f-469">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="97f1f-469">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="97f1f-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-470">Boolean</span></span>|<span data-ttu-id="97f1f-471">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="97f1f-471">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="97f1f-472">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-472">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="97f1f-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-473">Boolean</span></span>|<span data-ttu-id="97f1f-474">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="97f1f-474">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="97f1f-475">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-475">passcodeBlockModification</span></span>|<span data-ttu-id="97f1f-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-476">Boolean</span></span>|<span data-ttu-id="97f1f-477">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-477">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="97f1f-478">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="97f1f-478">passcodeBlockSimple</span></span>|<span data-ttu-id="97f1f-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-479">Boolean</span></span>|<span data-ttu-id="97f1f-480">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="97f1f-480">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="97f1f-481">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="97f1f-481">passcodeExpirationDays</span></span>|<span data-ttu-id="97f1f-482">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-482">Int32</span></span>|<span data-ttu-id="97f1f-483">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="97f1f-483">Number of days before the passcode expires.</span></span> <span data-ttu-id="97f1f-484">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="97f1f-484">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="97f1f-485">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="97f1f-485">passcodeMinimumLength</span></span>|<span data-ttu-id="97f1f-486">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-486">Int32</span></span>|<span data-ttu-id="97f1f-487">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="97f1f-487">Minimum length of passcode.</span></span> <span data-ttu-id="97f1f-488">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="97f1f-488">Valid values 4 to 14</span></span>|
|<span data-ttu-id="97f1f-489">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="97f1f-489">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="97f1f-490">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-490">Int32</span></span>|<span data-ttu-id="97f1f-491">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="97f1f-491">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="97f1f-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="97f1f-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="97f1f-493">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-493">Int32</span></span>|<span data-ttu-id="97f1f-494">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="97f1f-494">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="97f1f-495">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="97f1f-495">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="97f1f-496">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-496">Int32</span></span>|<span data-ttu-id="97f1f-497">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="97f1f-497">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="97f1f-498">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="97f1f-498">Valid values 0 to 4</span></span>|
|<span data-ttu-id="97f1f-499">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="97f1f-499">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="97f1f-500">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-500">Int32</span></span>|<span data-ttu-id="97f1f-501">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="97f1f-501">Number of previous passcodes to block.</span></span> <span data-ttu-id="97f1f-502">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="97f1f-502">Valid values 1 to 24</span></span>|
|<span data-ttu-id="97f1f-503">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="97f1f-503">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="97f1f-504">Int32</span><span class="sxs-lookup"><span data-stu-id="97f1f-504">Int32</span></span>|<span data-ttu-id="97f1f-505">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="97f1f-505">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="97f1f-506">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="97f1f-506">Valid values 4 to 11</span></span>|
|<span data-ttu-id="97f1f-507">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="97f1f-507">passcodeRequiredType</span></span>|[<span data-ttu-id="97f1f-508">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="97f1f-508">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="97f1f-509">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="97f1f-509">Type of passcode that is required.</span></span> <span data-ttu-id="97f1f-510">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="97f1f-510">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="97f1f-511">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="97f1f-511">passcodeRequired</span></span>|<span data-ttu-id="97f1f-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-512">Boolean</span></span>|<span data-ttu-id="97f1f-513">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="97f1f-513">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="97f1f-514">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-514">podcastsBlocked</span></span>|<span data-ttu-id="97f1f-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-515">Boolean</span></span>|<span data-ttu-id="97f1f-516">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-516">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="97f1f-517">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="97f1f-517">safariBlockAutofill</span></span>|<span data-ttu-id="97f1f-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-518">Boolean</span></span>|<span data-ttu-id="97f1f-519">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="97f1f-519">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="97f1f-520">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="97f1f-520">safariBlockJavaScript</span></span>|<span data-ttu-id="97f1f-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-521">Boolean</span></span>|<span data-ttu-id="97f1f-522">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="97f1f-522">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="97f1f-523">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="97f1f-523">safariBlockPopups</span></span>|<span data-ttu-id="97f1f-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-524">Boolean</span></span>|<span data-ttu-id="97f1f-525">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="97f1f-525">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="97f1f-526">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-526">safariBlocked</span></span>|<span data-ttu-id="97f1f-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-527">Boolean</span></span>|<span data-ttu-id="97f1f-528">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="97f1f-528">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="97f1f-529">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-529">safariCookieSettings</span></span>|[<span data-ttu-id="97f1f-530">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="97f1f-530">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="97f1f-531">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="97f1f-531">Cookie settings for Safari.</span></span> <span data-ttu-id="97f1f-532">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="97f1f-532">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="97f1f-533">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="97f1f-533">safariManagedDomains</span></span>|<span data-ttu-id="97f1f-534">String 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-534">String collection</span></span>|<span data-ttu-id="97f1f-535">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="97f1f-535">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="97f1f-536">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="97f1f-536">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="97f1f-537">String 集合</span><span class="sxs-lookup"><span data-stu-id="97f1f-537">String collection</span></span>|<span data-ttu-id="97f1f-538">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="97f1f-538">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="97f1f-539">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-539">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="97f1f-540">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="97f1f-540">safariRequireFraudWarning</span></span>|<span data-ttu-id="97f1f-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-541">Boolean</span></span>|<span data-ttu-id="97f1f-542">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="97f1f-542">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="97f1f-543">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-543">screenCaptureBlocked</span></span>|<span data-ttu-id="97f1f-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-544">Boolean</span></span>|<span data-ttu-id="97f1f-545">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="97f1f-545">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="97f1f-546">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-546">siriBlocked</span></span>|<span data-ttu-id="97f1f-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-547">Boolean</span></span>|<span data-ttu-id="97f1f-548">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="97f1f-548">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="97f1f-549">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-549">siriBlockedWhenLocked</span></span>|<span data-ttu-id="97f1f-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-550">Boolean</span></span>|<span data-ttu-id="97f1f-551">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="97f1f-551">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="97f1f-552">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="97f1f-552">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="97f1f-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-553">Boolean</span></span>|<span data-ttu-id="97f1f-554">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="97f1f-554">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="97f1f-555">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="97f1f-555">siriRequireProfanityFilter</span></span>|<span data-ttu-id="97f1f-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-556">Boolean</span></span>|<span data-ttu-id="97f1f-557">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="97f1f-557">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="97f1f-558">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="97f1f-558">spotlightBlockInternetResults</span></span>|<span data-ttu-id="97f1f-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-559">Boolean</span></span>|<span data-ttu-id="97f1f-560">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="97f1f-560">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="97f1f-561">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="97f1f-561">voiceDialingBlocked</span></span>|<span data-ttu-id="97f1f-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-562">Boolean</span></span>|<span data-ttu-id="97f1f-563">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="97f1f-563">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="97f1f-564">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="97f1f-564">wallpaperBlockModification</span></span>|<span data-ttu-id="97f1f-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-565">Boolean</span></span>|<span data-ttu-id="97f1f-566">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="97f1f-566">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="97f1f-567">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="97f1f-567">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="97f1f-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f1f-568">Boolean</span></span>|<span data-ttu-id="97f1f-569">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="97f1f-569">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="97f1f-570">响应</span><span class="sxs-lookup"><span data-stu-id="97f1f-570">Response</span></span>
<span data-ttu-id="97f1f-571">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97f1f-571">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97f1f-572">示例</span><span class="sxs-lookup"><span data-stu-id="97f1f-572">Example</span></span>

### <a name="request"></a><span data-ttu-id="97f1f-573">请求</span><span class="sxs-lookup"><span data-stu-id="97f1f-573">Request</span></span>
<span data-ttu-id="97f1f-574">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97f1f-574">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="97f1f-575">响应</span><span class="sxs-lookup"><span data-stu-id="97f1f-575">Response</span></span>
<span data-ttu-id="97f1f-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97f1f-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```









