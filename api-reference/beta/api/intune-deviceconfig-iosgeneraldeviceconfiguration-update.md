---
title: 更新 iosGeneralDeviceConfiguration
description: 更新 iosGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 590fa8264500fbbf10668a397fafd02247d1eb6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936891"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="1650f-103">更新 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1650f-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1650f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1650f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1650f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1650f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1650f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1650f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1650f-107">更新 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1650f-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1650f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1650f-108">Prerequisites</span></span>
<span data-ttu-id="1650f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1650f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1650f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1650f-111">Permission type</span></span>|<span data-ttu-id="1650f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1650f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1650f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1650f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1650f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1650f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1650f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1650f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1650f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1650f-116">Not supported.</span></span>|
|<span data-ttu-id="1650f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1650f-117">Application</span></span>|<span data-ttu-id="1650f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1650f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1650f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1650f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1650f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1650f-120">Request headers</span></span>
|<span data-ttu-id="1650f-121">标头</span><span class="sxs-lookup"><span data-stu-id="1650f-121">Header</span></span>|<span data-ttu-id="1650f-122">值</span><span class="sxs-lookup"><span data-stu-id="1650f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1650f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1650f-123">Authorization</span></span>|<span data-ttu-id="1650f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1650f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1650f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1650f-125">Accept</span></span>|<span data-ttu-id="1650f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1650f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1650f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1650f-127">Request body</span></span>
<span data-ttu-id="1650f-128">在请求正文中，提供 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1650f-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1650f-129">下表显示创建 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1650f-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1650f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1650f-130">Property</span></span>|<span data-ttu-id="1650f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1650f-131">Type</span></span>|<span data-ttu-id="1650f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1650f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1650f-133">id</span><span class="sxs-lookup"><span data-stu-id="1650f-133">id</span></span>|<span data-ttu-id="1650f-134">String</span><span class="sxs-lookup"><span data-stu-id="1650f-134">String</span></span>|<span data-ttu-id="1650f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1650f-135">Key of the entity.</span></span> <span data-ttu-id="1650f-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1650f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1650f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1650f-138">DateTimeOffset</span></span>|<span data-ttu-id="1650f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1650f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1650f-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1650f-141">roleScopeTagIds</span></span>|<span data-ttu-id="1650f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-142">String collection</span></span>|<span data-ttu-id="1650f-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1650f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1650f-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1650f-145">supportsScopeTags</span></span>|<span data-ttu-id="1650f-146">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-146">Boolean</span></span>|<span data-ttu-id="1650f-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="1650f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1650f-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1650f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1650f-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="1650f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1650f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1650f-150">This property is read-only.</span></span> <span data-ttu-id="1650f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1650f-152">createdDateTime</span></span>|<span data-ttu-id="1650f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1650f-153">DateTimeOffset</span></span>|<span data-ttu-id="1650f-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1650f-154">DateTime the object was created.</span></span> <span data-ttu-id="1650f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-156">description</span><span class="sxs-lookup"><span data-stu-id="1650f-156">description</span></span>|<span data-ttu-id="1650f-157">String</span><span class="sxs-lookup"><span data-stu-id="1650f-157">String</span></span>|<span data-ttu-id="1650f-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1650f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1650f-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1650f-160">displayName</span></span>|<span data-ttu-id="1650f-161">String</span><span class="sxs-lookup"><span data-stu-id="1650f-161">String</span></span>|<span data-ttu-id="1650f-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1650f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1650f-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-164">version</span><span class="sxs-lookup"><span data-stu-id="1650f-164">version</span></span>|<span data-ttu-id="1650f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-165">Int32</span></span>|<span data-ttu-id="1650f-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1650f-166">Version of the device configuration.</span></span> <span data-ttu-id="1650f-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1650f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1650f-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="1650f-168">accountBlockModification</span></span>|<span data-ttu-id="1650f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-169">Boolean</span></span>|<span data-ttu-id="1650f-170">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="1650f-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="1650f-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="1650f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-172">Boolean</span></span>|<span data-ttu-id="1650f-173">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="1650f-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="1650f-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-174">airDropBlocked</span></span>|<span data-ttu-id="1650f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-175">Boolean</span></span>|<span data-ttu-id="1650f-176">指示设备处于监督模式时是否允许使用 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="1650f-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="1650f-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="1650f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-178">Boolean</span></span>|<span data-ttu-id="1650f-179">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="1650f-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="1650f-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-181">Boolean</span></span>|<span data-ttu-id="1650f-182">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="1650f-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="1650f-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="1650f-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="1650f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-184">Boolean</span></span>|<span data-ttu-id="1650f-185">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="1650f-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="1650f-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-187">Boolean</span></span>|<span data-ttu-id="1650f-188">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="1650f-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-189">appleNewsBlocked</span></span>|<span data-ttu-id="1650f-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-190">Boolean</span></span>|<span data-ttu-id="1650f-191">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="1650f-192">appsSingleAppModeList</span></span>|<span data-ttu-id="1650f-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1650f-194">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="1650f-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="1650f-195">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="1650f-195">Supervised only.</span></span> <span data-ttu-id="1650f-196">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="1650f-196">iOS 7.0 and later.</span></span> <span data-ttu-id="1650f-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1650f-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1650f-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="1650f-198">appsVisibilityList</span></span>|<span data-ttu-id="1650f-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1650f-200">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="1650f-201">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="1650f-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1650f-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="1650f-202">appsVisibilityListType</span></span>|[<span data-ttu-id="1650f-203">appListType</span><span class="sxs-lookup"><span data-stu-id="1650f-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1650f-204">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="1650f-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="1650f-205">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="1650f-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1650f-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="1650f-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="1650f-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-207">Boolean</span></span>|<span data-ttu-id="1650f-208">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-209">appStoreBlocked</span></span>|<span data-ttu-id="1650f-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-210">Boolean</span></span>|<span data-ttu-id="1650f-211">指示是否阻止用户使用应用商店。</span><span class="sxs-lookup"><span data-stu-id="1650f-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="1650f-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="1650f-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="1650f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-213">Boolean</span></span>|<span data-ttu-id="1650f-214">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="1650f-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="1650f-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1650f-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="1650f-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-216">Boolean</span></span>|<span data-ttu-id="1650f-217">指示是否阻止应用商店应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="1650f-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="1650f-218">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="1650f-219">appStoreRequirePassword</span></span>|<span data-ttu-id="1650f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-220">Boolean</span></span>|<span data-ttu-id="1650f-221">指示使用应用商店时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="1650f-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="1650f-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="1650f-222">bluetoothBlockModification</span></span>|<span data-ttu-id="1650f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-223">Boolean</span></span>|<span data-ttu-id="1650f-224">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="1650f-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-225">cameraBlocked</span></span>|<span data-ttu-id="1650f-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-226">Boolean</span></span>|<span data-ttu-id="1650f-227">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="1650f-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="1650f-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="1650f-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="1650f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-229">Boolean</span></span>|<span data-ttu-id="1650f-230">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="1650f-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="1650f-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="1650f-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="1650f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-232">Boolean</span></span>|<span data-ttu-id="1650f-233">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="1650f-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="1650f-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="1650f-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="1650f-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-235">Boolean</span></span>|<span data-ttu-id="1650f-236">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="1650f-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="1650f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-238">Boolean</span></span>|<span data-ttu-id="1650f-239">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="1650f-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="1650f-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="1650f-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="1650f-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-241">Boolean</span></span>|<span data-ttu-id="1650f-242">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="1650f-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="1650f-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="1650f-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="1650f-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-244">Boolean</span></span>|<span data-ttu-id="1650f-245">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="1650f-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="1650f-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="1650f-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="1650f-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-247">Boolean</span></span>|<span data-ttu-id="1650f-248">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1650f-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="1650f-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="1650f-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-250">Boolean</span></span>|<span data-ttu-id="1650f-251">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="1650f-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1650f-252">compliantAppsList</span></span>|<span data-ttu-id="1650f-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1650f-254">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="1650f-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1650f-255">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="1650f-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1650f-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1650f-256">compliantAppListType</span></span>|[<span data-ttu-id="1650f-257">appListType</span><span class="sxs-lookup"><span data-stu-id="1650f-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1650f-258">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="1650f-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="1650f-259">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="1650f-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1650f-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="1650f-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="1650f-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-261">Boolean</span></span>|<span data-ttu-id="1650f-262">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="1650f-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-263">definitionLookupBlocked</span></span>|<span data-ttu-id="1650f-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-264">Boolean</span></span>|<span data-ttu-id="1650f-265">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="1650f-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="1650f-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="1650f-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-267">Boolean</span></span>|<span data-ttu-id="1650f-268">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="1650f-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="1650f-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-270">Boolean</span></span>|<span data-ttu-id="1650f-271">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="1650f-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="1650f-272">deviceBlockNameModification</span></span>|<span data-ttu-id="1650f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-273">Boolean</span></span>|<span data-ttu-id="1650f-274">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="1650f-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="1650f-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-276">Boolean</span></span>|<span data-ttu-id="1650f-277">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="1650f-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="1650f-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="1650f-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="1650f-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-279">Boolean</span></span>|<span data-ttu-id="1650f-280">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="1650f-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="1650f-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="1650f-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-282">Boolean</span></span>|<span data-ttu-id="1650f-283">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="1650f-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="1650f-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="1650f-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="1650f-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-285">Boolean</span></span>|<span data-ttu-id="1650f-286">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="1650f-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="1650f-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="1650f-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="1650f-288">String 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-288">String collection</span></span>|<span data-ttu-id="1650f-289">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="1650f-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="1650f-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="1650f-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="1650f-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-291">Boolean</span></span>|<span data-ttu-id="1650f-292">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="1650f-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="1650f-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="1650f-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="1650f-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-294">Boolean</span></span>|<span data-ttu-id="1650f-295">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="1650f-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-296">faceTimeBlocked</span></span>|<span data-ttu-id="1650f-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-297">Boolean</span></span>|<span data-ttu-id="1650f-298">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="1650f-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="1650f-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="1650f-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-300">Boolean</span></span>|<span data-ttu-id="1650f-301">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="1650f-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="1650f-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="1650f-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-303">Boolean</span></span>|<span data-ttu-id="1650f-304">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="1650f-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="1650f-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="1650f-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="1650f-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-306">Boolean</span></span>|<span data-ttu-id="1650f-307">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="1650f-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="1650f-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-308">gameCenterBlocked</span></span>|<span data-ttu-id="1650f-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-309">Boolean</span></span>|<span data-ttu-id="1650f-310">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="1650f-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-311">hostPairingBlocked</span></span>|<span data-ttu-id="1650f-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-312">Boolean</span></span>|<span data-ttu-id="1650f-313">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="1650f-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="1650f-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-315">Boolean</span></span>|<span data-ttu-id="1650f-316">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="1650f-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="1650f-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="1650f-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-318">Boolean</span></span>|<span data-ttu-id="1650f-319">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="1650f-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="1650f-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="1650f-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="1650f-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-321">Boolean</span></span>|<span data-ttu-id="1650f-322">指示是否阻止用户在另一个 iOS 或 MacOS 设备上继续从事在 iOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="1650f-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="1650f-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="1650f-323">iCloudBlockBackup</span></span>|<span data-ttu-id="1650f-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-324">Boolean</span></span>|<span data-ttu-id="1650f-325">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="1650f-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="1650f-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="1650f-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="1650f-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-327">Boolean</span></span>|<span data-ttu-id="1650f-328">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="1650f-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="1650f-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="1650f-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="1650f-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-330">Boolean</span></span>|<span data-ttu-id="1650f-331">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="1650f-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="1650f-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="1650f-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="1650f-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-333">Boolean</span></span>|<span data-ttu-id="1650f-334">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="1650f-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="1650f-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="1650f-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="1650f-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-336">Boolean</span></span>|<span data-ttu-id="1650f-337">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="1650f-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="1650f-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="1650f-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="1650f-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-339">Boolean</span></span>|<span data-ttu-id="1650f-340">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="1650f-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="1650f-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="1650f-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="1650f-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-342">Boolean</span></span>|<span data-ttu-id="1650f-343">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="1650f-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="1650f-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="1650f-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="1650f-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-345">Boolean</span></span>|<span data-ttu-id="1650f-346">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="1650f-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="1650f-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="1650f-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="1650f-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-348">Boolean</span></span>|<span data-ttu-id="1650f-349">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="1650f-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="1650f-350">iTunesBlockRadio</span></span>|<span data-ttu-id="1650f-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-351">Boolean</span></span>|<span data-ttu-id="1650f-352">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1650f-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="1650f-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="1650f-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-354">Boolean</span></span>|<span data-ttu-id="1650f-355">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1650f-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="1650f-356">keyboardBlockDictation</span></span>|<span data-ttu-id="1650f-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-357">Boolean</span></span>|<span data-ttu-id="1650f-358">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="1650f-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="1650f-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="1650f-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-360">Boolean</span></span>|<span data-ttu-id="1650f-361">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1650f-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="1650f-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="1650f-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-363">Boolean</span></span>|<span data-ttu-id="1650f-364">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="1650f-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="1650f-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-366">Boolean</span></span>|<span data-ttu-id="1650f-367">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1650f-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="1650f-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="1650f-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-369">Boolean</span></span>|<span data-ttu-id="1650f-370">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="1650f-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="1650f-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-372">Boolean</span></span>|<span data-ttu-id="1650f-373">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="1650f-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="1650f-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-375">Boolean</span></span>|<span data-ttu-id="1650f-376">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="1650f-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="1650f-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-378">Boolean</span></span>|<span data-ttu-id="1650f-379">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="1650f-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="1650f-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-381">Boolean</span></span>|<span data-ttu-id="1650f-382">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="1650f-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="1650f-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="1650f-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-384">Boolean</span></span>|<span data-ttu-id="1650f-385">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="1650f-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="1650f-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="1650f-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-387">Boolean</span></span>|<span data-ttu-id="1650f-388">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="1650f-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="1650f-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="1650f-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-390">Boolean</span></span>|<span data-ttu-id="1650f-391">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="1650f-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="1650f-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-393">Boolean</span></span>|<span data-ttu-id="1650f-394">指示在展台模式下是否允许访问语音过滤设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="1650f-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="1650f-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-396">Boolean</span></span>|<span data-ttu-id="1650f-397">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="1650f-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="1650f-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="1650f-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-399">Boolean</span></span>|<span data-ttu-id="1650f-400">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="1650f-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="1650f-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="1650f-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-402">Boolean</span></span>|<span data-ttu-id="1650f-403">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1650f-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="1650f-405">String</span><span class="sxs-lookup"><span data-stu-id="1650f-405">String</span></span>|<span data-ttu-id="1650f-406">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="1650f-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="1650f-407">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="1650f-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="1650f-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="1650f-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="1650f-409">字符串</span><span class="sxs-lookup"><span data-stu-id="1650f-409">String</span></span>|<span data-ttu-id="1650f-410">用于展台模式内置应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="1650f-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="1650f-411">未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="1650f-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="1650f-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="1650f-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="1650f-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-413">Boolean</span></span>|<span data-ttu-id="1650f-414">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="1650f-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="1650f-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="1650f-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-416">Boolean</span></span>|<span data-ttu-id="1650f-417">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="1650f-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="1650f-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="1650f-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-419">Boolean</span></span>|<span data-ttu-id="1650f-420">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="1650f-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="1650f-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="1650f-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-422">Boolean</span></span>|<span data-ttu-id="1650f-423">指示在展台模式下是否要求语音过滤。</span><span class="sxs-lookup"><span data-stu-id="1650f-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="1650f-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="1650f-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-425">Boolean</span></span>|<span data-ttu-id="1650f-426">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="1650f-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="1650f-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="1650f-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="1650f-428">String</span><span class="sxs-lookup"><span data-stu-id="1650f-428">String</span></span>|<span data-ttu-id="1650f-429">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="1650f-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="1650f-430">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="1650f-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="1650f-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="1650f-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="1650f-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-432">Boolean</span></span>|<span data-ttu-id="1650f-433">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="1650f-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="1650f-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="1650f-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="1650f-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-435">Boolean</span></span>|<span data-ttu-id="1650f-436">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="1650f-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="1650f-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="1650f-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="1650f-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-438">Boolean</span></span>|<span data-ttu-id="1650f-439">指示设备处于锁定状态时是否阻止用户使用 passbook。</span><span class="sxs-lookup"><span data-stu-id="1650f-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="1650f-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="1650f-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="1650f-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-441">Boolean</span></span>|<span data-ttu-id="1650f-442">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="1650f-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="1650f-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="1650f-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="1650f-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="1650f-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="1650f-445">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="1650f-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1650f-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="1650f-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1650f-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="1650f-448">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="1650f-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1650f-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="1650f-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1650f-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="1650f-451">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="1650f-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1650f-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="1650f-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1650f-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="1650f-454">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="1650f-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1650f-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="1650f-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1650f-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="1650f-457">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="1650f-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1650f-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="1650f-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1650f-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="1650f-460">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="1650f-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1650f-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="1650f-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1650f-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="1650f-463">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="1650f-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="1650f-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="1650f-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="1650f-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="1650f-466">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="1650f-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1650f-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="1650f-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1650f-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="1650f-469">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="1650f-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="1650f-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="1650f-470">networkUsageRules</span></span>|<span data-ttu-id="1650f-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="1650f-472">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="1650f-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="1650f-473">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="1650f-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="1650f-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="1650f-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="1650f-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="1650f-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="1650f-476">媒体内容应用程序的分级设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="1650f-477">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="1650f-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="1650f-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-478">messagesBlocked</span></span>|<span data-ttu-id="1650f-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-479">Boolean</span></span>|<span data-ttu-id="1650f-480">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="1650f-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="1650f-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="1650f-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="1650f-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-482">Boolean</span></span>|<span data-ttu-id="1650f-483">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1650f-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1650f-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="1650f-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-485">Boolean</span></span>|<span data-ttu-id="1650f-486">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="1650f-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1650f-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="1650f-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="1650f-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-488">Boolean</span></span>|<span data-ttu-id="1650f-489">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="1650f-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="1650f-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="1650f-490">passcodeBlockModification</span></span>|<span data-ttu-id="1650f-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-491">Boolean</span></span>|<span data-ttu-id="1650f-492">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1650f-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1650f-493">passcodeBlockSimple</span></span>|<span data-ttu-id="1650f-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-494">Boolean</span></span>|<span data-ttu-id="1650f-495">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="1650f-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="1650f-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1650f-496">passcodeExpirationDays</span></span>|<span data-ttu-id="1650f-497">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-497">Int32</span></span>|<span data-ttu-id="1650f-498">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="1650f-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="1650f-499">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="1650f-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="1650f-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1650f-500">passcodeMinimumLength</span></span>|<span data-ttu-id="1650f-501">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-501">Int32</span></span>|<span data-ttu-id="1650f-502">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="1650f-502">Minimum length of passcode.</span></span> <span data-ttu-id="1650f-503">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="1650f-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="1650f-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1650f-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1650f-505">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-505">Int32</span></span>|<span data-ttu-id="1650f-506">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="1650f-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="1650f-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1650f-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1650f-508">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-508">Int32</span></span>|<span data-ttu-id="1650f-509">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="1650f-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1650f-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1650f-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="1650f-511">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-511">Int32</span></span>|<span data-ttu-id="1650f-512">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="1650f-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="1650f-513">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="1650f-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="1650f-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="1650f-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="1650f-515">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-515">Int32</span></span>|<span data-ttu-id="1650f-516">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="1650f-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="1650f-517">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="1650f-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1650f-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="1650f-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="1650f-519">Int32</span><span class="sxs-lookup"><span data-stu-id="1650f-519">Int32</span></span>|<span data-ttu-id="1650f-520">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="1650f-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="1650f-521">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="1650f-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1650f-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="1650f-522">passcodeRequiredType</span></span>|[<span data-ttu-id="1650f-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1650f-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1650f-524">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="1650f-524">Type of passcode that is required.</span></span> <span data-ttu-id="1650f-525">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="1650f-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1650f-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="1650f-526">passcodeRequired</span></span>|<span data-ttu-id="1650f-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-527">Boolean</span></span>|<span data-ttu-id="1650f-528">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="1650f-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="1650f-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-529">podcastsBlocked</span></span>|<span data-ttu-id="1650f-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-530">Boolean</span></span>|<span data-ttu-id="1650f-531">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="1650f-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="1650f-532">safariBlockAutofill</span></span>|<span data-ttu-id="1650f-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-533">Boolean</span></span>|<span data-ttu-id="1650f-534">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="1650f-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="1650f-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="1650f-535">safariBlockJavaScript</span></span>|<span data-ttu-id="1650f-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-536">Boolean</span></span>|<span data-ttu-id="1650f-537">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="1650f-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="1650f-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="1650f-538">safariBlockPopups</span></span>|<span data-ttu-id="1650f-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-539">Boolean</span></span>|<span data-ttu-id="1650f-540">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="1650f-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="1650f-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-541">safariBlocked</span></span>|<span data-ttu-id="1650f-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-542">Boolean</span></span>|<span data-ttu-id="1650f-543">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="1650f-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="1650f-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-544">safariCookieSettings</span></span>|[<span data-ttu-id="1650f-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="1650f-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="1650f-546">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="1650f-546">Cookie settings for Safari.</span></span> <span data-ttu-id="1650f-547">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="1650f-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="1650f-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="1650f-548">safariManagedDomains</span></span>|<span data-ttu-id="1650f-549">String 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-549">String collection</span></span>|<span data-ttu-id="1650f-550">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="1650f-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="1650f-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="1650f-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="1650f-552">String 集合</span><span class="sxs-lookup"><span data-stu-id="1650f-552">String collection</span></span>|<span data-ttu-id="1650f-553">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="1650f-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="1650f-554">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1650f-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="1650f-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="1650f-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-556">Boolean</span></span>|<span data-ttu-id="1650f-557">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="1650f-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="1650f-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-558">screenCaptureBlocked</span></span>|<span data-ttu-id="1650f-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-559">Boolean</span></span>|<span data-ttu-id="1650f-560">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="1650f-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="1650f-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-561">siriBlocked</span></span>|<span data-ttu-id="1650f-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-562">Boolean</span></span>|<span data-ttu-id="1650f-563">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="1650f-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="1650f-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="1650f-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="1650f-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-565">Boolean</span></span>|<span data-ttu-id="1650f-566">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="1650f-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="1650f-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="1650f-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="1650f-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-568">Boolean</span></span>|<span data-ttu-id="1650f-569">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="1650f-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="1650f-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="1650f-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="1650f-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-571">Boolean</span></span>|<span data-ttu-id="1650f-572">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="1650f-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="1650f-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="1650f-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="1650f-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-574">Boolean</span></span>|<span data-ttu-id="1650f-575">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="1650f-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="1650f-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-576">voiceDialingBlocked</span></span>|<span data-ttu-id="1650f-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-577">Boolean</span></span>|<span data-ttu-id="1650f-578">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="1650f-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="1650f-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="1650f-579">wallpaperBlockModification</span></span>|<span data-ttu-id="1650f-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-580">Boolean</span></span>|<span data-ttu-id="1650f-581">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="1650f-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="1650f-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="1650f-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="1650f-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="1650f-583">Boolean</span></span>|<span data-ttu-id="1650f-584">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="1650f-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1650f-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="1650f-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="1650f-586">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-586">Boolean</span></span>|<span data-ttu-id="1650f-587">指示是否通过课堂非托管课程中注册学生将权限时，从请求教师尝试保留课程 (iOS 11.3 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="1650f-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="1650f-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="1650f-589">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-589">Boolean</span></span>|<span data-ttu-id="1650f-590">指示阻止 iCloud 钥匙链同步。</span><span class="sxs-lookup"><span data-stu-id="1650f-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="1650f-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="1650f-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="1650f-592">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-592">Boolean</span></span>|<span data-ttu-id="1650f-593">指示无线 PKI 更新已被阻止。</span><span class="sxs-lookup"><span data-stu-id="1650f-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="1650f-594">设置此限制 false 不会禁用 CRL 和 OCSP 检查 (iOS 7.0 和更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="1650f-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="1650f-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="1650f-596">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-596">Boolean</span></span>|<span data-ttu-id="1650f-597">指示是否有限 ad 跟踪。(iOS 7.0 和更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="1650f-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="1650f-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="1650f-599">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-599">Boolean</span></span>|<span data-ttu-id="1650f-600">指示企业书籍备份被阻止。</span><span class="sxs-lookup"><span data-stu-id="1650f-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="1650f-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="1650f-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="1650f-602">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-602">Boolean</span></span>|<span data-ttu-id="1650f-603">指示阻止的企业簿说明并突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="1650f-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="1650f-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="1650f-604">airPrintBlocked</span></span>|<span data-ttu-id="1650f-605">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-605">Boolean</span></span>|<span data-ttu-id="1650f-606">指示 AirPrint 阻止 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1650f-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="1650f-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="1650f-608">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-608">Boolean</span></span>|<span data-ttu-id="1650f-609">指示钥匙链存储的用户名和密码 Airprint 阻止 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1650f-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="1650f-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="1650f-611">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-611">Boolean</span></span>|<span data-ttu-id="1650f-612">指示受信任的证书是否需要 TLS 打印通信 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1650f-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="1650f-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="1650f-614">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-614">Boolean</span></span>|<span data-ttu-id="1650f-615">指示阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="1650f-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="1650f-616">这样可以防止在从网络流量 (iOS 11.0 及更高版本) 的网络钓鱼的虚假 AirPrint 蓝牙信号。</span><span class="sxs-lookup"><span data-stu-id="1650f-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1650f-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="1650f-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="1650f-618">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-618">Boolean</span></span>|<span data-ttu-id="1650f-619">指示从设备的系统应用程序删除被阻止监管设备 (iOS 11.0 及更高版本) 上。</span><span class="sxs-lookup"><span data-stu-id="1650f-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1650f-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="1650f-620">vpnBlockCreation</span></span>|<span data-ttu-id="1650f-621">布尔</span><span class="sxs-lookup"><span data-stu-id="1650f-621">Boolean</span></span>|<span data-ttu-id="1650f-622">指示创建 VPN 配置为阻止 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="1650f-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="1650f-623">响应</span><span class="sxs-lookup"><span data-stu-id="1650f-623">Response</span></span>
<span data-ttu-id="1650f-624">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1650f-624">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1650f-625">示例</span><span class="sxs-lookup"><span data-stu-id="1650f-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="1650f-626">请求</span><span class="sxs-lookup"><span data-stu-id="1650f-626">Request</span></span>
<span data-ttu-id="1650f-627">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1650f-627">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1650f-628">响应</span><span class="sxs-lookup"><span data-stu-id="1650f-628">Response</span></span>
<span data-ttu-id="1650f-p132">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1650f-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





