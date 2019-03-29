---
title: 更新 iosGeneralDeviceConfiguration
description: 更新 iosGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f72ae25934e08c228375dbfefc6a243e87792b82
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974361"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="36938-103">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="36938-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="36938-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36938-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36938-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36938-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36938-106">更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="36938-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36938-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="36938-107">Prerequisites</span></span>
<span data-ttu-id="36938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36938-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36938-110">Permission type</span></span>|<span data-ttu-id="36938-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36938-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36938-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36938-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36938-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36938-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36938-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36938-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36938-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36938-115">Not supported.</span></span>|
|<span data-ttu-id="36938-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36938-116">Application</span></span>|<span data-ttu-id="36938-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="36938-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36938-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36938-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="36938-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="36938-119">Request headers</span></span>
|<span data-ttu-id="36938-120">标头</span><span class="sxs-lookup"><span data-stu-id="36938-120">Header</span></span>|<span data-ttu-id="36938-121">值</span><span class="sxs-lookup"><span data-stu-id="36938-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36938-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36938-122">Authorization</span></span>|<span data-ttu-id="36938-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36938-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36938-124">接受</span><span class="sxs-lookup"><span data-stu-id="36938-124">Accept</span></span>|<span data-ttu-id="36938-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36938-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36938-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36938-126">Request body</span></span>
<span data-ttu-id="36938-127">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36938-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="36938-128">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36938-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="36938-129">属性</span><span class="sxs-lookup"><span data-stu-id="36938-129">Property</span></span>|<span data-ttu-id="36938-130">类型</span><span class="sxs-lookup"><span data-stu-id="36938-130">Type</span></span>|<span data-ttu-id="36938-131">说明</span><span class="sxs-lookup"><span data-stu-id="36938-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36938-132">id</span><span class="sxs-lookup"><span data-stu-id="36938-132">id</span></span>|<span data-ttu-id="36938-133">String</span><span class="sxs-lookup"><span data-stu-id="36938-133">String</span></span>|<span data-ttu-id="36938-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="36938-134">Key of the entity.</span></span> <span data-ttu-id="36938-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36938-136">lastModifiedDateTime</span></span>|<span data-ttu-id="36938-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36938-137">DateTimeOffset</span></span>|<span data-ttu-id="36938-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="36938-138">DateTime the object was last modified.</span></span> <span data-ttu-id="36938-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36938-140">roleScopeTagIds</span></span>|<span data-ttu-id="36938-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="36938-141">String collection</span></span>|<span data-ttu-id="36938-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="36938-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36938-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="36938-144">supportsScopeTags</span></span>|<span data-ttu-id="36938-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-145">Boolean</span></span>|<span data-ttu-id="36938-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="36938-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36938-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="36938-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36938-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="36938-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36938-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="36938-149">This property is read-only.</span></span> <span data-ttu-id="36938-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36938-151">createdDateTime</span></span>|<span data-ttu-id="36938-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36938-152">DateTimeOffset</span></span>|<span data-ttu-id="36938-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="36938-153">DateTime the object was created.</span></span> <span data-ttu-id="36938-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-155">description</span><span class="sxs-lookup"><span data-stu-id="36938-155">description</span></span>|<span data-ttu-id="36938-156">String</span><span class="sxs-lookup"><span data-stu-id="36938-156">String</span></span>|<span data-ttu-id="36938-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="36938-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36938-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-159">displayName</span><span class="sxs-lookup"><span data-stu-id="36938-159">displayName</span></span>|<span data-ttu-id="36938-160">String</span><span class="sxs-lookup"><span data-stu-id="36938-160">String</span></span>|<span data-ttu-id="36938-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="36938-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36938-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-163">version</span><span class="sxs-lookup"><span data-stu-id="36938-163">version</span></span>|<span data-ttu-id="36938-164">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-164">Int32</span></span>|<span data-ttu-id="36938-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="36938-165">Version of the device configuration.</span></span> <span data-ttu-id="36938-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36938-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36938-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="36938-167">accountBlockModification</span></span>|<span data-ttu-id="36938-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-168">Boolean</span></span>|<span data-ttu-id="36938-169">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="36938-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="36938-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="36938-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-171">Boolean</span></span>|<span data-ttu-id="36938-172">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="36938-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="36938-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-173">airDropBlocked</span></span>|<span data-ttu-id="36938-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-174">Boolean</span></span>|<span data-ttu-id="36938-175">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="36938-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="36938-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="36938-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-177">Boolean</span></span>|<span data-ttu-id="36938-178">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="36938-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="36938-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-180">Boolean</span></span>|<span data-ttu-id="36938-181">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="36938-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="36938-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="36938-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="36938-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-183">Boolean</span></span>|<span data-ttu-id="36938-184">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="36938-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="36938-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-186">Boolean</span></span>|<span data-ttu-id="36938-187">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="36938-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-188">appleNewsBlocked</span></span>|<span data-ttu-id="36938-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-189">Boolean</span></span>|<span data-ttu-id="36938-190">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="36938-191">appsSingleAppModeList</span></span>|<span data-ttu-id="36938-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36938-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="36938-193">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="36938-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="36938-194">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="36938-194">Supervised only.</span></span> <span data-ttu-id="36938-195">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="36938-195">iOS 7.0 and later.</span></span> <span data-ttu-id="36938-196">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="36938-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="36938-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="36938-197">appsVisibilityList</span></span>|<span data-ttu-id="36938-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36938-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="36938-199">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="36938-200">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="36938-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="36938-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="36938-201">appsVisibilityListType</span></span>|[<span data-ttu-id="36938-202">appListType</span><span class="sxs-lookup"><span data-stu-id="36938-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="36938-203">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="36938-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="36938-204">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="36938-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="36938-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="36938-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="36938-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-206">Boolean</span></span>|<span data-ttu-id="36938-207">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-208">appStoreBlocked</span></span>|<span data-ttu-id="36938-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-209">Boolean</span></span>|<span data-ttu-id="36938-210">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="36938-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="36938-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="36938-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="36938-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-212">Boolean</span></span>|<span data-ttu-id="36938-213">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="36938-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="36938-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="36938-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="36938-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-215">Boolean</span></span>|<span data-ttu-id="36938-216">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="36938-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="36938-217">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="36938-218">appStoreRequirePassword</span></span>|<span data-ttu-id="36938-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-219">Boolean</span></span>|<span data-ttu-id="36938-220">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="36938-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="36938-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="36938-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="36938-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-222">Boolean</span></span>|<span data-ttu-id="36938-223">指示在 Safari 中的 autofilling 密码和信用卡信息之前是否强制进行用户身份验证, 以及受监督的设备上的其他应用。</span><span class="sxs-lookup"><span data-stu-id="36938-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="36938-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="36938-224">bluetoothBlockModification</span></span>|<span data-ttu-id="36938-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-225">Boolean</span></span>|<span data-ttu-id="36938-226">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="36938-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-227">cameraBlocked</span></span>|<span data-ttu-id="36938-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-228">Boolean</span></span>|<span data-ttu-id="36938-229">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="36938-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="36938-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="36938-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="36938-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-231">Boolean</span></span>|<span data-ttu-id="36938-232">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="36938-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="36938-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="36938-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="36938-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-234">Boolean</span></span>|<span data-ttu-id="36938-235">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="36938-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="36938-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="36938-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="36938-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-237">Boolean</span></span>|<span data-ttu-id="36938-238">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="36938-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="36938-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="36938-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-240">Boolean</span></span>|<span data-ttu-id="36938-241">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="36938-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="36938-242">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="36938-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="36938-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-243">Boolean</span></span>|<span data-ttu-id="36938-244">指示是否允许用户在受监督的设备上更改移动电话计划的设置。</span><span class="sxs-lookup"><span data-stu-id="36938-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="36938-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="36938-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="36938-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-246">Boolean</span></span>|<span data-ttu-id="36938-247">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="36938-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="36938-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="36938-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="36938-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-249">Boolean</span></span>|<span data-ttu-id="36938-250">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="36938-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="36938-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="36938-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="36938-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-252">Boolean</span></span>|<span data-ttu-id="36938-253">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="36938-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="36938-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="36938-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-255">Boolean</span></span>|<span data-ttu-id="36938-256">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="36938-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="36938-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="36938-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-258">Boolean</span></span>|<span data-ttu-id="36938-259">指示设备处于监督模式时是否自动向教师的请求授予权限, 而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="36938-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="36938-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="36938-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-261">Boolean</span></span>|<span data-ttu-id="36938-262">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="36938-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="36938-263">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="36938-263">Supervised only.</span></span>|
|<span data-ttu-id="36938-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="36938-264">compliantAppsList</span></span>|<span data-ttu-id="36938-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36938-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="36938-266">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="36938-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="36938-267">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="36938-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="36938-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="36938-268">compliantAppListType</span></span>|[<span data-ttu-id="36938-269">appListType</span><span class="sxs-lookup"><span data-stu-id="36938-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="36938-270">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="36938-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="36938-271">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="36938-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="36938-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="36938-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="36938-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-273">Boolean</span></span>|<span data-ttu-id="36938-274">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="36938-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-275">definitionLookupBlocked</span></span>|<span data-ttu-id="36938-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-276">Boolean</span></span>|<span data-ttu-id="36938-277">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="36938-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="36938-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="36938-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-279">Boolean</span></span>|<span data-ttu-id="36938-280">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="36938-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="36938-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="36938-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-282">Boolean</span></span>|<span data-ttu-id="36938-283">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="36938-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="36938-284">deviceBlockNameModification</span></span>|<span data-ttu-id="36938-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-285">Boolean</span></span>|<span data-ttu-id="36938-286">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="36938-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="36938-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-288">Boolean</span></span>|<span data-ttu-id="36938-289">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="36938-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="36938-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="36938-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="36938-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-291">Boolean</span></span>|<span data-ttu-id="36938-292">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="36938-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="36938-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="36938-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-294">Boolean</span></span>|<span data-ttu-id="36938-295">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="36938-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="36938-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="36938-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="36938-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-297">Boolean</span></span>|<span data-ttu-id="36938-298">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="36938-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="36938-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="36938-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="36938-300">String 集合</span><span class="sxs-lookup"><span data-stu-id="36938-300">String collection</span></span>|<span data-ttu-id="36938-301">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="36938-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="36938-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="36938-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="36938-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-303">Boolean</span></span>|<span data-ttu-id="36938-304">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="36938-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="36938-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="36938-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="36938-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-306">Boolean</span></span>|<span data-ttu-id="36938-307">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="36938-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="36938-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="36938-308">esimBlockModification</span></span>|<span data-ttu-id="36938-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-309">Boolean</span></span>|<span data-ttu-id="36938-310">指示是否允许在受监督的设备的 eSIM 卡上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="36938-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="36938-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-311">faceTimeBlocked</span></span>|<span data-ttu-id="36938-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-312">Boolean</span></span>|<span data-ttu-id="36938-313">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="36938-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="36938-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="36938-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-315">Boolean</span></span>|<span data-ttu-id="36938-316">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="36938-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="36938-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="36938-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-318">Boolean</span></span>|<span data-ttu-id="36938-319">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="36938-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="36938-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="36938-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="36938-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-321">Boolean</span></span>|<span data-ttu-id="36938-322">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="36938-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="36938-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-323">gameCenterBlocked</span></span>|<span data-ttu-id="36938-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-324">Boolean</span></span>|<span data-ttu-id="36938-325">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="36938-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-326">hostPairingBlocked</span></span>|<span data-ttu-id="36938-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-327">Boolean</span></span>|<span data-ttu-id="36938-328">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="36938-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="36938-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-330">Boolean</span></span>|<span data-ttu-id="36938-331">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="36938-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="36938-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="36938-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-333">Boolean</span></span>|<span data-ttu-id="36938-334">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="36938-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="36938-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="36938-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="36938-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-336">Boolean</span></span>|<span data-ttu-id="36938-337">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="36938-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="36938-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="36938-338">iCloudBlockBackup</span></span>|<span data-ttu-id="36938-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-339">Boolean</span></span>|<span data-ttu-id="36938-340">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="36938-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="36938-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="36938-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="36938-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-342">Boolean</span></span>|<span data-ttu-id="36938-343">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="36938-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="36938-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="36938-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="36938-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-345">Boolean</span></span>|<span data-ttu-id="36938-346">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="36938-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="36938-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="36938-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="36938-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-348">Boolean</span></span>|<span data-ttu-id="36938-349">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="36938-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="36938-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="36938-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="36938-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-351">Boolean</span></span>|<span data-ttu-id="36938-352">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="36938-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="36938-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="36938-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="36938-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-354">Boolean</span></span>|<span data-ttu-id="36938-355">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="36938-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="36938-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="36938-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="36938-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-357">Boolean</span></span>|<span data-ttu-id="36938-358">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="36938-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="36938-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="36938-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="36938-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-360">Boolean</span></span>|<span data-ttu-id="36938-361">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="36938-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="36938-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="36938-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="36938-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-363">Boolean</span></span>|<span data-ttu-id="36938-364">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="36938-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="36938-365">iTunesBlockRadio</span></span>|<span data-ttu-id="36938-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-366">Boolean</span></span>|<span data-ttu-id="36938-367">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="36938-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="36938-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="36938-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-369">Boolean</span></span>|<span data-ttu-id="36938-370">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="36938-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="36938-371">keyboardBlockDictation</span></span>|<span data-ttu-id="36938-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-372">Boolean</span></span>|<span data-ttu-id="36938-373">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="36938-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="36938-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="36938-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-375">Boolean</span></span>|<span data-ttu-id="36938-376">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="36938-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="36938-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="36938-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-378">Boolean</span></span>|<span data-ttu-id="36938-379">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="36938-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="36938-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-381">Boolean</span></span>|<span data-ttu-id="36938-382">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="36938-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="36938-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="36938-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-384">Boolean</span></span>|<span data-ttu-id="36938-385">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="36938-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="36938-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="36938-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-387">Boolean</span></span>|<span data-ttu-id="36938-388">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="36938-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="36938-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="36938-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-390">Boolean</span></span>|<span data-ttu-id="36938-391">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="36938-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="36938-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="36938-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-393">Boolean</span></span>|<span data-ttu-id="36938-394">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="36938-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="36938-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="36938-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-396">Boolean</span></span>|<span data-ttu-id="36938-397">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="36938-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="36938-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="36938-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-399">Boolean</span></span>|<span data-ttu-id="36938-400">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="36938-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="36938-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="36938-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-402">Boolean</span></span>|<span data-ttu-id="36938-403">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="36938-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="36938-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="36938-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-405">Boolean</span></span>|<span data-ttu-id="36938-406">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="36938-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="36938-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="36938-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-408">Boolean</span></span>|<span data-ttu-id="36938-409">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="36938-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="36938-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="36938-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-411">Boolean</span></span>|<span data-ttu-id="36938-412">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="36938-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="36938-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="36938-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-414">Boolean</span></span>|<span data-ttu-id="36938-415">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="36938-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="36938-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="36938-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="36938-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-417">Boolean</span></span>|<span data-ttu-id="36938-418">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="36938-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="36938-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="36938-420">String</span><span class="sxs-lookup"><span data-stu-id="36938-420">String</span></span>|<span data-ttu-id="36938-421">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="36938-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="36938-422">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="36938-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="36938-423">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="36938-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="36938-424">String</span><span class="sxs-lookup"><span data-stu-id="36938-424">String</span></span>|<span data-ttu-id="36938-425">用于展台模式的内置应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="36938-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="36938-426">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="36938-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="36938-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="36938-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="36938-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-428">Boolean</span></span>|<span data-ttu-id="36938-429">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="36938-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="36938-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="36938-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-431">Boolean</span></span>|<span data-ttu-id="36938-432">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="36938-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="36938-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="36938-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-434">Boolean</span></span>|<span data-ttu-id="36938-435">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="36938-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="36938-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="36938-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-437">Boolean</span></span>|<span data-ttu-id="36938-438">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="36938-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="36938-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="36938-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-440">Boolean</span></span>|<span data-ttu-id="36938-441">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="36938-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="36938-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="36938-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="36938-443">String</span><span class="sxs-lookup"><span data-stu-id="36938-443">String</span></span>|<span data-ttu-id="36938-444">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="36938-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="36938-445">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="36938-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="36938-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="36938-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="36938-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-447">Boolean</span></span>|<span data-ttu-id="36938-448">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="36938-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="36938-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="36938-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="36938-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-450">Boolean</span></span>|<span data-ttu-id="36938-451">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="36938-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="36938-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="36938-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="36938-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-453">Boolean</span></span>|<span data-ttu-id="36938-454">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="36938-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="36938-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="36938-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="36938-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-456">Boolean</span></span>|<span data-ttu-id="36938-457">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="36938-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="36938-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="36938-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="36938-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="36938-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="36938-460">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="36938-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="36938-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="36938-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="36938-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="36938-463">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="36938-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="36938-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="36938-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="36938-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="36938-466">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="36938-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="36938-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="36938-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="36938-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="36938-469">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="36938-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="36938-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="36938-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="36938-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="36938-472">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="36938-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="36938-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="36938-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="36938-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="36938-475">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="36938-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="36938-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="36938-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="36938-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="36938-478">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="36938-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="36938-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="36938-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="36938-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="36938-481">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="36938-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="36938-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="36938-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="36938-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="36938-484">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="36938-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="36938-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="36938-485">networkUsageRules</span></span>|<span data-ttu-id="36938-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36938-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="36938-487">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="36938-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="36938-488">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="36938-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="36938-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="36938-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="36938-490">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="36938-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="36938-491">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="36938-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="36938-492">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="36938-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="36938-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-493">messagesBlocked</span></span>|<span data-ttu-id="36938-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-494">Boolean</span></span>|<span data-ttu-id="36938-495">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="36938-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="36938-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="36938-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="36938-497">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-497">Boolean</span></span>|<span data-ttu-id="36938-498">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="36938-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="36938-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="36938-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-500">Boolean</span></span>|<span data-ttu-id="36938-501">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="36938-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="36938-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="36938-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="36938-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-503">Boolean</span></span>|<span data-ttu-id="36938-504">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="36938-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="36938-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="36938-505">passcodeBlockModification</span></span>|<span data-ttu-id="36938-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-506">Boolean</span></span>|<span data-ttu-id="36938-507">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="36938-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="36938-508">passcodeBlockSimple</span></span>|<span data-ttu-id="36938-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-509">Boolean</span></span>|<span data-ttu-id="36938-510">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="36938-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="36938-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="36938-511">passcodeExpirationDays</span></span>|<span data-ttu-id="36938-512">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-512">Int32</span></span>|<span data-ttu-id="36938-513">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="36938-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="36938-514">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="36938-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="36938-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="36938-515">passcodeMinimumLength</span></span>|<span data-ttu-id="36938-516">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-516">Int32</span></span>|<span data-ttu-id="36938-517">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="36938-517">Minimum length of passcode.</span></span> <span data-ttu-id="36938-518">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="36938-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="36938-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="36938-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="36938-520">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-520">Int32</span></span>|<span data-ttu-id="36938-521">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="36938-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="36938-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="36938-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="36938-523">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-523">Int32</span></span>|<span data-ttu-id="36938-524">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="36938-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="36938-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="36938-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="36938-526">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-526">Int32</span></span>|<span data-ttu-id="36938-527">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="36938-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="36938-528">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="36938-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="36938-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="36938-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="36938-530">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-530">Int32</span></span>|<span data-ttu-id="36938-531">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="36938-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="36938-532">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="36938-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="36938-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="36938-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="36938-534">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-534">Int32</span></span>|<span data-ttu-id="36938-535">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="36938-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="36938-536">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="36938-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="36938-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="36938-537">passcodeRequiredType</span></span>|[<span data-ttu-id="36938-538">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="36938-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="36938-539">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="36938-539">Type of passcode that is required.</span></span> <span data-ttu-id="36938-540">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="36938-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="36938-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="36938-541">passcodeRequired</span></span>|<span data-ttu-id="36938-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-542">Boolean</span></span>|<span data-ttu-id="36938-543">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="36938-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="36938-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-544">podcastsBlocked</span></span>|<span data-ttu-id="36938-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-545">Boolean</span></span>|<span data-ttu-id="36938-546">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="36938-547">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="36938-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="36938-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-548">Boolean</span></span>|<span data-ttu-id="36938-549">指示是否启用提示以在受监督的设备上安装附近设备。</span><span class="sxs-lookup"><span data-stu-id="36938-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="36938-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="36938-550">safariBlockAutofill</span></span>|<span data-ttu-id="36938-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-551">Boolean</span></span>|<span data-ttu-id="36938-552">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="36938-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="36938-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="36938-553">safariBlockJavaScript</span></span>|<span data-ttu-id="36938-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-554">Boolean</span></span>|<span data-ttu-id="36938-555">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="36938-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="36938-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="36938-556">safariBlockPopups</span></span>|<span data-ttu-id="36938-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-557">Boolean</span></span>|<span data-ttu-id="36938-558">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="36938-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="36938-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-559">safariBlocked</span></span>|<span data-ttu-id="36938-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-560">Boolean</span></span>|<span data-ttu-id="36938-561">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="36938-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="36938-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="36938-562">safariCookieSettings</span></span>|[<span data-ttu-id="36938-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="36938-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="36938-564">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="36938-564">Cookie settings for Safari.</span></span> <span data-ttu-id="36938-565">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="36938-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="36938-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="36938-566">safariManagedDomains</span></span>|<span data-ttu-id="36938-567">String 集合</span><span class="sxs-lookup"><span data-stu-id="36938-567">String collection</span></span>|<span data-ttu-id="36938-568">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="36938-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="36938-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="36938-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="36938-570">String 集合</span><span class="sxs-lookup"><span data-stu-id="36938-570">String collection</span></span>|<span data-ttu-id="36938-571">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="36938-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="36938-572">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="36938-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="36938-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="36938-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-574">Boolean</span></span>|<span data-ttu-id="36938-575">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="36938-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="36938-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-576">screenCaptureBlocked</span></span>|<span data-ttu-id="36938-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-577">Boolean</span></span>|<span data-ttu-id="36938-578">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="36938-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="36938-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-579">siriBlocked</span></span>|<span data-ttu-id="36938-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-580">Boolean</span></span>|<span data-ttu-id="36938-581">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="36938-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="36938-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="36938-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="36938-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-583">Boolean</span></span>|<span data-ttu-id="36938-584">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="36938-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="36938-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="36938-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="36938-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-586">Boolean</span></span>|<span data-ttu-id="36938-587">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="36938-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="36938-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="36938-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="36938-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-589">Boolean</span></span>|<span data-ttu-id="36938-590">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="36938-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="36938-591">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="36938-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="36938-592">Int32</span><span class="sxs-lookup"><span data-stu-id="36938-592">Int32</span></span>|<span data-ttu-id="36938-593">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="36938-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="36938-594">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="36938-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="36938-595">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="36938-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="36938-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-596">Boolean</span></span>|<span data-ttu-id="36938-597">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="36938-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="36938-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="36938-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-599">Boolean</span></span>|<span data-ttu-id="36938-600">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="36938-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="36938-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-601">voiceDialingBlocked</span></span>|<span data-ttu-id="36938-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-602">Boolean</span></span>|<span data-ttu-id="36938-603">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="36938-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="36938-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="36938-604">wallpaperBlockModification</span></span>|<span data-ttu-id="36938-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-605">Boolean</span></span>|<span data-ttu-id="36938-606">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="36938-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="36938-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="36938-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="36938-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-608">Boolean</span></span>|<span data-ttu-id="36938-609">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="36938-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="36938-610">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="36938-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="36938-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-611">Boolean</span></span>|<span data-ttu-id="36938-612">指示在非托管课程中通过教室注册的学生是否会在尝试离开该课程 (iOS 11.3 及更高版本) 时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="36938-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="36938-613">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="36938-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="36938-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-614">Boolean</span></span>|<span data-ttu-id="36938-615">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="36938-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="36938-616">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="36938-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="36938-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-617">Boolean</span></span>|<span data-ttu-id="36938-618">指示是否阻止无线 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="36938-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="36938-619">将此限制设置为 false 不会禁用 CRL 和 OCSP 检查 (iOS 7.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="36938-620">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="36938-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="36938-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-621">Boolean</span></span>|<span data-ttu-id="36938-622">指示广告跟踪是否受限制。(iOS 7.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="36938-623">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="36938-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="36938-624">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-624">Boolean</span></span>|<span data-ttu-id="36938-625">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="36938-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="36938-626">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="36938-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="36938-627">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-627">Boolean</span></span>|<span data-ttu-id="36938-628">指示是否阻止企业书籍笔记和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="36938-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="36938-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-629">airPrintBlocked</span></span>|<span data-ttu-id="36938-630">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-630">Boolean</span></span>|<span data-ttu-id="36938-631">指示是否阻止 AirPrint (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="36938-632">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="36938-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="36938-633">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-633">Boolean</span></span>|<span data-ttu-id="36938-634">指示是否阻止 Airprint 的用户名和密码的密钥链存储 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="36938-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="36938-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="36938-636">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-636">Boolean</span></span>|<span data-ttu-id="36938-637">指示 TLS 打印通信是否需要受信任的证书 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="36938-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="36938-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="36938-639">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-639">Boolean</span></span>|<span data-ttu-id="36938-640">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="36938-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="36938-641">这样可以防止虚假的 AirPrint 蓝牙信号免受网络流量 (iOS 11.0 及更高版本) 的欺骗。</span><span class="sxs-lookup"><span data-stu-id="36938-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="36938-642">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="36938-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="36938-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-643">Boolean</span></span>|<span data-ttu-id="36938-644">指示是否在受监督的设备 (iOS 11.0 及更高版本) 上阻止从设备中删除系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="36938-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="36938-645">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="36938-645">vpnBlockCreation</span></span>|<span data-ttu-id="36938-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-646">Boolean</span></span>|<span data-ttu-id="36938-647">指示是否阻止创建 VPN 配置 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="36938-648">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-648">appRemovalBlocked</span></span>|<span data-ttu-id="36938-649">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-649">Boolean</span></span>|<span data-ttu-id="36938-650">指示是否允许删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="36938-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="36938-651">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="36938-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="36938-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-652">Boolean</span></span>|<span data-ttu-id="36938-653">指示是否允许在锁定设备时连接到 USB 附件 (iOS 11.4.1 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="36938-654">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="36938-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="36938-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-655">Boolean</span></span>|<span data-ttu-id="36938-656">指示是否允许自动填充密码功能 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="36938-657">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="36938-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="36938-658">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-658">Boolean</span></span>|<span data-ttu-id="36938-659">指示是否阻止来自附近设备 (iOS 12.0 及更高版本) 发出请求的密码。</span><span class="sxs-lookup"><span data-stu-id="36938-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="36938-660">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="36938-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="36938-661">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-661">Boolean</span></span>|<span data-ttu-id="36938-662">指示是否阻止使用 AirDrop 密码的共享密码功能 iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="36938-663">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="36938-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="36938-664">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-664">Boolean</span></span>|<span data-ttu-id="36938-665">指示是否启用日期和时间 "设置自动设置" 功能, 以及用户是否无法关闭该功能 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="36938-666">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="36938-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="36938-667">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-667">Boolean</span></span>|<span data-ttu-id="36938-668">指示托管应用程序是否可以将联系人写入非托管联系人帐户 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="36938-669">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="36938-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="36938-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="36938-670">Boolean</span></span>|<span data-ttu-id="36938-671">指示非托管应用是否可以从托管联系人帐户读取 (iOS 12.0 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="36938-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="36938-672">响应</span><span class="sxs-lookup"><span data-stu-id="36938-672">Response</span></span>
<span data-ttu-id="36938-673">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36938-673">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36938-674">示例</span><span class="sxs-lookup"><span data-stu-id="36938-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="36938-675">请求</span><span class="sxs-lookup"><span data-stu-id="36938-675">Request</span></span>
<span data-ttu-id="36938-676">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36938-676">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9105

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "esimBlockModification": true,
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
  "kioskModeBlockVolumeButtons": true,
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
  "proximityBlockSetupToNewDevice": true,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```

### <a name="response"></a><span data-ttu-id="36938-677">响应</span><span class="sxs-lookup"><span data-stu-id="36938-677">Response</span></span>
<span data-ttu-id="36938-p133">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36938-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9277

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "esimBlockModification": true,
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
  "kioskModeBlockVolumeButtons": true,
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
  "proximityBlockSetupToNewDevice": true,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```




