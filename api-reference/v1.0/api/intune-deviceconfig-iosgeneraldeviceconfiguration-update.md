---
title: 更新 iosGeneralDeviceConfiguration
description: 更新 iosGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d20c3e80092f11639495dcad5c393db2b0bd4bb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947272"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="a7cbf-103">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7cbf-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a7cbf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7cbf-105">更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-105">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7cbf-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7cbf-106">Prerequisites</span></span>
<span data-ttu-id="a7cbf-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a7cbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7cbf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7cbf-109">Permission type</span></span>|<span data-ttu-id="a7cbf-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7cbf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7cbf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7cbf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7cbf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7cbf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7cbf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7cbf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7cbf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-114">Not supported.</span></span>|
|<span data-ttu-id="a7cbf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7cbf-115">Application</span></span>|<span data-ttu-id="a7cbf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7cbf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7cbf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7cbf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7cbf-118">Request headers</span></span>
|<span data-ttu-id="a7cbf-119">标头</span><span class="sxs-lookup"><span data-stu-id="a7cbf-119">Header</span></span>|<span data-ttu-id="a7cbf-120">值</span><span class="sxs-lookup"><span data-stu-id="a7cbf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7cbf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7cbf-121">Authorization</span></span>|<span data-ttu-id="a7cbf-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7cbf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a7cbf-123">Accept</span></span>|<span data-ttu-id="a7cbf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7cbf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7cbf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7cbf-125">Request body</span></span>
<span data-ttu-id="a7cbf-126">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-126">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a7cbf-127">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-127">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="a7cbf-128">属性</span><span class="sxs-lookup"><span data-stu-id="a7cbf-128">Property</span></span>|<span data-ttu-id="a7cbf-129">类型</span><span class="sxs-lookup"><span data-stu-id="a7cbf-129">Type</span></span>|<span data-ttu-id="a7cbf-130">说明</span><span class="sxs-lookup"><span data-stu-id="a7cbf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7cbf-131">id</span><span class="sxs-lookup"><span data-stu-id="a7cbf-131">id</span></span>|<span data-ttu-id="a7cbf-132">String</span><span class="sxs-lookup"><span data-stu-id="a7cbf-132">String</span></span>|<span data-ttu-id="a7cbf-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-133">Key of the entity.</span></span> <span data-ttu-id="a7cbf-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7cbf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7cbf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7cbf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a7cbf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7cbf-136">DateTimeOffset</span></span>|<span data-ttu-id="a7cbf-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a7cbf-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7cbf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7cbf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7cbf-139">createdDateTime</span></span>|<span data-ttu-id="a7cbf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7cbf-140">DateTimeOffset</span></span>|<span data-ttu-id="a7cbf-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-141">DateTime the object was created.</span></span> <span data-ttu-id="a7cbf-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7cbf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7cbf-143">description</span><span class="sxs-lookup"><span data-stu-id="a7cbf-143">description</span></span>|<span data-ttu-id="a7cbf-144">String</span><span class="sxs-lookup"><span data-stu-id="a7cbf-144">String</span></span>|<span data-ttu-id="a7cbf-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7cbf-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7cbf-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7cbf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a7cbf-147">displayName</span></span>|<span data-ttu-id="a7cbf-148">String</span><span class="sxs-lookup"><span data-stu-id="a7cbf-148">String</span></span>|<span data-ttu-id="a7cbf-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7cbf-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7cbf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7cbf-151">version</span><span class="sxs-lookup"><span data-stu-id="a7cbf-151">version</span></span>|<span data-ttu-id="a7cbf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-152">Int32</span></span>|<span data-ttu-id="a7cbf-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-153">Version of the device configuration.</span></span> <span data-ttu-id="a7cbf-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7cbf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7cbf-155">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-155">accountBlockModification</span></span>|<span data-ttu-id="a7cbf-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-156">Boolean</span></span>|<span data-ttu-id="a7cbf-157">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-157">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-158">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="a7cbf-158">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="a7cbf-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-159">Boolean</span></span>|<span data-ttu-id="a7cbf-160">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-160">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-161">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-161">airDropBlocked</span></span>|<span data-ttu-id="a7cbf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-162">Boolean</span></span>|<span data-ttu-id="a7cbf-163">指示设备处于监督模式时是否允许使用 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-163">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-164">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="a7cbf-164">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="a7cbf-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-165">Boolean</span></span>|<span data-ttu-id="a7cbf-166">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-166">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-167">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="a7cbf-167">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="a7cbf-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-168">Boolean</span></span>|<span data-ttu-id="a7cbf-169">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-169">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="a7cbf-170">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="a7cbf-170">appleWatchBlockPairing</span></span>|<span data-ttu-id="a7cbf-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-171">Boolean</span></span>|<span data-ttu-id="a7cbf-172">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-172">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-173">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="a7cbf-173">appleWatchForceWristDetection</span></span>|<span data-ttu-id="a7cbf-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-174">Boolean</span></span>|<span data-ttu-id="a7cbf-175">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-175">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="a7cbf-176">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-176">appleNewsBlocked</span></span>|<span data-ttu-id="a7cbf-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-177">Boolean</span></span>|<span data-ttu-id="a7cbf-178">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-178">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-179">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="a7cbf-179">appsSingleAppModeList</span></span>|<span data-ttu-id="a7cbf-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a7cbf-181">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-181">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="a7cbf-182">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-182">Supervised only.</span></span> <span data-ttu-id="a7cbf-183">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-183">iOS 7.0 and later.</span></span> <span data-ttu-id="a7cbf-184">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a7cbf-185">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="a7cbf-185">appsVisibilityList</span></span>|<span data-ttu-id="a7cbf-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a7cbf-187">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-187">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="a7cbf-188">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a7cbf-189">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-189">appsVisibilityListType</span></span>|[<span data-ttu-id="a7cbf-190">appListType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="a7cbf-191">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-191">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="a7cbf-192">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a7cbf-193">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="a7cbf-193">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="a7cbf-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-194">Boolean</span></span>|<span data-ttu-id="a7cbf-195">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-195">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-196">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-196">appStoreBlocked</span></span>|<span data-ttu-id="a7cbf-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-197">Boolean</span></span>|<span data-ttu-id="a7cbf-198">指示是否阻止用户使用应用商店。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-198">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="a7cbf-199">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="a7cbf-199">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="a7cbf-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-200">Boolean</span></span>|<span data-ttu-id="a7cbf-201">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-201">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="a7cbf-202">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a7cbf-202">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="a7cbf-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-203">Boolean</span></span>|<span data-ttu-id="a7cbf-204">指示是否阻止应用商店应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-204">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="a7cbf-205">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-205">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-206">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a7cbf-206">appStoreRequirePassword</span></span>|<span data-ttu-id="a7cbf-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-207">Boolean</span></span>|<span data-ttu-id="a7cbf-208">指示使用应用商店时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-208">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="a7cbf-209">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-209">bluetoothBlockModification</span></span>|<span data-ttu-id="a7cbf-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-210">Boolean</span></span>|<span data-ttu-id="a7cbf-211">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-211">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-212">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-212">cameraBlocked</span></span>|<span data-ttu-id="a7cbf-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-213">Boolean</span></span>|<span data-ttu-id="a7cbf-214">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-214">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="a7cbf-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="a7cbf-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="a7cbf-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-216">Boolean</span></span>|<span data-ttu-id="a7cbf-217">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="a7cbf-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="a7cbf-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="a7cbf-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-219">Boolean</span></span>|<span data-ttu-id="a7cbf-220">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-220">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="a7cbf-221">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-221">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="a7cbf-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-222">Boolean</span></span>|<span data-ttu-id="a7cbf-223">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-223">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-224">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="a7cbf-224">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="a7cbf-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-225">Boolean</span></span>|<span data-ttu-id="a7cbf-226">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-226">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="a7cbf-227">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="a7cbf-227">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="a7cbf-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-228">Boolean</span></span>|<span data-ttu-id="a7cbf-229">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-229">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="a7cbf-230">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="a7cbf-230">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="a7cbf-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-231">Boolean</span></span>|<span data-ttu-id="a7cbf-232">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-232">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="a7cbf-233">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="a7cbf-233">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="a7cbf-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-234">Boolean</span></span>|<span data-ttu-id="a7cbf-235">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-235">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-236">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="a7cbf-236">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="a7cbf-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-237">Boolean</span></span>|<span data-ttu-id="a7cbf-238">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-238">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-239">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="a7cbf-239">compliantAppsList</span></span>|<span data-ttu-id="a7cbf-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a7cbf-241">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-241">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="a7cbf-242">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a7cbf-243">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-243">compliantAppListType</span></span>|[<span data-ttu-id="a7cbf-244">appListType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-244">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="a7cbf-245">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-245">List that is in the AppComplianceList.</span></span> <span data-ttu-id="a7cbf-246">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-246">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a7cbf-247">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="a7cbf-247">configurationProfileBlockChanges</span></span>|<span data-ttu-id="a7cbf-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-248">Boolean</span></span>|<span data-ttu-id="a7cbf-249">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-249">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-250">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-250">definitionLookupBlocked</span></span>|<span data-ttu-id="a7cbf-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-251">Boolean</span></span>|<span data-ttu-id="a7cbf-252">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-252">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="a7cbf-253">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="a7cbf-253">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="a7cbf-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-254">Boolean</span></span>|<span data-ttu-id="a7cbf-255">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-255">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-256">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-256">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="a7cbf-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-257">Boolean</span></span>|<span data-ttu-id="a7cbf-258">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-258">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-259">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-259">deviceBlockNameModification</span></span>|<span data-ttu-id="a7cbf-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-260">Boolean</span></span>|<span data-ttu-id="a7cbf-261">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-261">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-262">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="a7cbf-262">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="a7cbf-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-263">Boolean</span></span>|<span data-ttu-id="a7cbf-264">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-264">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="a7cbf-265">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-265">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="a7cbf-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-266">Boolean</span></span>|<span data-ttu-id="a7cbf-267">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-267">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="a7cbf-268">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="a7cbf-268">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="a7cbf-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-269">Boolean</span></span>|<span data-ttu-id="a7cbf-270">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-270">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="a7cbf-271">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="a7cbf-271">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="a7cbf-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-272">Boolean</span></span>|<span data-ttu-id="a7cbf-273">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-273">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="a7cbf-274">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="a7cbf-274">emailInDomainSuffixes</span></span>|<span data-ttu-id="a7cbf-275">String 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-275">String collection</span></span>|<span data-ttu-id="a7cbf-276">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-276">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="a7cbf-277">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="a7cbf-277">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="a7cbf-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-278">Boolean</span></span>|<span data-ttu-id="a7cbf-279">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-279">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="a7cbf-280">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-280">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="a7cbf-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-281">Boolean</span></span>|<span data-ttu-id="a7cbf-282">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-282">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="a7cbf-283">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-283">faceTimeBlocked</span></span>|<span data-ttu-id="a7cbf-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-284">Boolean</span></span>|<span data-ttu-id="a7cbf-285">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-285">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="a7cbf-286">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-286">findMyFriendsBlocked</span></span>|<span data-ttu-id="a7cbf-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-287">Boolean</span></span>|<span data-ttu-id="a7cbf-288">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-288">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-289">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="a7cbf-289">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="a7cbf-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-290">Boolean</span></span>|<span data-ttu-id="a7cbf-291">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-291">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="a7cbf-292">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="a7cbf-292">gamingBlockMultiplayer</span></span>|<span data-ttu-id="a7cbf-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-293">Boolean</span></span>|<span data-ttu-id="a7cbf-294">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-294">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="a7cbf-295">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-295">gameCenterBlocked</span></span>|<span data-ttu-id="a7cbf-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-296">Boolean</span></span>|<span data-ttu-id="a7cbf-297">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-297">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-298">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-298">hostPairingBlocked</span></span>|<span data-ttu-id="a7cbf-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-299">Boolean</span></span>|<span data-ttu-id="a7cbf-300">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-300">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-301">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-301">iBooksStoreBlocked</span></span>|<span data-ttu-id="a7cbf-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-302">Boolean</span></span>|<span data-ttu-id="a7cbf-303">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-303">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-304">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="a7cbf-304">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="a7cbf-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-305">Boolean</span></span>|<span data-ttu-id="a7cbf-306">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-306">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="a7cbf-307">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="a7cbf-307">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="a7cbf-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-308">Boolean</span></span>|<span data-ttu-id="a7cbf-309">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-309">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="a7cbf-310">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="a7cbf-310">iCloudBlockBackup</span></span>|<span data-ttu-id="a7cbf-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-311">Boolean</span></span>|<span data-ttu-id="a7cbf-312">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-312">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="a7cbf-313">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="a7cbf-313">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="a7cbf-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-314">Boolean</span></span>|<span data-ttu-id="a7cbf-315">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-315">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="a7cbf-316">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="a7cbf-316">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="a7cbf-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-317">Boolean</span></span>|<span data-ttu-id="a7cbf-318">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-318">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="a7cbf-319">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="a7cbf-319">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="a7cbf-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-320">Boolean</span></span>|<span data-ttu-id="a7cbf-321">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-321">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="a7cbf-322">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="a7cbf-322">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="a7cbf-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-323">Boolean</span></span>|<span data-ttu-id="a7cbf-324">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-324">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="a7cbf-325">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="a7cbf-325">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="a7cbf-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-326">Boolean</span></span>|<span data-ttu-id="a7cbf-327">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-327">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="a7cbf-328">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="a7cbf-328">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="a7cbf-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-329">Boolean</span></span>|<span data-ttu-id="a7cbf-330">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-330">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="a7cbf-331">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="a7cbf-331">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="a7cbf-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-332">Boolean</span></span>|<span data-ttu-id="a7cbf-333">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-333">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="a7cbf-334">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="a7cbf-334">iTunesBlockMusicService</span></span>|<span data-ttu-id="a7cbf-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-335">Boolean</span></span>|<span data-ttu-id="a7cbf-336">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-336">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="a7cbf-337">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="a7cbf-337">iTunesBlockRadio</span></span>|<span data-ttu-id="a7cbf-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-338">Boolean</span></span>|<span data-ttu-id="a7cbf-339">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-339">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-340">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="a7cbf-340">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="a7cbf-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-341">Boolean</span></span>|<span data-ttu-id="a7cbf-342">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-342">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-343">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="a7cbf-343">keyboardBlockDictation</span></span>|<span data-ttu-id="a7cbf-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-344">Boolean</span></span>|<span data-ttu-id="a7cbf-345">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-345">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-346">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="a7cbf-346">keyboardBlockPredictive</span></span>|<span data-ttu-id="a7cbf-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-347">Boolean</span></span>|<span data-ttu-id="a7cbf-348">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-348">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-349">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="a7cbf-349">keyboardBlockShortcuts</span></span>|<span data-ttu-id="a7cbf-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-350">Boolean</span></span>|<span data-ttu-id="a7cbf-351">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-351">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-352">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="a7cbf-352">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="a7cbf-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-353">Boolean</span></span>|<span data-ttu-id="a7cbf-354">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-354">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-355">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="a7cbf-355">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="a7cbf-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-356">Boolean</span></span>|<span data-ttu-id="a7cbf-357">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-357">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-358">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-358">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="a7cbf-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-359">Boolean</span></span>|<span data-ttu-id="a7cbf-360">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-360">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-361">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="a7cbf-361">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="a7cbf-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-362">Boolean</span></span>|<span data-ttu-id="a7cbf-363">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-363">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-364">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-364">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="a7cbf-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-365">Boolean</span></span>|<span data-ttu-id="a7cbf-366">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-366">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-367">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="a7cbf-367">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="a7cbf-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-368">Boolean</span></span>|<span data-ttu-id="a7cbf-369">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-369">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-370">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="a7cbf-370">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="a7cbf-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-371">Boolean</span></span>|<span data-ttu-id="a7cbf-372">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-372">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-373">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="a7cbf-373">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="a7cbf-374">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-374">Boolean</span></span>|<span data-ttu-id="a7cbf-375">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-375">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-376">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="a7cbf-376">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="a7cbf-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-377">Boolean</span></span>|<span data-ttu-id="a7cbf-378">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-378">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-379">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-379">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="a7cbf-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-380">Boolean</span></span>|<span data-ttu-id="a7cbf-381">指示在展台模式下是否允许访问语音过滤设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-381">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-382">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="a7cbf-382">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="a7cbf-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-383">Boolean</span></span>|<span data-ttu-id="a7cbf-384">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-384">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-385">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-385">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="a7cbf-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-386">Boolean</span></span>|<span data-ttu-id="a7cbf-387">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-387">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-388">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a7cbf-388">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="a7cbf-389">String</span><span class="sxs-lookup"><span data-stu-id="a7cbf-389">String</span></span>|<span data-ttu-id="a7cbf-390">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-390">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="a7cbf-391">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-391">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="a7cbf-392">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="a7cbf-392">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="a7cbf-393">字符串</span><span class="sxs-lookup"><span data-stu-id="a7cbf-393">String</span></span>|<span data-ttu-id="a7cbf-394">用于展台模式内置应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-394">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="a7cbf-395">未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-395">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="a7cbf-396">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="a7cbf-396">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="a7cbf-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-397">Boolean</span></span>|<span data-ttu-id="a7cbf-398">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-398">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-399">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="a7cbf-399">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="a7cbf-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-400">Boolean</span></span>|<span data-ttu-id="a7cbf-401">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-401">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-402">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="a7cbf-402">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="a7cbf-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-403">Boolean</span></span>|<span data-ttu-id="a7cbf-404">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-404">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-405">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="a7cbf-405">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="a7cbf-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-406">Boolean</span></span>|<span data-ttu-id="a7cbf-407">指示在展台模式下是否要求语音过滤。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-407">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-408">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="a7cbf-408">kioskModeRequireZoom</span></span>|<span data-ttu-id="a7cbf-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-409">Boolean</span></span>|<span data-ttu-id="a7cbf-410">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-410">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="a7cbf-411">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="a7cbf-411">kioskModeManagedAppId</span></span>|<span data-ttu-id="a7cbf-412">String</span><span class="sxs-lookup"><span data-stu-id="a7cbf-412">String</span></span>|<span data-ttu-id="a7cbf-413">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-413">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="a7cbf-414">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-414">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="a7cbf-415">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="a7cbf-415">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="a7cbf-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-416">Boolean</span></span>|<span data-ttu-id="a7cbf-417">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-417">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="a7cbf-418">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="a7cbf-418">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="a7cbf-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-419">Boolean</span></span>|<span data-ttu-id="a7cbf-420">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-420">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="a7cbf-421">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="a7cbf-421">lockScreenBlockPassbook</span></span>|<span data-ttu-id="a7cbf-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-422">Boolean</span></span>|<span data-ttu-id="a7cbf-423">指示设备处于锁定状态时是否阻止用户使用 passbook。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-423">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="a7cbf-424">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="a7cbf-424">lockScreenBlockTodayView</span></span>|<span data-ttu-id="a7cbf-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-425">Boolean</span></span>|<span data-ttu-id="a7cbf-426">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-426">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="a7cbf-427">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a7cbf-427">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="a7cbf-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a7cbf-428">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="a7cbf-429">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-429">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="a7cbf-430">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="a7cbf-430">mediaContentRatingCanada</span></span>|[<span data-ttu-id="a7cbf-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="a7cbf-431">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="a7cbf-432">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-432">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="a7cbf-433">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a7cbf-433">mediaContentRatingFrance</span></span>|[<span data-ttu-id="a7cbf-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a7cbf-434">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="a7cbf-435">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-435">Media content rating settings for France</span></span>|
|<span data-ttu-id="a7cbf-436">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="a7cbf-436">mediaContentRatingGermany</span></span>|[<span data-ttu-id="a7cbf-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="a7cbf-437">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="a7cbf-438">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-438">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="a7cbf-439">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a7cbf-439">mediaContentRatingIreland</span></span>|[<span data-ttu-id="a7cbf-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a7cbf-440">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="a7cbf-441">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-441">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="a7cbf-442">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a7cbf-442">mediaContentRatingJapan</span></span>|[<span data-ttu-id="a7cbf-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a7cbf-443">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="a7cbf-444">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-444">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="a7cbf-445">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="a7cbf-445">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="a7cbf-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="a7cbf-446">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="a7cbf-447">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-447">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="a7cbf-448">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a7cbf-448">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="a7cbf-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a7cbf-449">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="a7cbf-450">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-450">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="a7cbf-451">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a7cbf-451">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="a7cbf-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a7cbf-452">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="a7cbf-453">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="a7cbf-453">Media content rating settings for United States</span></span>|
|<span data-ttu-id="a7cbf-454">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="a7cbf-454">networkUsageRules</span></span>|<span data-ttu-id="a7cbf-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="a7cbf-456">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-456">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="a7cbf-457">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-457">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a7cbf-458">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="a7cbf-458">mediaContentRatingApps</span></span>|[<span data-ttu-id="a7cbf-459">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-459">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="a7cbf-460">媒体内容应用程序的分级设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-460">Media content rating settings for Apps.</span></span> <span data-ttu-id="a7cbf-461">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-461">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="a7cbf-462">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-462">messagesBlocked</span></span>|<span data-ttu-id="a7cbf-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-463">Boolean</span></span>|<span data-ttu-id="a7cbf-464">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-464">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="a7cbf-465">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-465">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="a7cbf-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-466">Boolean</span></span>|<span data-ttu-id="a7cbf-467">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-467">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-468">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a7cbf-468">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="a7cbf-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-469">Boolean</span></span>|<span data-ttu-id="a7cbf-470">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-470">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a7cbf-471">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-471">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="a7cbf-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-472">Boolean</span></span>|<span data-ttu-id="a7cbf-473">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-473">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="a7cbf-474">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-474">passcodeBlockModification</span></span>|<span data-ttu-id="a7cbf-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-475">Boolean</span></span>|<span data-ttu-id="a7cbf-476">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-476">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-477">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a7cbf-477">passcodeBlockSimple</span></span>|<span data-ttu-id="a7cbf-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-478">Boolean</span></span>|<span data-ttu-id="a7cbf-479">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-479">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="a7cbf-480">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a7cbf-480">passcodeExpirationDays</span></span>|<span data-ttu-id="a7cbf-481">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-481">Int32</span></span>|<span data-ttu-id="a7cbf-482">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-482">Number of days before the passcode expires.</span></span> <span data-ttu-id="a7cbf-483">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="a7cbf-483">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a7cbf-484">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a7cbf-484">passcodeMinimumLength</span></span>|<span data-ttu-id="a7cbf-485">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-485">Int32</span></span>|<span data-ttu-id="a7cbf-486">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-486">Minimum length of passcode.</span></span> <span data-ttu-id="a7cbf-487">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="a7cbf-487">Valid values 4 to 14</span></span>|
|<span data-ttu-id="a7cbf-488">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a7cbf-488">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a7cbf-489">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-489">Int32</span></span>|<span data-ttu-id="a7cbf-490">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-490">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="a7cbf-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a7cbf-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a7cbf-492">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-492">Int32</span></span>|<span data-ttu-id="a7cbf-493">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-493">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a7cbf-494">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a7cbf-494">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="a7cbf-495">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-495">Int32</span></span>|<span data-ttu-id="a7cbf-496">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-496">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="a7cbf-497">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="a7cbf-497">Valid values 0 to 4</span></span>|
|<span data-ttu-id="a7cbf-498">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="a7cbf-498">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="a7cbf-499">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-499">Int32</span></span>|<span data-ttu-id="a7cbf-500">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-500">Number of previous passcodes to block.</span></span> <span data-ttu-id="a7cbf-501">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="a7cbf-501">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a7cbf-502">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="a7cbf-502">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="a7cbf-503">Int32</span><span class="sxs-lookup"><span data-stu-id="a7cbf-503">Int32</span></span>|<span data-ttu-id="a7cbf-504">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-504">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="a7cbf-505">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="a7cbf-505">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a7cbf-506">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-506">passcodeRequiredType</span></span>|[<span data-ttu-id="a7cbf-507">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a7cbf-507">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a7cbf-508">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-508">Type of passcode that is required.</span></span> <span data-ttu-id="a7cbf-509">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-509">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a7cbf-510">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="a7cbf-510">passcodeRequired</span></span>|<span data-ttu-id="a7cbf-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-511">Boolean</span></span>|<span data-ttu-id="a7cbf-512">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-512">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="a7cbf-513">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-513">podcastsBlocked</span></span>|<span data-ttu-id="a7cbf-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-514">Boolean</span></span>|<span data-ttu-id="a7cbf-515">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-515">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="a7cbf-516">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="a7cbf-516">safariBlockAutofill</span></span>|<span data-ttu-id="a7cbf-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-517">Boolean</span></span>|<span data-ttu-id="a7cbf-518">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-518">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="a7cbf-519">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="a7cbf-519">safariBlockJavaScript</span></span>|<span data-ttu-id="a7cbf-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-520">Boolean</span></span>|<span data-ttu-id="a7cbf-521">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-521">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="a7cbf-522">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="a7cbf-522">safariBlockPopups</span></span>|<span data-ttu-id="a7cbf-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-523">Boolean</span></span>|<span data-ttu-id="a7cbf-524">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-524">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="a7cbf-525">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-525">safariBlocked</span></span>|<span data-ttu-id="a7cbf-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-526">Boolean</span></span>|<span data-ttu-id="a7cbf-527">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-527">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="a7cbf-528">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-528">safariCookieSettings</span></span>|[<span data-ttu-id="a7cbf-529">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="a7cbf-529">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="a7cbf-530">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-530">Cookie settings for Safari.</span></span> <span data-ttu-id="a7cbf-531">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-531">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="a7cbf-532">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="a7cbf-532">safariManagedDomains</span></span>|<span data-ttu-id="a7cbf-533">String 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-533">String collection</span></span>|<span data-ttu-id="a7cbf-534">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-534">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="a7cbf-535">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="a7cbf-535">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="a7cbf-536">String 集合</span><span class="sxs-lookup"><span data-stu-id="a7cbf-536">String collection</span></span>|<span data-ttu-id="a7cbf-537">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-537">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="a7cbf-538">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-538">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a7cbf-539">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="a7cbf-539">safariRequireFraudWarning</span></span>|<span data-ttu-id="a7cbf-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-540">Boolean</span></span>|<span data-ttu-id="a7cbf-541">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-541">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="a7cbf-542">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-542">screenCaptureBlocked</span></span>|<span data-ttu-id="a7cbf-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-543">Boolean</span></span>|<span data-ttu-id="a7cbf-544">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-544">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="a7cbf-545">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-545">siriBlocked</span></span>|<span data-ttu-id="a7cbf-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-546">Boolean</span></span>|<span data-ttu-id="a7cbf-547">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-547">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="a7cbf-548">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-548">siriBlockedWhenLocked</span></span>|<span data-ttu-id="a7cbf-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-549">Boolean</span></span>|<span data-ttu-id="a7cbf-550">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-550">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="a7cbf-551">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="a7cbf-551">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="a7cbf-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-552">Boolean</span></span>|<span data-ttu-id="a7cbf-553">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-553">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="a7cbf-554">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="a7cbf-554">siriRequireProfanityFilter</span></span>|<span data-ttu-id="a7cbf-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-555">Boolean</span></span>|<span data-ttu-id="a7cbf-556">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-556">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="a7cbf-557">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="a7cbf-557">spotlightBlockInternetResults</span></span>|<span data-ttu-id="a7cbf-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-558">Boolean</span></span>|<span data-ttu-id="a7cbf-559">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-559">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="a7cbf-560">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="a7cbf-560">voiceDialingBlocked</span></span>|<span data-ttu-id="a7cbf-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-561">Boolean</span></span>|<span data-ttu-id="a7cbf-562">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-562">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="a7cbf-563">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="a7cbf-563">wallpaperBlockModification</span></span>|<span data-ttu-id="a7cbf-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-564">Boolean</span></span>|<span data-ttu-id="a7cbf-565">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-565">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="a7cbf-566">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="a7cbf-566">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="a7cbf-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7cbf-567">Boolean</span></span>|<span data-ttu-id="a7cbf-568">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-568">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="a7cbf-569">响应</span><span class="sxs-lookup"><span data-stu-id="a7cbf-569">Response</span></span>
<span data-ttu-id="a7cbf-570">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-570">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7cbf-571">示例</span><span class="sxs-lookup"><span data-stu-id="a7cbf-571">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7cbf-572">请求</span><span class="sxs-lookup"><span data-stu-id="a7cbf-572">Request</span></span>
<span data-ttu-id="a7cbf-573">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-573">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7cbf-574">响应</span><span class="sxs-lookup"><span data-stu-id="a7cbf-574">Response</span></span>
<span data-ttu-id="a7cbf-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7cbf-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



