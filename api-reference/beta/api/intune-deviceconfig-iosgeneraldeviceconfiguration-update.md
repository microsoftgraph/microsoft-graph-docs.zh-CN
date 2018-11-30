---
title: 更新 iosGeneralDeviceConfiguration
description: 更新 iosGeneralDeviceConfiguration 对象的属性。
ms.openlocfilehash: 651915670976792e923ba34d8d560521742bbd44
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041778"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="27909-103">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="27909-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="27909-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27909-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27909-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27909-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27909-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="27909-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27909-107">更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27909-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27909-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27909-108">Prerequisites</span></span>
<span data-ttu-id="27909-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="27909-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27909-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27909-111">Permission type</span></span>|<span data-ttu-id="27909-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27909-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27909-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27909-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27909-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27909-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27909-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27909-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27909-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27909-116">Not supported.</span></span>|
|<span data-ttu-id="27909-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="27909-117">Application</span></span>|<span data-ttu-id="27909-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="27909-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27909-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27909-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="27909-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27909-120">Request headers</span></span>
|<span data-ttu-id="27909-121">标头</span><span class="sxs-lookup"><span data-stu-id="27909-121">Header</span></span>|<span data-ttu-id="27909-122">值</span><span class="sxs-lookup"><span data-stu-id="27909-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27909-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27909-123">Authorization</span></span>|<span data-ttu-id="27909-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27909-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27909-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27909-125">Accept</span></span>|<span data-ttu-id="27909-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27909-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27909-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27909-127">Request body</span></span>
<span data-ttu-id="27909-128">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27909-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="27909-129">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27909-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="27909-130">属性</span><span class="sxs-lookup"><span data-stu-id="27909-130">Property</span></span>|<span data-ttu-id="27909-131">类型</span><span class="sxs-lookup"><span data-stu-id="27909-131">Type</span></span>|<span data-ttu-id="27909-132">说明</span><span class="sxs-lookup"><span data-stu-id="27909-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27909-133">id</span><span class="sxs-lookup"><span data-stu-id="27909-133">id</span></span>|<span data-ttu-id="27909-134">String</span><span class="sxs-lookup"><span data-stu-id="27909-134">String</span></span>|<span data-ttu-id="27909-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27909-135">Key of the entity.</span></span> <span data-ttu-id="27909-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27909-137">lastModifiedDateTime</span></span>|<span data-ttu-id="27909-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27909-138">DateTimeOffset</span></span>|<span data-ttu-id="27909-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27909-139">DateTime the object was last modified.</span></span> <span data-ttu-id="27909-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27909-141">roleScopeTagIds</span></span>|<span data-ttu-id="27909-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="27909-142">String collection</span></span>|<span data-ttu-id="27909-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="27909-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="27909-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="27909-145">supportsScopeTags</span></span>|<span data-ttu-id="27909-146">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-146">Boolean</span></span>|<span data-ttu-id="27909-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="27909-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="27909-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="27909-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="27909-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="27909-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="27909-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="27909-150">This property is read-only.</span></span> <span data-ttu-id="27909-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27909-152">createdDateTime</span></span>|<span data-ttu-id="27909-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27909-153">DateTimeOffset</span></span>|<span data-ttu-id="27909-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27909-154">DateTime the object was created.</span></span> <span data-ttu-id="27909-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-156">description</span><span class="sxs-lookup"><span data-stu-id="27909-156">description</span></span>|<span data-ttu-id="27909-157">String</span><span class="sxs-lookup"><span data-stu-id="27909-157">String</span></span>|<span data-ttu-id="27909-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="27909-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27909-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-160">displayName</span><span class="sxs-lookup"><span data-stu-id="27909-160">displayName</span></span>|<span data-ttu-id="27909-161">String</span><span class="sxs-lookup"><span data-stu-id="27909-161">String</span></span>|<span data-ttu-id="27909-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="27909-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27909-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-164">version</span><span class="sxs-lookup"><span data-stu-id="27909-164">version</span></span>|<span data-ttu-id="27909-165">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-165">Int32</span></span>|<span data-ttu-id="27909-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="27909-166">Version of the device configuration.</span></span> <span data-ttu-id="27909-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27909-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27909-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="27909-168">accountBlockModification</span></span>|<span data-ttu-id="27909-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-169">Boolean</span></span>|<span data-ttu-id="27909-170">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="27909-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="27909-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="27909-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-172">Boolean</span></span>|<span data-ttu-id="27909-173">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="27909-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="27909-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-174">airDropBlocked</span></span>|<span data-ttu-id="27909-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-175">Boolean</span></span>|<span data-ttu-id="27909-176">指示设备处于监督模式时是否允许使用 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="27909-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="27909-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="27909-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-178">Boolean</span></span>|<span data-ttu-id="27909-179">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="27909-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="27909-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-181">Boolean</span></span>|<span data-ttu-id="27909-182">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="27909-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="27909-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="27909-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="27909-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-184">Boolean</span></span>|<span data-ttu-id="27909-185">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="27909-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="27909-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-187">Boolean</span></span>|<span data-ttu-id="27909-188">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="27909-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-189">appleNewsBlocked</span></span>|<span data-ttu-id="27909-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-190">Boolean</span></span>|<span data-ttu-id="27909-191">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="27909-192">appsSingleAppModeList</span></span>|<span data-ttu-id="27909-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27909-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="27909-194">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="27909-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="27909-195">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="27909-195">Supervised only.</span></span> <span data-ttu-id="27909-196">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="27909-196">iOS 7.0 and later.</span></span> <span data-ttu-id="27909-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="27909-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="27909-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="27909-198">appsVisibilityList</span></span>|<span data-ttu-id="27909-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27909-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="27909-200">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="27909-201">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="27909-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="27909-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="27909-202">appsVisibilityListType</span></span>|[<span data-ttu-id="27909-203">appListType</span><span class="sxs-lookup"><span data-stu-id="27909-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="27909-204">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="27909-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="27909-205">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="27909-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="27909-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="27909-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="27909-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-207">Boolean</span></span>|<span data-ttu-id="27909-208">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-209">appStoreBlocked</span></span>|<span data-ttu-id="27909-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-210">Boolean</span></span>|<span data-ttu-id="27909-211">指示是否阻止用户使用应用商店。</span><span class="sxs-lookup"><span data-stu-id="27909-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="27909-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="27909-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="27909-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-213">Boolean</span></span>|<span data-ttu-id="27909-214">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="27909-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="27909-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="27909-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="27909-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-216">Boolean</span></span>|<span data-ttu-id="27909-217">指示是否阻止应用商店应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="27909-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="27909-218">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="27909-219">appStoreRequirePassword</span></span>|<span data-ttu-id="27909-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-220">Boolean</span></span>|<span data-ttu-id="27909-221">指示使用应用商店时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="27909-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="27909-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="27909-222">bluetoothBlockModification</span></span>|<span data-ttu-id="27909-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-223">Boolean</span></span>|<span data-ttu-id="27909-224">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="27909-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-225">cameraBlocked</span></span>|<span data-ttu-id="27909-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-226">Boolean</span></span>|<span data-ttu-id="27909-227">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="27909-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="27909-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="27909-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="27909-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-229">Boolean</span></span>|<span data-ttu-id="27909-230">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="27909-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="27909-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="27909-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="27909-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-232">Boolean</span></span>|<span data-ttu-id="27909-233">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="27909-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="27909-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="27909-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="27909-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-235">Boolean</span></span>|<span data-ttu-id="27909-236">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="27909-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="27909-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="27909-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-238">Boolean</span></span>|<span data-ttu-id="27909-239">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="27909-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="27909-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="27909-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="27909-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-241">Boolean</span></span>|<span data-ttu-id="27909-242">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="27909-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="27909-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="27909-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="27909-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-244">Boolean</span></span>|<span data-ttu-id="27909-245">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="27909-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="27909-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="27909-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="27909-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-247">Boolean</span></span>|<span data-ttu-id="27909-248">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="27909-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="27909-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="27909-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-250">Boolean</span></span>|<span data-ttu-id="27909-251">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="27909-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="27909-252">compliantAppsList</span></span>|<span data-ttu-id="27909-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27909-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="27909-254">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="27909-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="27909-255">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="27909-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="27909-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="27909-256">compliantAppListType</span></span>|[<span data-ttu-id="27909-257">appListType</span><span class="sxs-lookup"><span data-stu-id="27909-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="27909-258">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="27909-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="27909-259">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="27909-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="27909-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="27909-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="27909-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-261">Boolean</span></span>|<span data-ttu-id="27909-262">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="27909-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-263">definitionLookupBlocked</span></span>|<span data-ttu-id="27909-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-264">Boolean</span></span>|<span data-ttu-id="27909-265">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="27909-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="27909-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="27909-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-267">Boolean</span></span>|<span data-ttu-id="27909-268">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="27909-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="27909-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="27909-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-270">Boolean</span></span>|<span data-ttu-id="27909-271">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="27909-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="27909-272">deviceBlockNameModification</span></span>|<span data-ttu-id="27909-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-273">Boolean</span></span>|<span data-ttu-id="27909-274">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="27909-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="27909-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-276">Boolean</span></span>|<span data-ttu-id="27909-277">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="27909-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="27909-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="27909-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="27909-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-279">Boolean</span></span>|<span data-ttu-id="27909-280">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="27909-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="27909-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="27909-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-282">Boolean</span></span>|<span data-ttu-id="27909-283">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="27909-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="27909-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="27909-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="27909-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-285">Boolean</span></span>|<span data-ttu-id="27909-286">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="27909-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="27909-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="27909-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="27909-288">String 集合</span><span class="sxs-lookup"><span data-stu-id="27909-288">String collection</span></span>|<span data-ttu-id="27909-289">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="27909-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="27909-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="27909-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="27909-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-291">Boolean</span></span>|<span data-ttu-id="27909-292">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="27909-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="27909-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="27909-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="27909-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-294">Boolean</span></span>|<span data-ttu-id="27909-295">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="27909-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="27909-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-296">faceTimeBlocked</span></span>|<span data-ttu-id="27909-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-297">Boolean</span></span>|<span data-ttu-id="27909-298">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="27909-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="27909-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="27909-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-300">Boolean</span></span>|<span data-ttu-id="27909-301">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="27909-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="27909-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="27909-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-303">Boolean</span></span>|<span data-ttu-id="27909-304">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="27909-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="27909-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="27909-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="27909-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-306">Boolean</span></span>|<span data-ttu-id="27909-307">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="27909-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="27909-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-308">gameCenterBlocked</span></span>|<span data-ttu-id="27909-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-309">Boolean</span></span>|<span data-ttu-id="27909-310">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="27909-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-311">hostPairingBlocked</span></span>|<span data-ttu-id="27909-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-312">Boolean</span></span>|<span data-ttu-id="27909-313">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="27909-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="27909-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-315">Boolean</span></span>|<span data-ttu-id="27909-316">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="27909-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="27909-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="27909-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-318">Boolean</span></span>|<span data-ttu-id="27909-319">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="27909-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="27909-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="27909-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="27909-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-321">Boolean</span></span>|<span data-ttu-id="27909-322">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="27909-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="27909-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="27909-323">iCloudBlockBackup</span></span>|<span data-ttu-id="27909-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-324">Boolean</span></span>|<span data-ttu-id="27909-325">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="27909-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="27909-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="27909-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="27909-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-327">Boolean</span></span>|<span data-ttu-id="27909-328">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="27909-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="27909-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="27909-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="27909-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-330">Boolean</span></span>|<span data-ttu-id="27909-331">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="27909-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="27909-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="27909-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="27909-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-333">Boolean</span></span>|<span data-ttu-id="27909-334">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="27909-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="27909-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="27909-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="27909-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-336">Boolean</span></span>|<span data-ttu-id="27909-337">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="27909-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="27909-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="27909-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="27909-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-339">Boolean</span></span>|<span data-ttu-id="27909-340">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="27909-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="27909-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="27909-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="27909-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-342">Boolean</span></span>|<span data-ttu-id="27909-343">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="27909-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="27909-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="27909-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="27909-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-345">Boolean</span></span>|<span data-ttu-id="27909-346">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="27909-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="27909-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="27909-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="27909-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-348">Boolean</span></span>|<span data-ttu-id="27909-349">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="27909-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="27909-350">iTunesBlockRadio</span></span>|<span data-ttu-id="27909-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-351">Boolean</span></span>|<span data-ttu-id="27909-352">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="27909-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="27909-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="27909-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-354">Boolean</span></span>|<span data-ttu-id="27909-355">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="27909-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="27909-356">keyboardBlockDictation</span></span>|<span data-ttu-id="27909-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-357">Boolean</span></span>|<span data-ttu-id="27909-358">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="27909-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="27909-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="27909-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-360">Boolean</span></span>|<span data-ttu-id="27909-361">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="27909-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="27909-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="27909-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-363">Boolean</span></span>|<span data-ttu-id="27909-364">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="27909-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="27909-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-366">Boolean</span></span>|<span data-ttu-id="27909-367">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="27909-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="27909-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="27909-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-369">Boolean</span></span>|<span data-ttu-id="27909-370">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="27909-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="27909-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="27909-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-372">Boolean</span></span>|<span data-ttu-id="27909-373">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="27909-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="27909-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="27909-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-375">Boolean</span></span>|<span data-ttu-id="27909-376">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="27909-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="27909-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="27909-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-378">Boolean</span></span>|<span data-ttu-id="27909-379">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="27909-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="27909-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="27909-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-381">Boolean</span></span>|<span data-ttu-id="27909-382">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="27909-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="27909-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="27909-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-384">Boolean</span></span>|<span data-ttu-id="27909-385">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="27909-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="27909-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="27909-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-387">Boolean</span></span>|<span data-ttu-id="27909-388">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="27909-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="27909-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="27909-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-390">Boolean</span></span>|<span data-ttu-id="27909-391">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="27909-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="27909-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="27909-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-393">Boolean</span></span>|<span data-ttu-id="27909-394">指示在展台模式下是否允许访问语音过滤设置。</span><span class="sxs-lookup"><span data-stu-id="27909-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="27909-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="27909-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-396">Boolean</span></span>|<span data-ttu-id="27909-397">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="27909-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="27909-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="27909-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-399">Boolean</span></span>|<span data-ttu-id="27909-400">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="27909-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="27909-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="27909-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="27909-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-402">Boolean</span></span>|<span data-ttu-id="27909-403">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="27909-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="27909-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="27909-405">String</span><span class="sxs-lookup"><span data-stu-id="27909-405">String</span></span>|<span data-ttu-id="27909-406">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="27909-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="27909-407">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="27909-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="27909-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="27909-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="27909-409">字符串</span><span class="sxs-lookup"><span data-stu-id="27909-409">String</span></span>|<span data-ttu-id="27909-410">用于展台模式内置应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="27909-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="27909-411">未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="27909-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="27909-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="27909-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="27909-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-413">Boolean</span></span>|<span data-ttu-id="27909-414">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="27909-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="27909-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="27909-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-416">Boolean</span></span>|<span data-ttu-id="27909-417">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="27909-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="27909-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="27909-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-419">Boolean</span></span>|<span data-ttu-id="27909-420">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="27909-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="27909-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="27909-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-422">Boolean</span></span>|<span data-ttu-id="27909-423">指示在展台模式下是否要求语音过滤。</span><span class="sxs-lookup"><span data-stu-id="27909-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="27909-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="27909-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-425">Boolean</span></span>|<span data-ttu-id="27909-426">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="27909-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="27909-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="27909-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="27909-428">String</span><span class="sxs-lookup"><span data-stu-id="27909-428">String</span></span>|<span data-ttu-id="27909-429">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="27909-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="27909-430">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="27909-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="27909-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="27909-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="27909-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-432">Boolean</span></span>|<span data-ttu-id="27909-433">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="27909-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="27909-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="27909-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="27909-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-435">Boolean</span></span>|<span data-ttu-id="27909-436">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="27909-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="27909-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="27909-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="27909-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-438">Boolean</span></span>|<span data-ttu-id="27909-439">指示设备处于锁定状态时是否阻止用户使用 passbook。</span><span class="sxs-lookup"><span data-stu-id="27909-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="27909-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="27909-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="27909-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-441">Boolean</span></span>|<span data-ttu-id="27909-442">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="27909-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="27909-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="27909-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="27909-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="27909-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="27909-445">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="27909-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="27909-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="27909-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="27909-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="27909-448">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="27909-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="27909-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="27909-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="27909-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="27909-451">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="27909-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="27909-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="27909-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="27909-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="27909-454">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="27909-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="27909-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="27909-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="27909-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="27909-457">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="27909-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="27909-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="27909-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="27909-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="27909-460">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="27909-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="27909-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="27909-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="27909-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="27909-463">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="27909-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="27909-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="27909-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="27909-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="27909-466">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="27909-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="27909-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="27909-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="27909-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="27909-469">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="27909-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="27909-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="27909-470">networkUsageRules</span></span>|<span data-ttu-id="27909-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27909-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="27909-472">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="27909-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="27909-473">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="27909-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="27909-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="27909-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="27909-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="27909-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="27909-476">媒体内容应用程序的分级设置。</span><span class="sxs-lookup"><span data-stu-id="27909-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="27909-477">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="27909-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="27909-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-478">messagesBlocked</span></span>|<span data-ttu-id="27909-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-479">Boolean</span></span>|<span data-ttu-id="27909-480">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="27909-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="27909-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="27909-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="27909-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-482">Boolean</span></span>|<span data-ttu-id="27909-483">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="27909-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="27909-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="27909-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-485">Boolean</span></span>|<span data-ttu-id="27909-486">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="27909-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="27909-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="27909-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="27909-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-488">Boolean</span></span>|<span data-ttu-id="27909-489">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="27909-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="27909-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="27909-490">passcodeBlockModification</span></span>|<span data-ttu-id="27909-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-491">Boolean</span></span>|<span data-ttu-id="27909-492">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="27909-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="27909-493">passcodeBlockSimple</span></span>|<span data-ttu-id="27909-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-494">Boolean</span></span>|<span data-ttu-id="27909-495">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="27909-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="27909-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="27909-496">passcodeExpirationDays</span></span>|<span data-ttu-id="27909-497">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-497">Int32</span></span>|<span data-ttu-id="27909-498">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="27909-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="27909-499">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="27909-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="27909-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="27909-500">passcodeMinimumLength</span></span>|<span data-ttu-id="27909-501">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-501">Int32</span></span>|<span data-ttu-id="27909-502">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="27909-502">Minimum length of passcode.</span></span> <span data-ttu-id="27909-503">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="27909-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="27909-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="27909-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="27909-505">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-505">Int32</span></span>|<span data-ttu-id="27909-506">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="27909-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="27909-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="27909-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="27909-508">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-508">Int32</span></span>|<span data-ttu-id="27909-509">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="27909-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="27909-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="27909-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="27909-511">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-511">Int32</span></span>|<span data-ttu-id="27909-512">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="27909-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="27909-513">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="27909-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="27909-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="27909-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="27909-515">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-515">Int32</span></span>|<span data-ttu-id="27909-516">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="27909-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="27909-517">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="27909-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="27909-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="27909-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="27909-519">Int32</span><span class="sxs-lookup"><span data-stu-id="27909-519">Int32</span></span>|<span data-ttu-id="27909-520">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="27909-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="27909-521">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="27909-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="27909-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="27909-522">passcodeRequiredType</span></span>|[<span data-ttu-id="27909-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="27909-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="27909-524">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="27909-524">Type of passcode that is required.</span></span> <span data-ttu-id="27909-525">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="27909-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="27909-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="27909-526">passcodeRequired</span></span>|<span data-ttu-id="27909-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-527">Boolean</span></span>|<span data-ttu-id="27909-528">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="27909-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="27909-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-529">podcastsBlocked</span></span>|<span data-ttu-id="27909-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-530">Boolean</span></span>|<span data-ttu-id="27909-531">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="27909-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="27909-532">safariBlockAutofill</span></span>|<span data-ttu-id="27909-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-533">Boolean</span></span>|<span data-ttu-id="27909-534">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="27909-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="27909-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="27909-535">safariBlockJavaScript</span></span>|<span data-ttu-id="27909-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-536">Boolean</span></span>|<span data-ttu-id="27909-537">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="27909-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="27909-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="27909-538">safariBlockPopups</span></span>|<span data-ttu-id="27909-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-539">Boolean</span></span>|<span data-ttu-id="27909-540">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="27909-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="27909-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-541">safariBlocked</span></span>|<span data-ttu-id="27909-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-542">Boolean</span></span>|<span data-ttu-id="27909-543">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="27909-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="27909-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="27909-544">safariCookieSettings</span></span>|[<span data-ttu-id="27909-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="27909-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="27909-546">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="27909-546">Cookie settings for Safari.</span></span> <span data-ttu-id="27909-547">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="27909-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="27909-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="27909-548">safariManagedDomains</span></span>|<span data-ttu-id="27909-549">String 集合</span><span class="sxs-lookup"><span data-stu-id="27909-549">String collection</span></span>|<span data-ttu-id="27909-550">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="27909-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="27909-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="27909-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="27909-552">String 集合</span><span class="sxs-lookup"><span data-stu-id="27909-552">String collection</span></span>|<span data-ttu-id="27909-553">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="27909-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="27909-554">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="27909-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="27909-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="27909-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-556">Boolean</span></span>|<span data-ttu-id="27909-557">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="27909-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="27909-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-558">screenCaptureBlocked</span></span>|<span data-ttu-id="27909-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-559">Boolean</span></span>|<span data-ttu-id="27909-560">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="27909-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="27909-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-561">siriBlocked</span></span>|<span data-ttu-id="27909-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-562">Boolean</span></span>|<span data-ttu-id="27909-563">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="27909-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="27909-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="27909-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="27909-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-565">Boolean</span></span>|<span data-ttu-id="27909-566">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="27909-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="27909-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="27909-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="27909-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-568">Boolean</span></span>|<span data-ttu-id="27909-569">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="27909-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="27909-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="27909-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="27909-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-571">Boolean</span></span>|<span data-ttu-id="27909-572">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="27909-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="27909-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="27909-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="27909-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-574">Boolean</span></span>|<span data-ttu-id="27909-575">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="27909-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="27909-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-576">voiceDialingBlocked</span></span>|<span data-ttu-id="27909-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-577">Boolean</span></span>|<span data-ttu-id="27909-578">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="27909-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="27909-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="27909-579">wallpaperBlockModification</span></span>|<span data-ttu-id="27909-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-580">Boolean</span></span>|<span data-ttu-id="27909-581">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="27909-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="27909-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="27909-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="27909-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="27909-583">Boolean</span></span>|<span data-ttu-id="27909-584">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="27909-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="27909-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="27909-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="27909-586">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-586">Boolean</span></span>|<span data-ttu-id="27909-587">指示是否通过课堂非托管课程中注册学生将权限时，从请求教师尝试保留课程 (iOS 11.3 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="27909-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="27909-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="27909-589">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-589">Boolean</span></span>|<span data-ttu-id="27909-590">指示阻止 iCloud 钥匙链同步。</span><span class="sxs-lookup"><span data-stu-id="27909-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="27909-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="27909-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="27909-592">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-592">Boolean</span></span>|<span data-ttu-id="27909-593">指示无线 PKI 更新已被阻止。</span><span class="sxs-lookup"><span data-stu-id="27909-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="27909-594">设置此限制 false 不会禁用 CRL 和 OCSP 检查 (iOS 7.0 和更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="27909-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="27909-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="27909-596">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-596">Boolean</span></span>|<span data-ttu-id="27909-597">指示是否有限 ad 跟踪。(iOS 7.0 和更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="27909-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="27909-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="27909-599">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-599">Boolean</span></span>|<span data-ttu-id="27909-600">指示企业书籍备份被阻止。</span><span class="sxs-lookup"><span data-stu-id="27909-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="27909-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="27909-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="27909-602">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-602">Boolean</span></span>|<span data-ttu-id="27909-603">指示阻止的企业簿说明并突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="27909-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="27909-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="27909-604">airPrintBlocked</span></span>|<span data-ttu-id="27909-605">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-605">Boolean</span></span>|<span data-ttu-id="27909-606">指示 AirPrint 阻止 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="27909-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="27909-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="27909-608">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-608">Boolean</span></span>|<span data-ttu-id="27909-609">指示钥匙链存储的用户名和密码 Airprint 阻止 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="27909-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="27909-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="27909-611">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-611">Boolean</span></span>|<span data-ttu-id="27909-612">指示受信任的证书是否需要 TLS 打印通信 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="27909-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="27909-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="27909-614">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-614">Boolean</span></span>|<span data-ttu-id="27909-615">指示阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="27909-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="27909-616">这样可以防止在从网络流量 (iOS 11.0 及更高版本) 的网络钓鱼的虚假 AirPrint 蓝牙信号。</span><span class="sxs-lookup"><span data-stu-id="27909-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="27909-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="27909-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="27909-618">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-618">Boolean</span></span>|<span data-ttu-id="27909-619">指示从设备的系统应用程序删除被阻止监管设备 (iOS 11.0 及更高版本) 上。</span><span class="sxs-lookup"><span data-stu-id="27909-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="27909-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="27909-620">vpnBlockCreation</span></span>|<span data-ttu-id="27909-621">布尔</span><span class="sxs-lookup"><span data-stu-id="27909-621">Boolean</span></span>|<span data-ttu-id="27909-622">指示创建 VPN 配置为阻止 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="27909-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="27909-623">响应</span><span class="sxs-lookup"><span data-stu-id="27909-623">Response</span></span>
<span data-ttu-id="27909-624">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27909-624">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27909-625">示例</span><span class="sxs-lookup"><span data-stu-id="27909-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="27909-626">请求</span><span class="sxs-lookup"><span data-stu-id="27909-626">Request</span></span>
<span data-ttu-id="27909-627">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27909-627">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8428

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "vpnBlockCreation": true
}
```

### <a name="response"></a><span data-ttu-id="27909-628">响应</span><span class="sxs-lookup"><span data-stu-id="27909-628">Response</span></span>
<span data-ttu-id="27909-p132">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27909-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8604

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
  "vpnBlockCreation": true
}
```





