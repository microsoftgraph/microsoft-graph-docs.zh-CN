---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 773f4bc46c6e090ac9ff42c6865c3cf7b51611a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42750759"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="12723-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="12723-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="12723-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12723-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12723-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12723-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12723-106">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12723-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12723-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="12723-107">Prerequisites</span></span>
<span data-ttu-id="12723-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12723-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12723-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12723-110">Permission type</span></span>|<span data-ttu-id="12723-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12723-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12723-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12723-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12723-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12723-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12723-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12723-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12723-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12723-115">Not supported.</span></span>|
|<span data-ttu-id="12723-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12723-116">Application</span></span>|<span data-ttu-id="12723-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12723-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12723-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12723-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12723-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12723-119">Request headers</span></span>
|<span data-ttu-id="12723-120">标头</span><span class="sxs-lookup"><span data-stu-id="12723-120">Header</span></span>|<span data-ttu-id="12723-121">值</span><span class="sxs-lookup"><span data-stu-id="12723-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12723-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12723-122">Authorization</span></span>|<span data-ttu-id="12723-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12723-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12723-124">接受</span><span class="sxs-lookup"><span data-stu-id="12723-124">Accept</span></span>|<span data-ttu-id="12723-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12723-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12723-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12723-126">Request body</span></span>
<span data-ttu-id="12723-127">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12723-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="12723-128">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12723-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="12723-129">属性</span><span class="sxs-lookup"><span data-stu-id="12723-129">Property</span></span>|<span data-ttu-id="12723-130">类型</span><span class="sxs-lookup"><span data-stu-id="12723-130">Type</span></span>|<span data-ttu-id="12723-131">说明</span><span class="sxs-lookup"><span data-stu-id="12723-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12723-132">id</span><span class="sxs-lookup"><span data-stu-id="12723-132">id</span></span>|<span data-ttu-id="12723-133">字符串</span><span class="sxs-lookup"><span data-stu-id="12723-133">String</span></span>|<span data-ttu-id="12723-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12723-134">Key of the entity.</span></span> <span data-ttu-id="12723-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12723-136">lastModifiedDateTime</span></span>|<span data-ttu-id="12723-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12723-137">DateTimeOffset</span></span>|<span data-ttu-id="12723-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="12723-138">DateTime the object was last modified.</span></span> <span data-ttu-id="12723-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12723-140">roleScopeTagIds</span></span>|<span data-ttu-id="12723-141">String collection</span><span class="sxs-lookup"><span data-stu-id="12723-141">String collection</span></span>|<span data-ttu-id="12723-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="12723-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12723-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="12723-144">supportsScopeTags</span></span>|<span data-ttu-id="12723-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-145">Boolean</span></span>|<span data-ttu-id="12723-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="12723-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12723-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="12723-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12723-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="12723-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12723-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="12723-149">This property is read-only.</span></span> <span data-ttu-id="12723-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12723-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12723-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12723-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12723-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="12723-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12723-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12723-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12723-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12723-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12723-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="12723-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12723-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12723-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12723-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12723-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12723-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="12723-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12723-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12723-163">createdDateTime</span></span>|<span data-ttu-id="12723-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12723-164">DateTimeOffset</span></span>|<span data-ttu-id="12723-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="12723-165">DateTime the object was created.</span></span> <span data-ttu-id="12723-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-167">说明</span><span class="sxs-lookup"><span data-stu-id="12723-167">description</span></span>|<span data-ttu-id="12723-168">String</span><span class="sxs-lookup"><span data-stu-id="12723-168">String</span></span>|<span data-ttu-id="12723-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="12723-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12723-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-171">displayName</span><span class="sxs-lookup"><span data-stu-id="12723-171">displayName</span></span>|<span data-ttu-id="12723-172">String</span><span class="sxs-lookup"><span data-stu-id="12723-172">String</span></span>|<span data-ttu-id="12723-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="12723-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12723-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-175">version</span><span class="sxs-lookup"><span data-stu-id="12723-175">version</span></span>|<span data-ttu-id="12723-176">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-176">Int32</span></span>|<span data-ttu-id="12723-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="12723-177">Version of the device configuration.</span></span> <span data-ttu-id="12723-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12723-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12723-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="12723-179">accountBlockModification</span></span>|<span data-ttu-id="12723-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-180">Boolean</span></span>|<span data-ttu-id="12723-181">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="12723-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="12723-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="12723-183">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-183">Boolean</span></span>|<span data-ttu-id="12723-184">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="12723-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="12723-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-185">airDropBlocked</span></span>|<span data-ttu-id="12723-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-186">Boolean</span></span>|<span data-ttu-id="12723-187">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="12723-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="12723-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="12723-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-189">Boolean</span></span>|<span data-ttu-id="12723-190">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="12723-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="12723-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-192">Boolean</span></span>|<span data-ttu-id="12723-193">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="12723-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="12723-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="12723-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="12723-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-195">Boolean</span></span>|<span data-ttu-id="12723-196">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="12723-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="12723-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-198">Boolean</span></span>|<span data-ttu-id="12723-199">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="12723-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-200">appleNewsBlocked</span></span>|<span data-ttu-id="12723-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-201">Boolean</span></span>|<span data-ttu-id="12723-202">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="12723-203">appsSingleAppModeList</span></span>|<span data-ttu-id="12723-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12723-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="12723-205">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="12723-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="12723-206">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="12723-206">Supervised only.</span></span> <span data-ttu-id="12723-207">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-207">iOS 7.0 and later.</span></span> <span data-ttu-id="12723-208">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="12723-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="12723-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="12723-209">appsVisibilityList</span></span>|<span data-ttu-id="12723-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12723-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="12723-211">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="12723-212">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="12723-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="12723-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="12723-213">appsVisibilityListType</span></span>|[<span data-ttu-id="12723-214">appListType</span><span class="sxs-lookup"><span data-stu-id="12723-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="12723-215">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="12723-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="12723-216">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="12723-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="12723-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="12723-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="12723-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-218">Boolean</span></span>|<span data-ttu-id="12723-219">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-220">appStoreBlocked</span></span>|<span data-ttu-id="12723-221">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-221">Boolean</span></span>|<span data-ttu-id="12723-222">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="12723-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="12723-223">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="12723-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="12723-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-225">Boolean</span></span>|<span data-ttu-id="12723-226">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="12723-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="12723-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="12723-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="12723-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-228">Boolean</span></span>|<span data-ttu-id="12723-229">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="12723-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="12723-230">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="12723-231">appStoreRequirePassword</span></span>|<span data-ttu-id="12723-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-232">Boolean</span></span>|<span data-ttu-id="12723-233">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="12723-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="12723-234">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="12723-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="12723-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-235">Boolean</span></span>|<span data-ttu-id="12723-236">指示在 Safari 中的 autofilling 密码和信用卡信息之前是否强制进行用户身份验证，以及受监督的设备上的其他应用。</span><span class="sxs-lookup"><span data-stu-id="12723-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="12723-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="12723-237">bluetoothBlockModification</span></span>|<span data-ttu-id="12723-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-238">Boolean</span></span>|<span data-ttu-id="12723-239">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="12723-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-240">cameraBlocked</span></span>|<span data-ttu-id="12723-241">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-241">Boolean</span></span>|<span data-ttu-id="12723-242">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="12723-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="12723-243">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="12723-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="12723-245">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-245">Boolean</span></span>|<span data-ttu-id="12723-246">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="12723-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="12723-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="12723-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="12723-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-248">Boolean</span></span>|<span data-ttu-id="12723-249">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="12723-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="12723-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="12723-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="12723-251">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-251">Boolean</span></span>|<span data-ttu-id="12723-252">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="12723-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="12723-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="12723-254">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-254">Boolean</span></span>|<span data-ttu-id="12723-255">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="12723-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="12723-256">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="12723-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="12723-257">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-257">Boolean</span></span>|<span data-ttu-id="12723-258">指示是否允许用户在受监督的设备上更改移动电话计划的设置。</span><span class="sxs-lookup"><span data-stu-id="12723-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="12723-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="12723-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="12723-260">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-260">Boolean</span></span>|<span data-ttu-id="12723-261">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="12723-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="12723-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="12723-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="12723-263">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-263">Boolean</span></span>|<span data-ttu-id="12723-264">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="12723-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="12723-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="12723-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="12723-266">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-266">Boolean</span></span>|<span data-ttu-id="12723-267">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="12723-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="12723-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="12723-269">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-269">Boolean</span></span>|<span data-ttu-id="12723-270">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="12723-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-271">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="12723-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="12723-272">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-272">Boolean</span></span>|<span data-ttu-id="12723-273">指示设备处于监督模式时是否自动向教师的请求授予权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="12723-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-274">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="12723-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="12723-275">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-275">Boolean</span></span>|<span data-ttu-id="12723-276">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="12723-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="12723-277">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="12723-277">Supervised only.</span></span>|
|<span data-ttu-id="12723-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="12723-278">compliantAppsList</span></span>|<span data-ttu-id="12723-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12723-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="12723-280">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="12723-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="12723-281">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="12723-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="12723-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="12723-282">compliantAppListType</span></span>|[<span data-ttu-id="12723-283">appListType</span><span class="sxs-lookup"><span data-stu-id="12723-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="12723-284">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="12723-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="12723-285">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="12723-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="12723-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="12723-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="12723-287">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-287">Boolean</span></span>|<span data-ttu-id="12723-288">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="12723-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-289">definitionLookupBlocked</span></span>|<span data-ttu-id="12723-290">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-290">Boolean</span></span>|<span data-ttu-id="12723-291">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="12723-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="12723-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="12723-293">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-293">Boolean</span></span>|<span data-ttu-id="12723-294">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="12723-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="12723-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="12723-296">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-296">Boolean</span></span>|<span data-ttu-id="12723-297">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="12723-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="12723-298">deviceBlockNameModification</span></span>|<span data-ttu-id="12723-299">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-299">Boolean</span></span>|<span data-ttu-id="12723-300">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="12723-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="12723-302">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-302">Boolean</span></span>|<span data-ttu-id="12723-303">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="12723-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="12723-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="12723-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="12723-305">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-305">Boolean</span></span>|<span data-ttu-id="12723-306">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="12723-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="12723-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="12723-308">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-308">Boolean</span></span>|<span data-ttu-id="12723-309">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="12723-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="12723-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="12723-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="12723-311">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-311">Boolean</span></span>|<span data-ttu-id="12723-312">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="12723-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="12723-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="12723-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="12723-314">String 集合</span><span class="sxs-lookup"><span data-stu-id="12723-314">String collection</span></span>|<span data-ttu-id="12723-315">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="12723-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="12723-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="12723-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="12723-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-317">Boolean</span></span>|<span data-ttu-id="12723-318">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="12723-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="12723-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="12723-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="12723-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-320">Boolean</span></span>|<span data-ttu-id="12723-321">\[已\]弃用配置此设置并将值设置为 "true" 对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="12723-321">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="12723-322">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="12723-322">esimBlockModification</span></span>|<span data-ttu-id="12723-323">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-323">Boolean</span></span>|<span data-ttu-id="12723-324">指示是否允许在受监督的设备的 eSIM 卡上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="12723-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="12723-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-325">faceTimeBlocked</span></span>|<span data-ttu-id="12723-326">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-326">Boolean</span></span>|<span data-ttu-id="12723-327">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="12723-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="12723-328">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="12723-330">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-330">Boolean</span></span>|<span data-ttu-id="12723-331">指示设备处于监督模式时是否阻止更改以查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="12723-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="12723-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="12723-333">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-333">Boolean</span></span>|<span data-ttu-id="12723-334">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="12723-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="12723-335">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="12723-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="12723-337">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-337">Boolean</span></span>|<span data-ttu-id="12723-338">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="12723-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="12723-339">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-340">gameCenterBlocked</span></span>|<span data-ttu-id="12723-341">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-341">Boolean</span></span>|<span data-ttu-id="12723-342">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="12723-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-343">hostPairingBlocked</span></span>|<span data-ttu-id="12723-344">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-344">Boolean</span></span>|<span data-ttu-id="12723-345">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="12723-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="12723-347">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-347">Boolean</span></span>|<span data-ttu-id="12723-348">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="12723-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="12723-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="12723-350">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-350">Boolean</span></span>|<span data-ttu-id="12723-351">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="12723-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="12723-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="12723-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="12723-353">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-353">Boolean</span></span>|<span data-ttu-id="12723-354">指示是否阻止用户将其在 iOS 设备上启动的工作继续到另一个 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="12723-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="12723-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="12723-355">iCloudBlockBackup</span></span>|<span data-ttu-id="12723-356">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-356">Boolean</span></span>|<span data-ttu-id="12723-357">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="12723-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="12723-358">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="12723-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="12723-360">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-360">Boolean</span></span>|<span data-ttu-id="12723-361">指示是否阻止 iCloud 文档同步。需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="12723-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="12723-363">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-363">Boolean</span></span>|<span data-ttu-id="12723-364">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="12723-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="12723-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="12723-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="12723-366">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-366">Boolean</span></span>|<span data-ttu-id="12723-367">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="12723-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="12723-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="12723-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="12723-369">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-369">Boolean</span></span>|<span data-ttu-id="12723-370">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="12723-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="12723-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="12723-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="12723-372">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-372">Boolean</span></span>|<span data-ttu-id="12723-373">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="12723-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="12723-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="12723-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="12723-375">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-375">Boolean</span></span>|<span data-ttu-id="12723-376">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="12723-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="12723-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="12723-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="12723-378">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-378">Boolean</span></span>|<span data-ttu-id="12723-379">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="12723-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="12723-380">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="12723-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="12723-382">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-382">Boolean</span></span>|<span data-ttu-id="12723-383">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="12723-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="12723-384">iTunesBlockRadio</span></span>|<span data-ttu-id="12723-385">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-385">Boolean</span></span>|<span data-ttu-id="12723-386">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="12723-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="12723-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="12723-388">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-388">Boolean</span></span>|<span data-ttu-id="12723-389">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="12723-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="12723-390">keyboardBlockDictation</span></span>|<span data-ttu-id="12723-391">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-391">Boolean</span></span>|<span data-ttu-id="12723-392">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="12723-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="12723-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="12723-394">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-394">Boolean</span></span>|<span data-ttu-id="12723-395">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="12723-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="12723-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="12723-397">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-397">Boolean</span></span>|<span data-ttu-id="12723-398">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="12723-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="12723-400">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-400">Boolean</span></span>|<span data-ttu-id="12723-401">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="12723-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="12723-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="12723-403">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-403">Boolean</span></span>|<span data-ttu-id="12723-404">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="12723-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="12723-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="12723-406">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-406">Boolean</span></span>|<span data-ttu-id="12723-407">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="12723-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="12723-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="12723-409">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-409">Boolean</span></span>|<span data-ttu-id="12723-410">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="12723-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="12723-411">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="12723-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="12723-412">请改用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="12723-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="12723-413">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="12723-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="12723-414">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-414">Boolean</span></span>|<span data-ttu-id="12723-415">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="12723-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="12723-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="12723-417">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-417">Boolean</span></span>|<span data-ttu-id="12723-418">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="12723-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="12723-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="12723-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-420">Boolean</span></span>|<span data-ttu-id="12723-421">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="12723-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="12723-422">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="12723-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="12723-423">请改用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="12723-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="12723-424">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="12723-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="12723-425">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-425">Boolean</span></span>|<span data-ttu-id="12723-426">指示在展台模式下是否阻止使用铃声开关。</span><span class="sxs-lookup"><span data-stu-id="12723-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="12723-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="12723-428">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-428">Boolean</span></span>|<span data-ttu-id="12723-429">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="12723-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="12723-430">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="12723-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="12723-431">请改用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="12723-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="12723-432">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="12723-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="12723-433">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-433">Boolean</span></span>|<span data-ttu-id="12723-434">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="12723-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="12723-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="12723-436">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-436">Boolean</span></span>|<span data-ttu-id="12723-437">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="12723-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="12723-438">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="12723-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="12723-439">请改用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="12723-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="12723-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="12723-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="12723-441">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-441">Boolean</span></span>|<span data-ttu-id="12723-442">指示在展台模式下是否阻止使用 "睡眠" 按钮。</span><span class="sxs-lookup"><span data-stu-id="12723-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="12723-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="12723-444">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-444">Boolean</span></span>|<span data-ttu-id="12723-445">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="12723-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="12723-446">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="12723-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="12723-447">请改用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="12723-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="12723-448">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="12723-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="12723-449">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-449">Boolean</span></span>|<span data-ttu-id="12723-450">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="12723-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-451">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="12723-451">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="12723-452">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-452">Boolean</span></span>|<span data-ttu-id="12723-453">指示是否在展台模式下启用语音控制。</span><span class="sxs-lookup"><span data-stu-id="12723-453">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="12723-454">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="12723-454">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="12723-455">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-455">Boolean</span></span>|<span data-ttu-id="12723-456">指示是否允许用户在展台模式下切换语音控件。</span><span class="sxs-lookup"><span data-stu-id="12723-456">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="12723-457">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="12723-457">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="12723-458">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-458">Boolean</span></span>|<span data-ttu-id="12723-459">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="12723-459">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-460">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="12723-460">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="12723-461">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-461">Boolean</span></span>|<span data-ttu-id="12723-462">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="12723-462">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="12723-463">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="12723-463">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="12723-464">请改用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="12723-464">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="12723-465">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="12723-465">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="12723-466">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-466">Boolean</span></span>|<span data-ttu-id="12723-467">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="12723-467">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="12723-468">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="12723-468">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="12723-469">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-469">Boolean</span></span>|<span data-ttu-id="12723-470">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="12723-470">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-471">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="12723-471">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="12723-472">String</span><span class="sxs-lookup"><span data-stu-id="12723-472">String</span></span>|<span data-ttu-id="12723-473">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="12723-473">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="12723-474">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="12723-474">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="12723-475">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="12723-475">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="12723-476">String</span><span class="sxs-lookup"><span data-stu-id="12723-476">String</span></span>|<span data-ttu-id="12723-477">用于展台模式的内置应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="12723-477">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="12723-478">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="12723-478">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="12723-479">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="12723-479">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="12723-480">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-480">Boolean</span></span>|<span data-ttu-id="12723-481">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="12723-481">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-482">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="12723-482">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="12723-483">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-483">Boolean</span></span>|<span data-ttu-id="12723-484">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="12723-484">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-485">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="12723-485">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="12723-486">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-486">Boolean</span></span>|<span data-ttu-id="12723-487">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="12723-487">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-488">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="12723-488">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="12723-489">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-489">Boolean</span></span>|<span data-ttu-id="12723-490">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="12723-490">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-491">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="12723-491">kioskModeRequireZoom</span></span>|<span data-ttu-id="12723-492">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-492">Boolean</span></span>|<span data-ttu-id="12723-493">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="12723-493">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="12723-494">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="12723-494">kioskModeManagedAppId</span></span>|<span data-ttu-id="12723-495">String</span><span class="sxs-lookup"><span data-stu-id="12723-495">String</span></span>|<span data-ttu-id="12723-496">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="12723-496">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="12723-497">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="12723-497">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="12723-498">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="12723-498">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="12723-499">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-499">Boolean</span></span>|<span data-ttu-id="12723-500">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="12723-500">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="12723-501">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="12723-501">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="12723-502">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-502">Boolean</span></span>|<span data-ttu-id="12723-503">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="12723-503">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="12723-504">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="12723-504">lockScreenBlockPassbook</span></span>|<span data-ttu-id="12723-505">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-505">Boolean</span></span>|<span data-ttu-id="12723-506">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="12723-506">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="12723-507">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="12723-507">lockScreenBlockTodayView</span></span>|<span data-ttu-id="12723-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-508">Boolean</span></span>|<span data-ttu-id="12723-509">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="12723-509">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="12723-510">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="12723-510">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="12723-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="12723-511">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="12723-512">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-512">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="12723-513">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="12723-513">mediaContentRatingCanada</span></span>|[<span data-ttu-id="12723-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="12723-514">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="12723-515">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-515">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="12723-516">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="12723-516">mediaContentRatingFrance</span></span>|[<span data-ttu-id="12723-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="12723-517">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="12723-518">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-518">Media content rating settings for France</span></span>|
|<span data-ttu-id="12723-519">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="12723-519">mediaContentRatingGermany</span></span>|[<span data-ttu-id="12723-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="12723-520">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="12723-521">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-521">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="12723-522">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="12723-522">mediaContentRatingIreland</span></span>|[<span data-ttu-id="12723-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="12723-523">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="12723-524">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-524">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="12723-525">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="12723-525">mediaContentRatingJapan</span></span>|[<span data-ttu-id="12723-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="12723-526">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="12723-527">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-527">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="12723-528">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="12723-528">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="12723-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="12723-529">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="12723-530">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-530">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="12723-531">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="12723-531">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="12723-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="12723-532">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="12723-533">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-533">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="12723-534">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="12723-534">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="12723-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="12723-535">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="12723-536">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="12723-536">Media content rating settings for United States</span></span>|
|<span data-ttu-id="12723-537">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="12723-537">networkUsageRules</span></span>|<span data-ttu-id="12723-538">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12723-538">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="12723-539">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="12723-539">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="12723-540">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="12723-540">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="12723-541">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="12723-541">mediaContentRatingApps</span></span>|[<span data-ttu-id="12723-542">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="12723-542">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="12723-543">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="12723-543">Media content rating settings for Apps.</span></span> <span data-ttu-id="12723-544">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="12723-544">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="12723-545">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-545">messagesBlocked</span></span>|<span data-ttu-id="12723-546">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-546">Boolean</span></span>|<span data-ttu-id="12723-547">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="12723-547">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="12723-548">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="12723-548">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="12723-549">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-549">Boolean</span></span>|<span data-ttu-id="12723-550">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-550">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="12723-551">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="12723-551">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="12723-552">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-552">Boolean</span></span>|<span data-ttu-id="12723-553">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="12723-553">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="12723-554">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="12723-554">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="12723-555">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-555">Boolean</span></span>|<span data-ttu-id="12723-556">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="12723-556">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="12723-557">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="12723-557">passcodeBlockModification</span></span>|<span data-ttu-id="12723-558">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-558">Boolean</span></span>|<span data-ttu-id="12723-559">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-559">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="12723-560">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="12723-560">passcodeBlockSimple</span></span>|<span data-ttu-id="12723-561">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-561">Boolean</span></span>|<span data-ttu-id="12723-562">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="12723-562">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="12723-563">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="12723-563">passcodeExpirationDays</span></span>|<span data-ttu-id="12723-564">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-564">Int32</span></span>|<span data-ttu-id="12723-565">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="12723-565">Number of days before the passcode expires.</span></span> <span data-ttu-id="12723-566">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="12723-566">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="12723-567">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="12723-567">passcodeMinimumLength</span></span>|<span data-ttu-id="12723-568">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-568">Int32</span></span>|<span data-ttu-id="12723-569">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="12723-569">Minimum length of passcode.</span></span> <span data-ttu-id="12723-570">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="12723-570">Valid values 4 to 14</span></span>|
|<span data-ttu-id="12723-571">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="12723-571">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="12723-572">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-572">Int32</span></span>|<span data-ttu-id="12723-573">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="12723-573">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="12723-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="12723-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="12723-575">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-575">Int32</span></span>|<span data-ttu-id="12723-576">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="12723-576">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="12723-577">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="12723-577">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="12723-578">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-578">Int32</span></span>|<span data-ttu-id="12723-579">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="12723-579">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="12723-580">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="12723-580">Valid values 0 to 4</span></span>|
|<span data-ttu-id="12723-581">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="12723-581">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="12723-582">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-582">Int32</span></span>|<span data-ttu-id="12723-583">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="12723-583">Number of previous passcodes to block.</span></span> <span data-ttu-id="12723-584">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="12723-584">Valid values 1 to 24</span></span>|
|<span data-ttu-id="12723-585">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="12723-585">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="12723-586">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-586">Int32</span></span>|<span data-ttu-id="12723-587">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="12723-587">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="12723-588">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="12723-588">Valid values 4 to 11</span></span>|
|<span data-ttu-id="12723-589">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="12723-589">passcodeRequiredType</span></span>|[<span data-ttu-id="12723-590">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="12723-590">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="12723-591">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="12723-591">Type of passcode that is required.</span></span> <span data-ttu-id="12723-592">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="12723-592">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="12723-593">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="12723-593">passcodeRequired</span></span>|<span data-ttu-id="12723-594">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-594">Boolean</span></span>|<span data-ttu-id="12723-595">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="12723-595">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="12723-596">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-596">podcastsBlocked</span></span>|<span data-ttu-id="12723-597">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-597">Boolean</span></span>|<span data-ttu-id="12723-598">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-598">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="12723-599">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="12723-599">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="12723-600">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-600">Boolean</span></span>|<span data-ttu-id="12723-601">指示是否启用提示以在受监督的设备上安装附近设备。</span><span class="sxs-lookup"><span data-stu-id="12723-601">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="12723-602">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="12723-602">safariBlockAutofill</span></span>|<span data-ttu-id="12723-603">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-603">Boolean</span></span>|<span data-ttu-id="12723-604">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="12723-604">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="12723-605">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-605">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-606">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="12723-606">safariBlockJavaScript</span></span>|<span data-ttu-id="12723-607">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-607">Boolean</span></span>|<span data-ttu-id="12723-608">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="12723-608">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="12723-609">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="12723-609">safariBlockPopups</span></span>|<span data-ttu-id="12723-610">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-610">Boolean</span></span>|<span data-ttu-id="12723-611">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="12723-611">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="12723-612">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-612">safariBlocked</span></span>|<span data-ttu-id="12723-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-613">Boolean</span></span>|<span data-ttu-id="12723-614">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="12723-614">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="12723-615">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-615">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-616">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="12723-616">safariCookieSettings</span></span>|[<span data-ttu-id="12723-617">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="12723-617">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="12723-618">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="12723-618">Cookie settings for Safari.</span></span> <span data-ttu-id="12723-619">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="12723-619">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="12723-620">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="12723-620">safariManagedDomains</span></span>|<span data-ttu-id="12723-621">String collection</span><span class="sxs-lookup"><span data-stu-id="12723-621">String collection</span></span>|<span data-ttu-id="12723-622">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="12723-622">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="12723-623">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="12723-623">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="12723-624">String 集合</span><span class="sxs-lookup"><span data-stu-id="12723-624">String collection</span></span>|<span data-ttu-id="12723-625">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="12723-625">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="12723-626">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-626">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="12723-627">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="12723-627">safariRequireFraudWarning</span></span>|<span data-ttu-id="12723-628">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-628">Boolean</span></span>|<span data-ttu-id="12723-629">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="12723-629">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="12723-630">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-630">screenCaptureBlocked</span></span>|<span data-ttu-id="12723-631">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-631">Boolean</span></span>|<span data-ttu-id="12723-632">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="12723-632">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="12723-633">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-633">siriBlocked</span></span>|<span data-ttu-id="12723-634">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-634">Boolean</span></span>|<span data-ttu-id="12723-635">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="12723-635">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="12723-636">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="12723-636">siriBlockedWhenLocked</span></span>|<span data-ttu-id="12723-637">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-637">Boolean</span></span>|<span data-ttu-id="12723-638">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="12723-638">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="12723-639">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="12723-639">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="12723-640">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-640">Boolean</span></span>|<span data-ttu-id="12723-641">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="12723-641">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="12723-642">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="12723-642">siriRequireProfanityFilter</span></span>|<span data-ttu-id="12723-643">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-643">Boolean</span></span>|<span data-ttu-id="12723-644">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="12723-644">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="12723-645">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="12723-645">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="12723-646">Int32</span><span class="sxs-lookup"><span data-stu-id="12723-646">Int32</span></span>|<span data-ttu-id="12723-647">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="12723-647">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="12723-648">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="12723-648">Valid values 0 to 90</span></span>|
|<span data-ttu-id="12723-649">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="12723-649">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="12723-650">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-650">Boolean</span></span>|<span data-ttu-id="12723-651">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="12723-651">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-652">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="12723-652">spotlightBlockInternetResults</span></span>|<span data-ttu-id="12723-653">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-653">Boolean</span></span>|<span data-ttu-id="12723-654">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="12723-654">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="12723-655">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-655">voiceDialingBlocked</span></span>|<span data-ttu-id="12723-656">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-656">Boolean</span></span>|<span data-ttu-id="12723-657">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="12723-657">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="12723-658">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="12723-658">wallpaperBlockModification</span></span>|<span data-ttu-id="12723-659">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-659">Boolean</span></span>|<span data-ttu-id="12723-660">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-660">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="12723-661">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="12723-661">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="12723-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="12723-662">Boolean</span></span>|<span data-ttu-id="12723-663">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="12723-663">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="12723-664">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="12723-664">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="12723-665">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-665">Boolean</span></span>|<span data-ttu-id="12723-666">指示在非托管课程中通过教室注册的学生是否会在尝试离开该课程（iOS 11.3 及更高版本）时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="12723-666">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="12723-667">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="12723-667">keychainBlockCloudSync</span></span>|<span data-ttu-id="12723-668">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-668">Boolean</span></span>|<span data-ttu-id="12723-669">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="12723-669">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="12723-670">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-670">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-671">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="12723-671">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="12723-672">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-672">Boolean</span></span>|<span data-ttu-id="12723-673">指示是否阻止无线 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="12723-673">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="12723-674">将此限制设置为 false 不会禁用 CRL 和 OCSP 检查（iOS 7.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-674">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="12723-675">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="12723-675">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="12723-676">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-676">Boolean</span></span>|<span data-ttu-id="12723-677">指示广告跟踪是否受限制。（iOS 7.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-677">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="12723-678">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="12723-678">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="12723-679">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-679">Boolean</span></span>|<span data-ttu-id="12723-680">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="12723-680">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="12723-681">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="12723-681">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="12723-682">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-682">Boolean</span></span>|<span data-ttu-id="12723-683">指示是否阻止企业书籍笔记和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="12723-683">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="12723-684">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-684">airPrintBlocked</span></span>|<span data-ttu-id="12723-685">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-685">Boolean</span></span>|<span data-ttu-id="12723-686">指示是否阻止 AirPrint （iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-686">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="12723-687">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="12723-687">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="12723-688">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-688">Boolean</span></span>|<span data-ttu-id="12723-689">指示是否阻止 Airprint 的用户名和密码的密钥链存储（iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-689">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="12723-690">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="12723-690">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="12723-691">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-691">Boolean</span></span>|<span data-ttu-id="12723-692">指示 TLS 打印通信是否需要受信任的证书（iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-692">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="12723-693">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="12723-693">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="12723-694">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-694">Boolean</span></span>|<span data-ttu-id="12723-695">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="12723-695">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="12723-696">这样可以防止虚假的 AirPrint 蓝牙信号免受网络流量（iOS 11.0 及更高版本）的欺骗。</span><span class="sxs-lookup"><span data-stu-id="12723-696">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="12723-697">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-697">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="12723-698">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-698">Boolean</span></span>|<span data-ttu-id="12723-699">指示设备是否可以使用服务器消息块（SMB）协议访问网络服务器上的文件或其他资源。</span><span class="sxs-lookup"><span data-stu-id="12723-699">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="12723-700">适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="12723-700">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="12723-701">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-701">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="12723-702">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-702">Boolean</span></span>|<span data-ttu-id="12723-703">指示带 access 的 sevices 是否可以连接到 USB 驱动器上的文件并打开文件。</span><span class="sxs-lookup"><span data-stu-id="12723-703">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="12723-704">适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="12723-704">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="12723-705">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="12723-705">wifiPowerOnForced</span></span>|<span data-ttu-id="12723-706">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-706">Boolean</span></span>|<span data-ttu-id="12723-707">指示 Wi-fi 是否仍处于打开状态，即使设备处于飞行模式时也是如此。</span><span class="sxs-lookup"><span data-stu-id="12723-707">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="12723-708">适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="12723-708">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="12723-709">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="12723-709">blockSystemAppRemoval</span></span>|<span data-ttu-id="12723-710">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-710">Boolean</span></span>|<span data-ttu-id="12723-711">指示是否在受监督的设备（iOS 11.0 及更高版本）上阻止从设备中删除系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="12723-711">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="12723-712">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="12723-712">vpnBlockCreation</span></span>|<span data-ttu-id="12723-713">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-713">Boolean</span></span>|<span data-ttu-id="12723-714">指示是否阻止创建 VPN 配置（iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-714">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="12723-715">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-715">appRemovalBlocked</span></span>|<span data-ttu-id="12723-716">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-716">Boolean</span></span>|<span data-ttu-id="12723-717">指示是否允许删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="12723-717">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="12723-718">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-718">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="12723-719">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-719">Boolean</span></span>|<span data-ttu-id="12723-720">指示是否允许在锁定设备时连接到 USB 附件（iOS 11.4.1 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-720">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="12723-721">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="12723-721">passwordBlockAutoFill</span></span>|<span data-ttu-id="12723-722">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-722">Boolean</span></span>|<span data-ttu-id="12723-723">指示是否允许自动填充密码功能（iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-723">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="12723-724">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="12723-724">passwordBlockProximityRequests</span></span>|<span data-ttu-id="12723-725">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-725">Boolean</span></span>|<span data-ttu-id="12723-726">指示是否阻止来自附近设备（iOS 12.0 及更高版本）发出请求的密码。</span><span class="sxs-lookup"><span data-stu-id="12723-726">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="12723-727">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="12723-727">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="12723-728">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-728">Boolean</span></span>|<span data-ttu-id="12723-729">指示是否阻止使用 AirDrop 密码的共享密码功能 iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-729">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="12723-730">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="12723-730">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="12723-731">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-731">Boolean</span></span>|<span data-ttu-id="12723-732">指示是否启用日期和时间 "设置自动设置" 功能，以及用户是否无法关闭该功能（iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-732">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="12723-733">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="12723-733">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="12723-734">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-734">Boolean</span></span>|<span data-ttu-id="12723-735">指示托管应用程序是否可以将联系人写入非托管联系人帐户（iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-735">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="12723-736">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="12723-736">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="12723-737">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-737">Boolean</span></span>|<span data-ttu-id="12723-738">指示非托管应用是否可以从托管联系人帐户读取（iOS 12.0 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-738">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="12723-739">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="12723-739">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="12723-740">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-740">Boolean</span></span>|<span data-ttu-id="12723-741">指示是否阻止用户修改个人热点设置（iOS 12.2 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-741">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="12723-742">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-742">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="12723-743">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-743">Boolean</span></span>|<span data-ttu-id="12723-744">指示设备受到监督时是否阻止连续路径键盘（iOS 13 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-744">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="12723-745">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-745">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="12723-746">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-746">Boolean</span></span>|<span data-ttu-id="12723-747">指示设备受到监督时是否阻止查找我的设备（iOS 13 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-747">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="12723-748">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-748">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="12723-749">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-749">Boolean</span></span>|<span data-ttu-id="12723-750">指示设备受到监督时是否阻止查找我的好友（iOS 13 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12723-750">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="12723-751">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="12723-751">iTunesBlocked</span></span>|<span data-ttu-id="12723-752">布尔值</span><span class="sxs-lookup"><span data-stu-id="12723-752">Boolean</span></span>|<span data-ttu-id="12723-753">指示是否阻止 iTunes 应用。</span><span class="sxs-lookup"><span data-stu-id="12723-753">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="12723-754">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="12723-754">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="12723-755">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="12723-755">kioskModeAppType</span></span>|[<span data-ttu-id="12723-756">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="12723-756">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="12723-757">在展台模式下运行的应用类型。</span><span class="sxs-lookup"><span data-stu-id="12723-757">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="12723-758">可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。</span><span class="sxs-lookup"><span data-stu-id="12723-758">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="12723-759">响应</span><span class="sxs-lookup"><span data-stu-id="12723-759">Response</span></span>
<span data-ttu-id="12723-760">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12723-760">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12723-761">示例</span><span class="sxs-lookup"><span data-stu-id="12723-761">Example</span></span>

### <a name="request"></a><span data-ttu-id="12723-762">请求</span><span class="sxs-lookup"><span data-stu-id="12723-762">Request</span></span>
<span data-ttu-id="12723-763">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12723-763">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10518

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
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
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="12723-764">响应</span><span class="sxs-lookup"><span data-stu-id="12723-764">Response</span></span>
<span data-ttu-id="12723-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12723-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10690

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
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
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```




