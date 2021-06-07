---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e8649b945c6f57b1968c067798ac5141b28a089
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757078"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="f5de4-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5de4-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="f5de4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5de4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5de4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5de4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5de4-106">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5de4-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5de4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5de4-107">Prerequisites</span></span>
<span data-ttu-id="f5de4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5de4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5de4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5de4-110">Permission type</span></span>|<span data-ttu-id="f5de4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5de4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5de4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5de4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5de4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5de4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5de4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5de4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5de4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5de4-115">Not supported.</span></span>|
|<span data-ttu-id="f5de4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5de4-116">Application</span></span>|<span data-ttu-id="f5de4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5de4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5de4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5de4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5de4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5de4-119">Request headers</span></span>
|<span data-ttu-id="f5de4-120">标头</span><span class="sxs-lookup"><span data-stu-id="f5de4-120">Header</span></span>|<span data-ttu-id="f5de4-121">值</span><span class="sxs-lookup"><span data-stu-id="f5de4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5de4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5de4-122">Authorization</span></span>|<span data-ttu-id="f5de4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5de4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5de4-124">接受</span><span class="sxs-lookup"><span data-stu-id="f5de4-124">Accept</span></span>|<span data-ttu-id="f5de4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5de4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5de4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5de4-126">Request body</span></span>
<span data-ttu-id="f5de4-127">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5de4-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f5de4-128">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5de4-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f5de4-129">属性</span><span class="sxs-lookup"><span data-stu-id="f5de4-129">Property</span></span>|<span data-ttu-id="f5de4-130">类型</span><span class="sxs-lookup"><span data-stu-id="f5de4-130">Type</span></span>|<span data-ttu-id="f5de4-131">说明</span><span class="sxs-lookup"><span data-stu-id="f5de4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5de4-132">id</span><span class="sxs-lookup"><span data-stu-id="f5de4-132">id</span></span>|<span data-ttu-id="f5de4-133">String</span><span class="sxs-lookup"><span data-stu-id="f5de4-133">String</span></span>|<span data-ttu-id="f5de4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5de4-134">Key of the entity.</span></span> <span data-ttu-id="f5de4-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5de4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5de4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5de4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f5de4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5de4-137">DateTimeOffset</span></span>|<span data-ttu-id="f5de4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5de4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f5de4-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5de4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5de4-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5de4-140">createdDateTime</span></span>|<span data-ttu-id="f5de4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5de4-141">DateTimeOffset</span></span>|<span data-ttu-id="f5de4-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5de4-142">DateTime the object was created.</span></span> <span data-ttu-id="f5de4-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5de4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5de4-144">说明</span><span class="sxs-lookup"><span data-stu-id="f5de4-144">description</span></span>|<span data-ttu-id="f5de4-145">String</span><span class="sxs-lookup"><span data-stu-id="f5de4-145">String</span></span>|<span data-ttu-id="f5de4-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f5de4-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5de4-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5de4-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5de4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f5de4-148">displayName</span></span>|<span data-ttu-id="f5de4-149">String</span><span class="sxs-lookup"><span data-stu-id="f5de4-149">String</span></span>|<span data-ttu-id="f5de4-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f5de4-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5de4-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5de4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5de4-152">version</span><span class="sxs-lookup"><span data-stu-id="f5de4-152">version</span></span>|<span data-ttu-id="f5de4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-153">Int32</span></span>|<span data-ttu-id="f5de4-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f5de4-154">Version of the device configuration.</span></span> <span data-ttu-id="f5de4-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5de4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5de4-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-156">accountBlockModification</span></span>|<span data-ttu-id="f5de4-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-157">Boolean</span></span>|<span data-ttu-id="f5de4-158">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="f5de4-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="f5de4-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="f5de4-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-160">Boolean</span></span>|<span data-ttu-id="f5de4-161">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="f5de4-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="f5de4-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-162">airDropBlocked</span></span>|<span data-ttu-id="f5de4-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-163">Boolean</span></span>|<span data-ttu-id="f5de4-164">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="f5de4-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="f5de4-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="f5de4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-166">Boolean</span></span>|<span data-ttu-id="f5de4-167">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="f5de4-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="f5de4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-169">Boolean</span></span>|<span data-ttu-id="f5de4-170">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="f5de4-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="f5de4-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="f5de4-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="f5de4-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-172">Boolean</span></span>|<span data-ttu-id="f5de4-173">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="f5de4-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="f5de4-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-175">Boolean</span></span>|<span data-ttu-id="f5de4-176">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="f5de4-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-177">appleNewsBlocked</span></span>|<span data-ttu-id="f5de4-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-178">Boolean</span></span>|<span data-ttu-id="f5de4-179">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="f5de4-180">appsSingleAppModeList</span></span>|<span data-ttu-id="f5de4-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f5de4-182">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="f5de4-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="f5de4-183">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="f5de4-183">Supervised only.</span></span> <span data-ttu-id="f5de4-184">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="f5de4-184">iOS 7.0 and later.</span></span> <span data-ttu-id="f5de4-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f5de4-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f5de4-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="f5de4-186">appsVisibilityList</span></span>|<span data-ttu-id="f5de4-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f5de4-188">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="f5de4-189">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f5de4-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f5de4-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="f5de4-190">appsVisibilityListType</span></span>|[<span data-ttu-id="f5de4-191">appListType</span><span class="sxs-lookup"><span data-stu-id="f5de4-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f5de4-192">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="f5de4-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="f5de4-193">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="f5de4-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f5de4-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="f5de4-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="f5de4-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-195">Boolean</span></span>|<span data-ttu-id="f5de4-196">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-197">appStoreBlocked</span></span>|<span data-ttu-id="f5de4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-198">Boolean</span></span>|<span data-ttu-id="f5de4-199">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="f5de4-199">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="f5de4-200">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-200">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-201">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="f5de4-201">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="f5de4-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-202">Boolean</span></span>|<span data-ttu-id="f5de4-203">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="f5de4-203">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="f5de4-204">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f5de4-204">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="f5de4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-205">Boolean</span></span>|<span data-ttu-id="f5de4-206">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="f5de4-206">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="f5de4-207">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-207">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-208">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="f5de4-208">appStoreRequirePassword</span></span>|<span data-ttu-id="f5de4-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-209">Boolean</span></span>|<span data-ttu-id="f5de4-210">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="f5de4-210">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="f5de4-211">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-211">bluetoothBlockModification</span></span>|<span data-ttu-id="f5de4-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-212">Boolean</span></span>|<span data-ttu-id="f5de4-213">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-213">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="f5de4-214">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-214">cameraBlocked</span></span>|<span data-ttu-id="f5de4-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-215">Boolean</span></span>|<span data-ttu-id="f5de4-216">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="f5de4-216">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="f5de4-217">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-217">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="f5de4-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="f5de4-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-219">Boolean</span></span>|<span data-ttu-id="f5de4-220">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="f5de4-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="f5de4-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="f5de4-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="f5de4-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-222">Boolean</span></span>|<span data-ttu-id="f5de4-223">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="f5de4-223">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="f5de4-224">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-224">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="f5de4-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-225">Boolean</span></span>|<span data-ttu-id="f5de4-226">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-226">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-227">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="f5de4-227">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="f5de4-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-228">Boolean</span></span>|<span data-ttu-id="f5de4-229">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="f5de4-229">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="f5de4-230">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="f5de4-230">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="f5de4-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-231">Boolean</span></span>|<span data-ttu-id="f5de4-232">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="f5de4-232">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="f5de4-233">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="f5de4-233">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="f5de4-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-234">Boolean</span></span>|<span data-ttu-id="f5de4-235">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="f5de4-235">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="f5de4-236">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f5de4-236">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="f5de4-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-237">Boolean</span></span>|<span data-ttu-id="f5de4-238">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-238">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f5de4-239">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f5de4-239">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="f5de4-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-240">Boolean</span></span>|<span data-ttu-id="f5de4-241">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="f5de4-241">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-242">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f5de4-242">compliantAppsList</span></span>|<span data-ttu-id="f5de4-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f5de4-244">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-244">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f5de4-245">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f5de4-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f5de4-246">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f5de4-246">compliantAppListType</span></span>|[<span data-ttu-id="f5de4-247">appListType</span><span class="sxs-lookup"><span data-stu-id="f5de4-247">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f5de4-248">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="f5de4-248">List that is in the AppComplianceList.</span></span> <span data-ttu-id="f5de4-249">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="f5de4-249">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f5de4-250">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="f5de4-250">configurationProfileBlockChanges</span></span>|<span data-ttu-id="f5de4-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-251">Boolean</span></span>|<span data-ttu-id="f5de4-252">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="f5de4-252">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-253">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-253">definitionLookupBlocked</span></span>|<span data-ttu-id="f5de4-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-254">Boolean</span></span>|<span data-ttu-id="f5de4-255">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-255">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="f5de4-256">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="f5de4-256">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="f5de4-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-257">Boolean</span></span>|<span data-ttu-id="f5de4-258">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="f5de4-258">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-259">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-259">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="f5de4-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-260">Boolean</span></span>|<span data-ttu-id="f5de4-261">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="f5de4-261">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-262">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-262">deviceBlockNameModification</span></span>|<span data-ttu-id="f5de4-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-263">Boolean</span></span>|<span data-ttu-id="f5de4-264">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-264">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-265">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="f5de4-265">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="f5de4-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-266">Boolean</span></span>|<span data-ttu-id="f5de4-267">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="f5de4-267">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f5de4-268">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-268">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="f5de4-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-269">Boolean</span></span>|<span data-ttu-id="f5de4-270">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-270">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="f5de4-271">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="f5de4-271">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="f5de4-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-272">Boolean</span></span>|<span data-ttu-id="f5de4-273">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="f5de4-273">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="f5de4-274">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="f5de4-274">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="f5de4-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-275">Boolean</span></span>|<span data-ttu-id="f5de4-276">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="f5de4-276">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="f5de4-277">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f5de4-277">emailInDomainSuffixes</span></span>|<span data-ttu-id="f5de4-278">String 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-278">String collection</span></span>|<span data-ttu-id="f5de4-279">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="f5de4-279">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f5de4-280">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="f5de4-280">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="f5de4-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-281">Boolean</span></span>|<span data-ttu-id="f5de4-282">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-282">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="f5de4-283">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-283">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="f5de4-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-284">Boolean</span></span>|<span data-ttu-id="f5de4-285">\[已弃用 \] 配置此设置，将值设置为"true"对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="f5de4-285">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="f5de4-286">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-286">faceTimeBlocked</span></span>|<span data-ttu-id="f5de4-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-287">Boolean</span></span>|<span data-ttu-id="f5de4-288">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="f5de4-288">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="f5de4-289">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-289">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-290">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-290">findMyFriendsBlocked</span></span>|<span data-ttu-id="f5de4-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-291">Boolean</span></span>|<span data-ttu-id="f5de4-292">指示设备在监督模式下时是否阻止对"查找我的好友"的更改。</span><span class="sxs-lookup"><span data-stu-id="f5de4-292">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-293">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="f5de4-293">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="f5de4-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-294">Boolean</span></span>|<span data-ttu-id="f5de4-295">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="f5de4-295">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="f5de4-296">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-296">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-297">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="f5de4-297">gamingBlockMultiplayer</span></span>|<span data-ttu-id="f5de4-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-298">Boolean</span></span>|<span data-ttu-id="f5de4-299">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="f5de4-299">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="f5de4-300">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-300">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-301">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-301">gameCenterBlocked</span></span>|<span data-ttu-id="f5de4-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-302">Boolean</span></span>|<span data-ttu-id="f5de4-303">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="f5de4-303">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-304">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-304">hostPairingBlocked</span></span>|<span data-ttu-id="f5de4-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-305">Boolean</span></span>|<span data-ttu-id="f5de4-306">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-306">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-307">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-307">iBooksStoreBlocked</span></span>|<span data-ttu-id="f5de4-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-308">Boolean</span></span>|<span data-ttu-id="f5de4-309">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="f5de4-309">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-310">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="f5de4-310">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="f5de4-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-311">Boolean</span></span>|<span data-ttu-id="f5de4-312">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="f5de4-312">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="f5de4-313">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="f5de4-313">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="f5de4-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-314">Boolean</span></span>|<span data-ttu-id="f5de4-315">指示是否阻止用户继续在 iOS 设备上启动的工作到其他 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-315">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="f5de4-316">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="f5de4-316">iCloudBlockBackup</span></span>|<span data-ttu-id="f5de4-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-317">Boolean</span></span>|<span data-ttu-id="f5de4-318">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="f5de4-318">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="f5de4-319">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-319">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-320">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="f5de4-320">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="f5de4-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-321">Boolean</span></span>|<span data-ttu-id="f5de4-322">指示是否阻止 iCloud 文档同步。需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-322">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-323">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="f5de4-323">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="f5de4-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-324">Boolean</span></span>|<span data-ttu-id="f5de4-325">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="f5de4-325">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="f5de4-326">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="f5de4-326">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="f5de4-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-327">Boolean</span></span>|<span data-ttu-id="f5de4-328">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="f5de4-328">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="f5de4-329">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="f5de4-329">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="f5de4-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-330">Boolean</span></span>|<span data-ttu-id="f5de4-331">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="f5de4-331">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="f5de4-332">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="f5de4-332">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="f5de4-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-333">Boolean</span></span>|<span data-ttu-id="f5de4-334">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="f5de4-334">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="f5de4-335">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="f5de4-335">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="f5de4-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-336">Boolean</span></span>|<span data-ttu-id="f5de4-337">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="f5de4-337">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="f5de4-338">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="f5de4-338">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="f5de4-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-339">Boolean</span></span>|<span data-ttu-id="f5de4-340">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="f5de4-340">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="f5de4-341">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-341">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-342">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="f5de4-342">iTunesBlockMusicService</span></span>|<span data-ttu-id="f5de4-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-343">Boolean</span></span>|<span data-ttu-id="f5de4-344">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-344">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f5de4-345">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="f5de4-345">iTunesBlockRadio</span></span>|<span data-ttu-id="f5de4-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-346">Boolean</span></span>|<span data-ttu-id="f5de4-347">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-347">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f5de4-348">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="f5de4-348">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="f5de4-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-349">Boolean</span></span>|<span data-ttu-id="f5de4-350">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-350">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f5de4-351">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="f5de4-351">keyboardBlockDictation</span></span>|<span data-ttu-id="f5de4-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-352">Boolean</span></span>|<span data-ttu-id="f5de4-353">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="f5de4-353">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-354">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="f5de4-354">keyboardBlockPredictive</span></span>|<span data-ttu-id="f5de4-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-355">Boolean</span></span>|<span data-ttu-id="f5de4-356">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-356">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f5de4-357">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="f5de4-357">keyboardBlockShortcuts</span></span>|<span data-ttu-id="f5de4-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-358">Boolean</span></span>|<span data-ttu-id="f5de4-359">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-359">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-360">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="f5de4-360">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="f5de4-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-361">Boolean</span></span>|<span data-ttu-id="f5de4-362">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-362">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f5de4-363">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="f5de4-363">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="f5de4-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-364">Boolean</span></span>|<span data-ttu-id="f5de4-365">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="f5de4-365">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-366">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-366">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="f5de4-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-367">Boolean</span></span>|<span data-ttu-id="f5de4-368">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-368">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-369">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="f5de4-369">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="f5de4-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-370">Boolean</span></span>|<span data-ttu-id="f5de4-371">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="f5de4-371">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="f5de4-372">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-372">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="f5de4-373">请改为使用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="f5de4-373">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="f5de4-374">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-374">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="f5de4-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-375">Boolean</span></span>|<span data-ttu-id="f5de4-376">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-376">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-377">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="f5de4-377">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="f5de4-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-378">Boolean</span></span>|<span data-ttu-id="f5de4-379">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="f5de4-379">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="f5de4-380">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-380">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="f5de4-381">请改为使用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="f5de4-381">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="f5de4-382">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="f5de4-382">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="f5de4-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-383">Boolean</span></span>|<span data-ttu-id="f5de4-384">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="f5de4-384">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="f5de4-385">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-385">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="f5de4-386">请改为使用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="f5de4-386">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="f5de4-387">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="f5de4-387">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="f5de4-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-388">Boolean</span></span>|<span data-ttu-id="f5de4-389">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="f5de4-389">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="f5de4-390">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-390">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="f5de4-391">请改为使用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="f5de4-391">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="f5de4-392">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="f5de4-392">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="f5de4-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-393">Boolean</span></span>|<span data-ttu-id="f5de4-394">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="f5de4-394">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="f5de4-395">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-395">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="f5de4-396">请改为使用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="f5de4-396">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="f5de4-397">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-397">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="f5de4-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-398">Boolean</span></span>|<span data-ttu-id="f5de4-399">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-399">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-400">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="f5de4-400">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="f5de4-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-401">Boolean</span></span>|<span data-ttu-id="f5de4-402">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="f5de4-402">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="f5de4-403">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-403">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="f5de4-404">请改为使用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="f5de4-404">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="f5de4-405">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-405">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="f5de4-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-406">Boolean</span></span>|<span data-ttu-id="f5de4-407">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-407">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-408">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f5de4-408">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="f5de4-409">String</span><span class="sxs-lookup"><span data-stu-id="f5de4-409">String</span></span>|<span data-ttu-id="f5de4-410">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="f5de4-410">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="f5de4-411">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="f5de4-411">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="f5de4-412">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="f5de4-412">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="f5de4-413">String</span><span class="sxs-lookup"><span data-stu-id="f5de4-413">String</span></span>|<span data-ttu-id="f5de4-414">用于展台模式的内置应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="f5de4-414">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="f5de4-415">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-415">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="f5de4-416">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="f5de4-416">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="f5de4-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-417">Boolean</span></span>|<span data-ttu-id="f5de4-418">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="f5de4-418">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-419">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="f5de4-419">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="f5de4-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-420">Boolean</span></span>|<span data-ttu-id="f5de4-421">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="f5de4-421">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-422">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="f5de4-422">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="f5de4-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-423">Boolean</span></span>|<span data-ttu-id="f5de4-424">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="f5de4-424">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-425">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="f5de4-425">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="f5de4-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-426">Boolean</span></span>|<span data-ttu-id="f5de4-427">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="f5de4-427">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-428">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="f5de4-428">kioskModeRequireZoom</span></span>|<span data-ttu-id="f5de4-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-429">Boolean</span></span>|<span data-ttu-id="f5de4-430">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="f5de4-430">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="f5de4-431">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="f5de4-431">kioskModeManagedAppId</span></span>|<span data-ttu-id="f5de4-432">String</span><span class="sxs-lookup"><span data-stu-id="f5de4-432">String</span></span>|<span data-ttu-id="f5de4-433">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="f5de4-433">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="f5de4-434">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="f5de4-434">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="f5de4-435">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="f5de4-435">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="f5de4-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-436">Boolean</span></span>|<span data-ttu-id="f5de4-437">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="f5de4-437">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="f5de4-438">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="f5de4-438">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="f5de4-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-439">Boolean</span></span>|<span data-ttu-id="f5de4-440">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="f5de4-440">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="f5de4-441">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="f5de4-441">lockScreenBlockPassbook</span></span>|<span data-ttu-id="f5de4-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-442">Boolean</span></span>|<span data-ttu-id="f5de4-443">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="f5de4-443">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="f5de4-444">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="f5de4-444">lockScreenBlockTodayView</span></span>|<span data-ttu-id="f5de4-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-445">Boolean</span></span>|<span data-ttu-id="f5de4-446">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="f5de4-446">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="f5de4-447">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f5de4-447">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="f5de4-448">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f5de4-448">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="f5de4-449">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-449">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="f5de4-450">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f5de4-450">mediaContentRatingCanada</span></span>|[<span data-ttu-id="f5de4-451">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f5de4-451">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="f5de4-452">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-452">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="f5de4-453">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f5de4-453">mediaContentRatingFrance</span></span>|[<span data-ttu-id="f5de4-454">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f5de4-454">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="f5de4-455">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-455">Media content rating settings for France</span></span>|
|<span data-ttu-id="f5de4-456">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f5de4-456">mediaContentRatingGermany</span></span>|[<span data-ttu-id="f5de4-457">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f5de4-457">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="f5de4-458">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-458">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="f5de4-459">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="f5de4-459">mediaContentRatingIreland</span></span>|[<span data-ttu-id="f5de4-460">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="f5de4-460">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="f5de4-461">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-461">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="f5de4-462">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f5de4-462">mediaContentRatingJapan</span></span>|[<span data-ttu-id="f5de4-463">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f5de4-463">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="f5de4-464">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-464">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="f5de4-465">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f5de4-465">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="f5de4-466">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f5de4-466">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="f5de4-467">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-467">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="f5de4-468">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f5de4-468">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="f5de4-469">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f5de4-469">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="f5de4-470">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-470">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="f5de4-471">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f5de4-471">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="f5de4-472">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f5de4-472">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="f5de4-473">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="f5de4-473">Media content rating settings for United States</span></span>|
|<span data-ttu-id="f5de4-474">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="f5de4-474">networkUsageRules</span></span>|<span data-ttu-id="f5de4-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="f5de4-476">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="f5de4-476">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="f5de4-477">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f5de4-477">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f5de4-478">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="f5de4-478">mediaContentRatingApps</span></span>|[<span data-ttu-id="f5de4-479">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="f5de4-479">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="f5de4-480">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-480">Media content rating settings for Apps.</span></span> <span data-ttu-id="f5de4-481">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="f5de4-481">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="f5de4-482">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-482">messagesBlocked</span></span>|<span data-ttu-id="f5de4-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-483">Boolean</span></span>|<span data-ttu-id="f5de4-484">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="f5de4-484">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="f5de4-485">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-485">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="f5de4-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-486">Boolean</span></span>|<span data-ttu-id="f5de4-487">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-487">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f5de4-488">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f5de4-488">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="f5de4-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-489">Boolean</span></span>|<span data-ttu-id="f5de4-490">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="f5de4-490">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f5de4-491">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-491">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="f5de4-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-492">Boolean</span></span>|<span data-ttu-id="f5de4-493">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="f5de4-493">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="f5de4-494">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-494">passcodeBlockModification</span></span>|<span data-ttu-id="f5de4-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-495">Boolean</span></span>|<span data-ttu-id="f5de4-496">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-496">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f5de4-497">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f5de4-497">passcodeBlockSimple</span></span>|<span data-ttu-id="f5de4-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-498">Boolean</span></span>|<span data-ttu-id="f5de4-499">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="f5de4-499">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="f5de4-500">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f5de4-500">passcodeExpirationDays</span></span>|<span data-ttu-id="f5de4-501">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-501">Int32</span></span>|<span data-ttu-id="f5de4-502">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="f5de4-502">Number of days before the passcode expires.</span></span> <span data-ttu-id="f5de4-503">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="f5de4-503">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f5de4-504">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f5de4-504">passcodeMinimumLength</span></span>|<span data-ttu-id="f5de4-505">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-505">Int32</span></span>|<span data-ttu-id="f5de4-506">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="f5de4-506">Minimum length of passcode.</span></span> <span data-ttu-id="f5de4-507">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="f5de4-507">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f5de4-508">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f5de4-508">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f5de4-509">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-509">Int32</span></span>|<span data-ttu-id="f5de4-510">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="f5de4-510">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="f5de4-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f5de4-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f5de4-512">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-512">Int32</span></span>|<span data-ttu-id="f5de4-513">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="f5de4-513">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f5de4-514">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f5de4-514">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="f5de4-515">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-515">Int32</span></span>|<span data-ttu-id="f5de4-516">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f5de4-516">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="f5de4-517">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="f5de4-517">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f5de4-518">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="f5de4-518">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="f5de4-519">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-519">Int32</span></span>|<span data-ttu-id="f5de4-520">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f5de4-520">Number of previous passcodes to block.</span></span> <span data-ttu-id="f5de4-521">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="f5de4-521">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f5de4-522">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="f5de4-522">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="f5de4-523">Int32</span><span class="sxs-lookup"><span data-stu-id="f5de4-523">Int32</span></span>|<span data-ttu-id="f5de4-524">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="f5de4-524">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="f5de4-525">有效值为 2 至 11</span><span class="sxs-lookup"><span data-stu-id="f5de4-525">Valid values 2 to 11</span></span>|
|<span data-ttu-id="f5de4-526">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="f5de4-526">passcodeRequiredType</span></span>|[<span data-ttu-id="f5de4-527">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f5de4-527">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f5de4-528">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f5de4-528">Type of passcode that is required.</span></span> <span data-ttu-id="f5de4-529">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f5de4-529">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f5de4-530">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="f5de4-530">passcodeRequired</span></span>|<span data-ttu-id="f5de4-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-531">Boolean</span></span>|<span data-ttu-id="f5de4-532">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="f5de4-532">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="f5de4-533">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-533">podcastsBlocked</span></span>|<span data-ttu-id="f5de4-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-534">Boolean</span></span>|<span data-ttu-id="f5de4-535">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-535">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="f5de4-536">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f5de4-536">safariBlockAutofill</span></span>|<span data-ttu-id="f5de4-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-537">Boolean</span></span>|<span data-ttu-id="f5de4-538">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="f5de4-538">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="f5de4-539">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-539">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-540">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="f5de4-540">safariBlockJavaScript</span></span>|<span data-ttu-id="f5de4-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-541">Boolean</span></span>|<span data-ttu-id="f5de4-542">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="f5de4-542">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="f5de4-543">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="f5de4-543">safariBlockPopups</span></span>|<span data-ttu-id="f5de4-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-544">Boolean</span></span>|<span data-ttu-id="f5de4-545">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="f5de4-545">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="f5de4-546">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-546">safariBlocked</span></span>|<span data-ttu-id="f5de4-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-547">Boolean</span></span>|<span data-ttu-id="f5de4-548">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="f5de4-548">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="f5de4-549">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-549">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="f5de4-550">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-550">safariCookieSettings</span></span>|[<span data-ttu-id="f5de4-551">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="f5de4-551">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="f5de4-552">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="f5de4-552">Cookie settings for Safari.</span></span> <span data-ttu-id="f5de4-553">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="f5de4-553">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="f5de4-554">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="f5de4-554">safariManagedDomains</span></span>|<span data-ttu-id="f5de4-555">String 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-555">String collection</span></span>|<span data-ttu-id="f5de4-556">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="f5de4-556">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="f5de4-557">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="f5de4-557">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="f5de4-558">String 集合</span><span class="sxs-lookup"><span data-stu-id="f5de4-558">String collection</span></span>|<span data-ttu-id="f5de4-559">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="f5de4-559">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="f5de4-560">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-560">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f5de4-561">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="f5de4-561">safariRequireFraudWarning</span></span>|<span data-ttu-id="f5de4-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-562">Boolean</span></span>|<span data-ttu-id="f5de4-563">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="f5de4-563">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="f5de4-564">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-564">screenCaptureBlocked</span></span>|<span data-ttu-id="f5de4-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-565">Boolean</span></span>|<span data-ttu-id="f5de4-566">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="f5de4-566">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="f5de4-567">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-567">siriBlocked</span></span>|<span data-ttu-id="f5de4-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-568">Boolean</span></span>|<span data-ttu-id="f5de4-569">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="f5de4-569">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="f5de4-570">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-570">siriBlockedWhenLocked</span></span>|<span data-ttu-id="f5de4-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-571">Boolean</span></span>|<span data-ttu-id="f5de4-572">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="f5de4-572">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="f5de4-573">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="f5de4-573">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="f5de4-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-574">Boolean</span></span>|<span data-ttu-id="f5de4-575">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="f5de4-575">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="f5de4-576">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="f5de4-576">siriRequireProfanityFilter</span></span>|<span data-ttu-id="f5de4-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-577">Boolean</span></span>|<span data-ttu-id="f5de4-578">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="f5de4-578">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="f5de4-579">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="f5de4-579">spotlightBlockInternetResults</span></span>|<span data-ttu-id="f5de4-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-580">Boolean</span></span>|<span data-ttu-id="f5de4-581">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="f5de4-581">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="f5de4-582">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="f5de4-582">voiceDialingBlocked</span></span>|<span data-ttu-id="f5de4-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-583">Boolean</span></span>|<span data-ttu-id="f5de4-584">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="f5de4-584">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="f5de4-585">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="f5de4-585">wallpaperBlockModification</span></span>|<span data-ttu-id="f5de4-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-586">Boolean</span></span>|<span data-ttu-id="f5de4-587">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="f5de4-587">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="f5de4-588">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="f5de4-588">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="f5de4-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5de4-589">Boolean</span></span>|<span data-ttu-id="f5de4-590">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="f5de4-590">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="f5de4-591">适用于运行 iOS 和 iPadOS 版本 14.4 及更早版本的设备。</span><span class="sxs-lookup"><span data-stu-id="f5de4-591">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="f5de4-592">运行 14.5+ 的设备应该使用设置"WiFiConnectToAllowedNetworksOnlyForced"。</span><span class="sxs-lookup"><span data-stu-id="f5de4-592">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|



## <a name="response"></a><span data-ttu-id="f5de4-593">响应</span><span class="sxs-lookup"><span data-stu-id="f5de4-593">Response</span></span>
<span data-ttu-id="f5de4-594">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5de4-594">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5de4-595">示例</span><span class="sxs-lookup"><span data-stu-id="f5de4-595">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5de4-596">请求</span><span class="sxs-lookup"><span data-stu-id="f5de4-596">Request</span></span>
<span data-ttu-id="f5de4-597">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5de4-597">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5de4-598">响应</span><span class="sxs-lookup"><span data-stu-id="f5de4-598">Response</span></span>
<span data-ttu-id="f5de4-p143">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5de4-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




