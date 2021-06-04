---
title: 更新 iosGeneralDeviceConfiguration
description: 更新 iosGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 679996c701f076c98047b71e5d57fae479e5751b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753865"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="e4f89-103">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4f89-103">Update iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e4f89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4f89-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4f89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4f89-106">更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4f89-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4f89-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4f89-107">Prerequisites</span></span>
<span data-ttu-id="e4f89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4f89-110">Permission type</span></span>|<span data-ttu-id="e4f89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4f89-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4f89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4f89-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f89-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4f89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4f89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f89-115">Not supported.</span></span>|
|<span data-ttu-id="e4f89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4f89-116">Application</span></span>|<span data-ttu-id="e4f89-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f89-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4f89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4f89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e4f89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4f89-119">Request headers</span></span>
|<span data-ttu-id="e4f89-120">标头</span><span class="sxs-lookup"><span data-stu-id="e4f89-120">Header</span></span>|<span data-ttu-id="e4f89-121">值</span><span class="sxs-lookup"><span data-stu-id="e4f89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4f89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4f89-122">Authorization</span></span>|<span data-ttu-id="e4f89-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4f89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4f89-124">接受</span><span class="sxs-lookup"><span data-stu-id="e4f89-124">Accept</span></span>|<span data-ttu-id="e4f89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4f89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4f89-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4f89-126">Request body</span></span>
<span data-ttu-id="e4f89-127">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f89-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e4f89-128">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4f89-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e4f89-129">属性</span><span class="sxs-lookup"><span data-stu-id="e4f89-129">Property</span></span>|<span data-ttu-id="e4f89-130">类型</span><span class="sxs-lookup"><span data-stu-id="e4f89-130">Type</span></span>|<span data-ttu-id="e4f89-131">说明</span><span class="sxs-lookup"><span data-stu-id="e4f89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4f89-132">id</span><span class="sxs-lookup"><span data-stu-id="e4f89-132">id</span></span>|<span data-ttu-id="e4f89-133">String</span><span class="sxs-lookup"><span data-stu-id="e4f89-133">String</span></span>|<span data-ttu-id="e4f89-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e4f89-134">Key of the entity.</span></span> <span data-ttu-id="e4f89-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4f89-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4f89-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f89-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e4f89-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f89-137">DateTimeOffset</span></span>|<span data-ttu-id="e4f89-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e4f89-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e4f89-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4f89-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4f89-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f89-140">createdDateTime</span></span>|<span data-ttu-id="e4f89-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f89-141">DateTimeOffset</span></span>|<span data-ttu-id="e4f89-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e4f89-142">DateTime the object was created.</span></span> <span data-ttu-id="e4f89-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4f89-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4f89-144">说明</span><span class="sxs-lookup"><span data-stu-id="e4f89-144">description</span></span>|<span data-ttu-id="e4f89-145">String</span><span class="sxs-lookup"><span data-stu-id="e4f89-145">String</span></span>|<span data-ttu-id="e4f89-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e4f89-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4f89-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4f89-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4f89-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e4f89-148">displayName</span></span>|<span data-ttu-id="e4f89-149">String</span><span class="sxs-lookup"><span data-stu-id="e4f89-149">String</span></span>|<span data-ttu-id="e4f89-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e4f89-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4f89-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4f89-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4f89-152">version</span><span class="sxs-lookup"><span data-stu-id="e4f89-152">version</span></span>|<span data-ttu-id="e4f89-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-153">Int32</span></span>|<span data-ttu-id="e4f89-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e4f89-154">Version of the device configuration.</span></span> <span data-ttu-id="e4f89-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4f89-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4f89-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-156">accountBlockModification</span></span>|<span data-ttu-id="e4f89-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-157">Boolean</span></span>|<span data-ttu-id="e4f89-158">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="e4f89-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="e4f89-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="e4f89-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-160">Boolean</span></span>|<span data-ttu-id="e4f89-161">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="e4f89-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="e4f89-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-162">airDropBlocked</span></span>|<span data-ttu-id="e4f89-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-163">Boolean</span></span>|<span data-ttu-id="e4f89-164">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="e4f89-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="e4f89-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="e4f89-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-166">Boolean</span></span>|<span data-ttu-id="e4f89-167">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="e4f89-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="e4f89-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-169">Boolean</span></span>|<span data-ttu-id="e4f89-170">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="e4f89-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="e4f89-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="e4f89-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="e4f89-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-172">Boolean</span></span>|<span data-ttu-id="e4f89-173">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="e4f89-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="e4f89-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-175">Boolean</span></span>|<span data-ttu-id="e4f89-176">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="e4f89-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-177">appleNewsBlocked</span></span>|<span data-ttu-id="e4f89-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-178">Boolean</span></span>|<span data-ttu-id="e4f89-179">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="e4f89-180">appsSingleAppModeList</span></span>|<span data-ttu-id="e4f89-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e4f89-182">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="e4f89-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="e4f89-183">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="e4f89-183">Supervised only.</span></span> <span data-ttu-id="e4f89-184">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="e4f89-184">iOS 7.0 and later.</span></span> <span data-ttu-id="e4f89-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e4f89-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e4f89-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="e4f89-186">appsVisibilityList</span></span>|<span data-ttu-id="e4f89-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e4f89-188">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="e4f89-189">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e4f89-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e4f89-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="e4f89-190">appsVisibilityListType</span></span>|[<span data-ttu-id="e4f89-191">appListType</span><span class="sxs-lookup"><span data-stu-id="e4f89-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e4f89-192">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="e4f89-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="e4f89-193">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="e4f89-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e4f89-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="e4f89-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="e4f89-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-195">Boolean</span></span>|<span data-ttu-id="e4f89-196">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-197">appStoreBlocked</span></span>|<span data-ttu-id="e4f89-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-198">Boolean</span></span>|<span data-ttu-id="e4f89-199">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="e4f89-199">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="e4f89-200">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-200">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-201">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="e4f89-201">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="e4f89-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-202">Boolean</span></span>|<span data-ttu-id="e4f89-203">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="e4f89-203">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="e4f89-204">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e4f89-204">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="e4f89-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-205">Boolean</span></span>|<span data-ttu-id="e4f89-206">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="e4f89-206">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="e4f89-207">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-207">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-208">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e4f89-208">appStoreRequirePassword</span></span>|<span data-ttu-id="e4f89-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-209">Boolean</span></span>|<span data-ttu-id="e4f89-210">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e4f89-210">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="e4f89-211">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-211">bluetoothBlockModification</span></span>|<span data-ttu-id="e4f89-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-212">Boolean</span></span>|<span data-ttu-id="e4f89-213">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-213">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="e4f89-214">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-214">cameraBlocked</span></span>|<span data-ttu-id="e4f89-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-215">Boolean</span></span>|<span data-ttu-id="e4f89-216">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="e4f89-216">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="e4f89-217">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-217">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="e4f89-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="e4f89-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-219">Boolean</span></span>|<span data-ttu-id="e4f89-220">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="e4f89-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="e4f89-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="e4f89-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="e4f89-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-222">Boolean</span></span>|<span data-ttu-id="e4f89-223">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="e4f89-223">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="e4f89-224">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-224">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="e4f89-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-225">Boolean</span></span>|<span data-ttu-id="e4f89-226">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-226">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-227">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="e4f89-227">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="e4f89-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-228">Boolean</span></span>|<span data-ttu-id="e4f89-229">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="e4f89-229">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="e4f89-230">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="e4f89-230">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="e4f89-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-231">Boolean</span></span>|<span data-ttu-id="e4f89-232">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="e4f89-232">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="e4f89-233">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="e4f89-233">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="e4f89-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-234">Boolean</span></span>|<span data-ttu-id="e4f89-235">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="e4f89-235">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="e4f89-236">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e4f89-236">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="e4f89-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-237">Boolean</span></span>|<span data-ttu-id="e4f89-238">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-238">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e4f89-239">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e4f89-239">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="e4f89-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-240">Boolean</span></span>|<span data-ttu-id="e4f89-241">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="e4f89-241">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-242">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e4f89-242">compliantAppsList</span></span>|<span data-ttu-id="e4f89-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e4f89-244">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-244">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e4f89-245">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e4f89-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e4f89-246">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e4f89-246">compliantAppListType</span></span>|[<span data-ttu-id="e4f89-247">appListType</span><span class="sxs-lookup"><span data-stu-id="e4f89-247">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e4f89-248">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="e4f89-248">List that is in the AppComplianceList.</span></span> <span data-ttu-id="e4f89-249">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="e4f89-249">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e4f89-250">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="e4f89-250">configurationProfileBlockChanges</span></span>|<span data-ttu-id="e4f89-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-251">Boolean</span></span>|<span data-ttu-id="e4f89-252">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="e4f89-252">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-253">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-253">definitionLookupBlocked</span></span>|<span data-ttu-id="e4f89-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-254">Boolean</span></span>|<span data-ttu-id="e4f89-255">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-255">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="e4f89-256">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="e4f89-256">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="e4f89-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-257">Boolean</span></span>|<span data-ttu-id="e4f89-258">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="e4f89-258">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-259">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-259">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="e4f89-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-260">Boolean</span></span>|<span data-ttu-id="e4f89-261">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="e4f89-261">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-262">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-262">deviceBlockNameModification</span></span>|<span data-ttu-id="e4f89-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-263">Boolean</span></span>|<span data-ttu-id="e4f89-264">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-264">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-265">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="e4f89-265">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="e4f89-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-266">Boolean</span></span>|<span data-ttu-id="e4f89-267">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="e4f89-267">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="e4f89-268">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-268">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="e4f89-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-269">Boolean</span></span>|<span data-ttu-id="e4f89-270">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-270">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="e4f89-271">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="e4f89-271">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="e4f89-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-272">Boolean</span></span>|<span data-ttu-id="e4f89-273">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="e4f89-273">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="e4f89-274">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="e4f89-274">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="e4f89-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-275">Boolean</span></span>|<span data-ttu-id="e4f89-276">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="e4f89-276">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="e4f89-277">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="e4f89-277">emailInDomainSuffixes</span></span>|<span data-ttu-id="e4f89-278">String 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-278">String collection</span></span>|<span data-ttu-id="e4f89-279">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="e4f89-279">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="e4f89-280">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="e4f89-280">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="e4f89-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-281">Boolean</span></span>|<span data-ttu-id="e4f89-282">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-282">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="e4f89-283">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-283">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="e4f89-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-284">Boolean</span></span>|<span data-ttu-id="e4f89-285">\[已弃用 \] 配置此设置，将值设置为"true"对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="e4f89-285">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="e4f89-286">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-286">faceTimeBlocked</span></span>|<span data-ttu-id="e4f89-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-287">Boolean</span></span>|<span data-ttu-id="e4f89-288">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="e4f89-288">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="e4f89-289">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-289">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-290">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-290">findMyFriendsBlocked</span></span>|<span data-ttu-id="e4f89-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-291">Boolean</span></span>|<span data-ttu-id="e4f89-292">指示设备在监督模式下时是否阻止对"查找我的好友"的更改。</span><span class="sxs-lookup"><span data-stu-id="e4f89-292">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-293">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="e4f89-293">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="e4f89-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-294">Boolean</span></span>|<span data-ttu-id="e4f89-295">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="e4f89-295">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="e4f89-296">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-296">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-297">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="e4f89-297">gamingBlockMultiplayer</span></span>|<span data-ttu-id="e4f89-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-298">Boolean</span></span>|<span data-ttu-id="e4f89-299">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="e4f89-299">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="e4f89-300">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-300">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-301">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-301">gameCenterBlocked</span></span>|<span data-ttu-id="e4f89-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-302">Boolean</span></span>|<span data-ttu-id="e4f89-303">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="e4f89-303">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-304">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-304">hostPairingBlocked</span></span>|<span data-ttu-id="e4f89-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-305">Boolean</span></span>|<span data-ttu-id="e4f89-306">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-306">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-307">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-307">iBooksStoreBlocked</span></span>|<span data-ttu-id="e4f89-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-308">Boolean</span></span>|<span data-ttu-id="e4f89-309">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="e4f89-309">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-310">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="e4f89-310">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="e4f89-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-311">Boolean</span></span>|<span data-ttu-id="e4f89-312">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="e4f89-312">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="e4f89-313">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="e4f89-313">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="e4f89-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-314">Boolean</span></span>|<span data-ttu-id="e4f89-315">指示是否阻止用户继续在 iOS 设备上启动的工作到其他 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-315">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="e4f89-316">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="e4f89-316">iCloudBlockBackup</span></span>|<span data-ttu-id="e4f89-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-317">Boolean</span></span>|<span data-ttu-id="e4f89-318">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="e4f89-318">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="e4f89-319">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-319">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-320">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="e4f89-320">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="e4f89-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-321">Boolean</span></span>|<span data-ttu-id="e4f89-322">指示是否阻止 iCloud 文档同步。需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-322">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-323">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="e4f89-323">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="e4f89-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-324">Boolean</span></span>|<span data-ttu-id="e4f89-325">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="e4f89-325">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="e4f89-326">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="e4f89-326">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="e4f89-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-327">Boolean</span></span>|<span data-ttu-id="e4f89-328">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="e4f89-328">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="e4f89-329">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="e4f89-329">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="e4f89-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-330">Boolean</span></span>|<span data-ttu-id="e4f89-331">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="e4f89-331">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="e4f89-332">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="e4f89-332">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="e4f89-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-333">Boolean</span></span>|<span data-ttu-id="e4f89-334">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="e4f89-334">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="e4f89-335">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="e4f89-335">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="e4f89-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-336">Boolean</span></span>|<span data-ttu-id="e4f89-337">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="e4f89-337">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="e4f89-338">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="e4f89-338">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="e4f89-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-339">Boolean</span></span>|<span data-ttu-id="e4f89-340">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="e4f89-340">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="e4f89-341">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-341">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-342">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="e4f89-342">iTunesBlockMusicService</span></span>|<span data-ttu-id="e4f89-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-343">Boolean</span></span>|<span data-ttu-id="e4f89-344">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-344">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e4f89-345">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="e4f89-345">iTunesBlockRadio</span></span>|<span data-ttu-id="e4f89-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-346">Boolean</span></span>|<span data-ttu-id="e4f89-347">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-347">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e4f89-348">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="e4f89-348">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="e4f89-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-349">Boolean</span></span>|<span data-ttu-id="e4f89-350">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-350">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="e4f89-351">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="e4f89-351">keyboardBlockDictation</span></span>|<span data-ttu-id="e4f89-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-352">Boolean</span></span>|<span data-ttu-id="e4f89-353">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="e4f89-353">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-354">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="e4f89-354">keyboardBlockPredictive</span></span>|<span data-ttu-id="e4f89-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-355">Boolean</span></span>|<span data-ttu-id="e4f89-356">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-356">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="e4f89-357">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="e4f89-357">keyboardBlockShortcuts</span></span>|<span data-ttu-id="e4f89-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-358">Boolean</span></span>|<span data-ttu-id="e4f89-359">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-359">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-360">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="e4f89-360">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="e4f89-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-361">Boolean</span></span>|<span data-ttu-id="e4f89-362">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-362">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="e4f89-363">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="e4f89-363">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="e4f89-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-364">Boolean</span></span>|<span data-ttu-id="e4f89-365">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="e4f89-365">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-366">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-366">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="e4f89-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-367">Boolean</span></span>|<span data-ttu-id="e4f89-368">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-368">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-369">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="e4f89-369">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="e4f89-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-370">Boolean</span></span>|<span data-ttu-id="e4f89-371">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="e4f89-371">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="e4f89-372">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-372">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="e4f89-373">请改为使用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="e4f89-373">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="e4f89-374">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-374">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="e4f89-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-375">Boolean</span></span>|<span data-ttu-id="e4f89-376">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-376">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-377">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="e4f89-377">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="e4f89-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-378">Boolean</span></span>|<span data-ttu-id="e4f89-379">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="e4f89-379">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="e4f89-380">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-380">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="e4f89-381">请改为使用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="e4f89-381">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="e4f89-382">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="e4f89-382">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="e4f89-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-383">Boolean</span></span>|<span data-ttu-id="e4f89-384">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="e4f89-384">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="e4f89-385">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-385">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="e4f89-386">请改为使用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="e4f89-386">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="e4f89-387">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="e4f89-387">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="e4f89-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-388">Boolean</span></span>|<span data-ttu-id="e4f89-389">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="e4f89-389">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="e4f89-390">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-390">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="e4f89-391">请改为使用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="e4f89-391">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="e4f89-392">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="e4f89-392">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="e4f89-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-393">Boolean</span></span>|<span data-ttu-id="e4f89-394">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="e4f89-394">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="e4f89-395">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-395">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="e4f89-396">请改为使用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="e4f89-396">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="e4f89-397">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-397">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="e4f89-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-398">Boolean</span></span>|<span data-ttu-id="e4f89-399">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-399">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-400">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="e4f89-400">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="e4f89-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-401">Boolean</span></span>|<span data-ttu-id="e4f89-402">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="e4f89-402">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="e4f89-403">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-403">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="e4f89-404">请改为使用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="e4f89-404">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="e4f89-405">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-405">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="e4f89-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-406">Boolean</span></span>|<span data-ttu-id="e4f89-407">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-407">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-408">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e4f89-408">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="e4f89-409">String</span><span class="sxs-lookup"><span data-stu-id="e4f89-409">String</span></span>|<span data-ttu-id="e4f89-410">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="e4f89-410">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="e4f89-411">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="e4f89-411">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="e4f89-412">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="e4f89-412">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="e4f89-413">String</span><span class="sxs-lookup"><span data-stu-id="e4f89-413">String</span></span>|<span data-ttu-id="e4f89-414">用于展台模式的内置应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="e4f89-414">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="e4f89-415">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-415">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="e4f89-416">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="e4f89-416">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="e4f89-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-417">Boolean</span></span>|<span data-ttu-id="e4f89-418">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="e4f89-418">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-419">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="e4f89-419">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="e4f89-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-420">Boolean</span></span>|<span data-ttu-id="e4f89-421">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="e4f89-421">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-422">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="e4f89-422">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="e4f89-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-423">Boolean</span></span>|<span data-ttu-id="e4f89-424">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="e4f89-424">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-425">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="e4f89-425">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="e4f89-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-426">Boolean</span></span>|<span data-ttu-id="e4f89-427">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="e4f89-427">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-428">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="e4f89-428">kioskModeRequireZoom</span></span>|<span data-ttu-id="e4f89-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-429">Boolean</span></span>|<span data-ttu-id="e4f89-430">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="e4f89-430">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="e4f89-431">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="e4f89-431">kioskModeManagedAppId</span></span>|<span data-ttu-id="e4f89-432">String</span><span class="sxs-lookup"><span data-stu-id="e4f89-432">String</span></span>|<span data-ttu-id="e4f89-433">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="e4f89-433">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="e4f89-434">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="e4f89-434">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="e4f89-435">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="e4f89-435">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="e4f89-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-436">Boolean</span></span>|<span data-ttu-id="e4f89-437">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="e4f89-437">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="e4f89-438">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="e4f89-438">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="e4f89-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-439">Boolean</span></span>|<span data-ttu-id="e4f89-440">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="e4f89-440">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="e4f89-441">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="e4f89-441">lockScreenBlockPassbook</span></span>|<span data-ttu-id="e4f89-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-442">Boolean</span></span>|<span data-ttu-id="e4f89-443">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="e4f89-443">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="e4f89-444">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="e4f89-444">lockScreenBlockTodayView</span></span>|<span data-ttu-id="e4f89-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-445">Boolean</span></span>|<span data-ttu-id="e4f89-446">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="e4f89-446">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="e4f89-447">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="e4f89-447">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="e4f89-448">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="e4f89-448">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="e4f89-449">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-449">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="e4f89-450">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="e4f89-450">mediaContentRatingCanada</span></span>|[<span data-ttu-id="e4f89-451">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="e4f89-451">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="e4f89-452">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-452">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="e4f89-453">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="e4f89-453">mediaContentRatingFrance</span></span>|[<span data-ttu-id="e4f89-454">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="e4f89-454">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="e4f89-455">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-455">Media content rating settings for France</span></span>|
|<span data-ttu-id="e4f89-456">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="e4f89-456">mediaContentRatingGermany</span></span>|[<span data-ttu-id="e4f89-457">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="e4f89-457">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="e4f89-458">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-458">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="e4f89-459">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e4f89-459">mediaContentRatingIreland</span></span>|[<span data-ttu-id="e4f89-460">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e4f89-460">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="e4f89-461">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-461">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="e4f89-462">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="e4f89-462">mediaContentRatingJapan</span></span>|[<span data-ttu-id="e4f89-463">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="e4f89-463">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="e4f89-464">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-464">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="e4f89-465">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="e4f89-465">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="e4f89-466">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="e4f89-466">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="e4f89-467">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-467">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="e4f89-468">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="e4f89-468">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="e4f89-469">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="e4f89-469">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="e4f89-470">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-470">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="e4f89-471">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="e4f89-471">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="e4f89-472">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="e4f89-472">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="e4f89-473">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="e4f89-473">Media content rating settings for United States</span></span>|
|<span data-ttu-id="e4f89-474">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="e4f89-474">networkUsageRules</span></span>|<span data-ttu-id="e4f89-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="e4f89-476">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="e4f89-476">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="e4f89-477">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e4f89-477">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="e4f89-478">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="e4f89-478">mediaContentRatingApps</span></span>|[<span data-ttu-id="e4f89-479">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="e4f89-479">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="e4f89-480">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-480">Media content rating settings for Apps.</span></span> <span data-ttu-id="e4f89-481">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="e4f89-481">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="e4f89-482">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-482">messagesBlocked</span></span>|<span data-ttu-id="e4f89-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-483">Boolean</span></span>|<span data-ttu-id="e4f89-484">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="e4f89-484">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="e4f89-485">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-485">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="e4f89-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-486">Boolean</span></span>|<span data-ttu-id="e4f89-487">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-487">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e4f89-488">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e4f89-488">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="e4f89-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-489">Boolean</span></span>|<span data-ttu-id="e4f89-490">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="e4f89-490">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e4f89-491">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-491">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="e4f89-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-492">Boolean</span></span>|<span data-ttu-id="e4f89-493">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="e4f89-493">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="e4f89-494">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-494">passcodeBlockModification</span></span>|<span data-ttu-id="e4f89-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-495">Boolean</span></span>|<span data-ttu-id="e4f89-496">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-496">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="e4f89-497">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e4f89-497">passcodeBlockSimple</span></span>|<span data-ttu-id="e4f89-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-498">Boolean</span></span>|<span data-ttu-id="e4f89-499">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="e4f89-499">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="e4f89-500">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e4f89-500">passcodeExpirationDays</span></span>|<span data-ttu-id="e4f89-501">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-501">Int32</span></span>|<span data-ttu-id="e4f89-502">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e4f89-502">Number of days before the passcode expires.</span></span> <span data-ttu-id="e4f89-503">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="e4f89-503">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e4f89-504">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e4f89-504">passcodeMinimumLength</span></span>|<span data-ttu-id="e4f89-505">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-505">Int32</span></span>|<span data-ttu-id="e4f89-506">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e4f89-506">Minimum length of passcode.</span></span> <span data-ttu-id="e4f89-507">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="e4f89-507">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e4f89-508">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e4f89-508">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e4f89-509">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-509">Int32</span></span>|<span data-ttu-id="e4f89-510">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="e4f89-510">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="e4f89-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e4f89-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e4f89-512">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-512">Int32</span></span>|<span data-ttu-id="e4f89-513">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="e4f89-513">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e4f89-514">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e4f89-514">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="e4f89-515">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-515">Int32</span></span>|<span data-ttu-id="e4f89-516">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e4f89-516">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="e4f89-517">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="e4f89-517">Valid values 0 to 4</span></span>|
|<span data-ttu-id="e4f89-518">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="e4f89-518">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="e4f89-519">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-519">Int32</span></span>|<span data-ttu-id="e4f89-520">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e4f89-520">Number of previous passcodes to block.</span></span> <span data-ttu-id="e4f89-521">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="e4f89-521">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e4f89-522">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="e4f89-522">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="e4f89-523">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f89-523">Int32</span></span>|<span data-ttu-id="e4f89-524">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="e4f89-524">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="e4f89-525">有效值为 2 至 11</span><span class="sxs-lookup"><span data-stu-id="e4f89-525">Valid values 2 to 11</span></span>|
|<span data-ttu-id="e4f89-526">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="e4f89-526">passcodeRequiredType</span></span>|[<span data-ttu-id="e4f89-527">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e4f89-527">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e4f89-528">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e4f89-528">Type of passcode that is required.</span></span> <span data-ttu-id="e4f89-529">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e4f89-529">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e4f89-530">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="e4f89-530">passcodeRequired</span></span>|<span data-ttu-id="e4f89-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-531">Boolean</span></span>|<span data-ttu-id="e4f89-532">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e4f89-532">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="e4f89-533">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-533">podcastsBlocked</span></span>|<span data-ttu-id="e4f89-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-534">Boolean</span></span>|<span data-ttu-id="e4f89-535">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-535">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="e4f89-536">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e4f89-536">safariBlockAutofill</span></span>|<span data-ttu-id="e4f89-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-537">Boolean</span></span>|<span data-ttu-id="e4f89-538">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="e4f89-538">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="e4f89-539">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-539">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-540">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="e4f89-540">safariBlockJavaScript</span></span>|<span data-ttu-id="e4f89-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-541">Boolean</span></span>|<span data-ttu-id="e4f89-542">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="e4f89-542">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="e4f89-543">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="e4f89-543">safariBlockPopups</span></span>|<span data-ttu-id="e4f89-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-544">Boolean</span></span>|<span data-ttu-id="e4f89-545">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="e4f89-545">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="e4f89-546">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-546">safariBlocked</span></span>|<span data-ttu-id="e4f89-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-547">Boolean</span></span>|<span data-ttu-id="e4f89-548">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="e4f89-548">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="e4f89-549">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-549">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="e4f89-550">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-550">safariCookieSettings</span></span>|[<span data-ttu-id="e4f89-551">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="e4f89-551">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="e4f89-552">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="e4f89-552">Cookie settings for Safari.</span></span> <span data-ttu-id="e4f89-553">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="e4f89-553">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="e4f89-554">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="e4f89-554">safariManagedDomains</span></span>|<span data-ttu-id="e4f89-555">String 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-555">String collection</span></span>|<span data-ttu-id="e4f89-556">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="e4f89-556">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="e4f89-557">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="e4f89-557">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="e4f89-558">String 集合</span><span class="sxs-lookup"><span data-stu-id="e4f89-558">String collection</span></span>|<span data-ttu-id="e4f89-559">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="e4f89-559">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="e4f89-560">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-560">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="e4f89-561">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="e4f89-561">safariRequireFraudWarning</span></span>|<span data-ttu-id="e4f89-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-562">Boolean</span></span>|<span data-ttu-id="e4f89-563">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="e4f89-563">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="e4f89-564">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-564">screenCaptureBlocked</span></span>|<span data-ttu-id="e4f89-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-565">Boolean</span></span>|<span data-ttu-id="e4f89-566">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="e4f89-566">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="e4f89-567">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-567">siriBlocked</span></span>|<span data-ttu-id="e4f89-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-568">Boolean</span></span>|<span data-ttu-id="e4f89-569">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="e4f89-569">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="e4f89-570">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-570">siriBlockedWhenLocked</span></span>|<span data-ttu-id="e4f89-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-571">Boolean</span></span>|<span data-ttu-id="e4f89-572">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="e4f89-572">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="e4f89-573">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="e4f89-573">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="e4f89-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-574">Boolean</span></span>|<span data-ttu-id="e4f89-575">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="e4f89-575">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="e4f89-576">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="e4f89-576">siriRequireProfanityFilter</span></span>|<span data-ttu-id="e4f89-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-577">Boolean</span></span>|<span data-ttu-id="e4f89-578">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="e4f89-578">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="e4f89-579">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="e4f89-579">spotlightBlockInternetResults</span></span>|<span data-ttu-id="e4f89-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-580">Boolean</span></span>|<span data-ttu-id="e4f89-581">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="e4f89-581">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="e4f89-582">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="e4f89-582">voiceDialingBlocked</span></span>|<span data-ttu-id="e4f89-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-583">Boolean</span></span>|<span data-ttu-id="e4f89-584">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="e4f89-584">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="e4f89-585">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="e4f89-585">wallpaperBlockModification</span></span>|<span data-ttu-id="e4f89-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-586">Boolean</span></span>|<span data-ttu-id="e4f89-587">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e4f89-587">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="e4f89-588">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="e4f89-588">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="e4f89-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f89-589">Boolean</span></span>|<span data-ttu-id="e4f89-590">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="e4f89-590">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="e4f89-591">适用于运行 iOS 和 iPadOS 版本 14.4 及更早版本的设备。</span><span class="sxs-lookup"><span data-stu-id="e4f89-591">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="e4f89-592">运行 14.5+ 的设备应该使用设置"WiFiConnectToAllowedNetworksOnlyForced"。</span><span class="sxs-lookup"><span data-stu-id="e4f89-592">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|



## <a name="response"></a><span data-ttu-id="e4f89-593">响应</span><span class="sxs-lookup"><span data-stu-id="e4f89-593">Response</span></span>
<span data-ttu-id="e4f89-594">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4f89-594">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4f89-595">示例</span><span class="sxs-lookup"><span data-stu-id="e4f89-595">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4f89-596">请求</span><span class="sxs-lookup"><span data-stu-id="e4f89-596">Request</span></span>
<span data-ttu-id="e4f89-597">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4f89-597">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="e4f89-598">响应</span><span class="sxs-lookup"><span data-stu-id="e4f89-598">Response</span></span>
<span data-ttu-id="e4f89-p143">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4f89-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




