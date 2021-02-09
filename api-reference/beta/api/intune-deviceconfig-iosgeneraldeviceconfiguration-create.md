---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6fe71b13b76574a379b1695ce20292e15931080
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154640"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="b9200-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9200-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="b9200-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9200-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9200-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9200-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9200-107">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9200-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9200-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9200-108">Prerequisites</span></span>
<span data-ttu-id="b9200-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9200-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9200-111">Permission type</span></span>|<span data-ttu-id="b9200-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9200-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9200-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9200-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9200-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9200-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9200-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9200-116">Not supported.</span></span>|
|<span data-ttu-id="b9200-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9200-117">Application</span></span>|<span data-ttu-id="b9200-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9200-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9200-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b9200-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9200-120">Request headers</span></span>
|<span data-ttu-id="b9200-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9200-121">Header</span></span>|<span data-ttu-id="b9200-122">值</span><span class="sxs-lookup"><span data-stu-id="b9200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9200-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9200-123">Authorization</span></span>|<span data-ttu-id="b9200-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9200-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9200-125">Accept</span></span>|<span data-ttu-id="b9200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9200-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9200-127">Request body</span></span>
<span data-ttu-id="b9200-128">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9200-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="b9200-129">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b9200-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="b9200-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9200-130">Property</span></span>|<span data-ttu-id="b9200-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9200-131">Type</span></span>|<span data-ttu-id="b9200-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9200-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9200-133">id</span><span class="sxs-lookup"><span data-stu-id="b9200-133">id</span></span>|<span data-ttu-id="b9200-134">String</span><span class="sxs-lookup"><span data-stu-id="b9200-134">String</span></span>|<span data-ttu-id="b9200-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b9200-135">Key of the entity.</span></span> <span data-ttu-id="b9200-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9200-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b9200-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9200-138">DateTimeOffset</span></span>|<span data-ttu-id="b9200-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b9200-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b9200-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9200-141">roleScopeTagIds</span></span>|<span data-ttu-id="b9200-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b9200-142">String collection</span></span>|<span data-ttu-id="b9200-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b9200-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9200-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9200-145">supportsScopeTags</span></span>|<span data-ttu-id="b9200-146">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-146">Boolean</span></span>|<span data-ttu-id="b9200-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="b9200-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b9200-148">如果此值为 false 且实体对范围用户不可见，则不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b9200-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b9200-149">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="b9200-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b9200-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b9200-150">This property is read-only.</span></span> <span data-ttu-id="b9200-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b9200-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b9200-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b9200-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b9200-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="b9200-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b9200-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b9200-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b9200-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b9200-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b9200-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b9200-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b9200-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b9200-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b9200-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b9200-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b9200-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b9200-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b9200-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9200-164">createdDateTime</span></span>|<span data-ttu-id="b9200-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9200-165">DateTimeOffset</span></span>|<span data-ttu-id="b9200-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b9200-166">DateTime the object was created.</span></span> <span data-ttu-id="b9200-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-168">说明</span><span class="sxs-lookup"><span data-stu-id="b9200-168">description</span></span>|<span data-ttu-id="b9200-169">String</span><span class="sxs-lookup"><span data-stu-id="b9200-169">String</span></span>|<span data-ttu-id="b9200-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b9200-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9200-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b9200-172">displayName</span></span>|<span data-ttu-id="b9200-173">String</span><span class="sxs-lookup"><span data-stu-id="b9200-173">String</span></span>|<span data-ttu-id="b9200-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b9200-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9200-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-176">version</span><span class="sxs-lookup"><span data-stu-id="b9200-176">version</span></span>|<span data-ttu-id="b9200-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-177">Int32</span></span>|<span data-ttu-id="b9200-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b9200-178">Version of the device configuration.</span></span> <span data-ttu-id="b9200-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9200-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9200-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="b9200-180">accountBlockModification</span></span>|<span data-ttu-id="b9200-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-181">Boolean</span></span>|<span data-ttu-id="b9200-182">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="b9200-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="b9200-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="b9200-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-184">Boolean</span></span>|<span data-ttu-id="b9200-185">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="b9200-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="b9200-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-186">airDropBlocked</span></span>|<span data-ttu-id="b9200-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-187">Boolean</span></span>|<span data-ttu-id="b9200-188">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="b9200-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="b9200-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="b9200-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-190">Boolean</span></span>|<span data-ttu-id="b9200-191">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="b9200-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="b9200-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-193">Boolean</span></span>|<span data-ttu-id="b9200-194">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="b9200-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="b9200-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="b9200-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="b9200-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-196">Boolean</span></span>|<span data-ttu-id="b9200-197">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="b9200-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="b9200-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-199">Boolean</span></span>|<span data-ttu-id="b9200-200">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="b9200-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-201">appleNewsBlocked</span></span>|<span data-ttu-id="b9200-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-202">Boolean</span></span>|<span data-ttu-id="b9200-203">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="b9200-204">appsSingleAppModeList</span></span>|<span data-ttu-id="b9200-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b9200-206">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="b9200-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="b9200-207">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="b9200-207">Supervised only.</span></span> <span data-ttu-id="b9200-208">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="b9200-208">iOS 7.0 and later.</span></span> <span data-ttu-id="b9200-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b9200-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b9200-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="b9200-210">appsVisibilityList</span></span>|<span data-ttu-id="b9200-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b9200-212">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="b9200-213">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b9200-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b9200-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="b9200-214">appsVisibilityListType</span></span>|[<span data-ttu-id="b9200-215">appListType</span><span class="sxs-lookup"><span data-stu-id="b9200-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b9200-216">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="b9200-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="b9200-217">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="b9200-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b9200-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="b9200-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="b9200-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-219">Boolean</span></span>|<span data-ttu-id="b9200-220">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-221">appStoreBlocked</span></span>|<span data-ttu-id="b9200-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-222">Boolean</span></span>|<span data-ttu-id="b9200-223">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="b9200-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="b9200-224">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="b9200-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="b9200-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-226">Boolean</span></span>|<span data-ttu-id="b9200-227">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="b9200-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="b9200-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b9200-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="b9200-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-229">Boolean</span></span>|<span data-ttu-id="b9200-230">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="b9200-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="b9200-231">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="b9200-232">appStoreRequirePassword</span></span>|<span data-ttu-id="b9200-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-233">Boolean</span></span>|<span data-ttu-id="b9200-234">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b9200-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="b9200-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="b9200-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="b9200-236">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-236">Boolean</span></span>|<span data-ttu-id="b9200-237">指示在 Safari 和其他受监督设备上应用自动填充密码和信用卡信息之前是否强制用户身份验证。</span><span class="sxs-lookup"><span data-stu-id="b9200-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="b9200-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="b9200-238">bluetoothBlockModification</span></span>|<span data-ttu-id="b9200-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-239">Boolean</span></span>|<span data-ttu-id="b9200-240">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="b9200-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-241">cameraBlocked</span></span>|<span data-ttu-id="b9200-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-242">Boolean</span></span>|<span data-ttu-id="b9200-243">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="b9200-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="b9200-244">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b9200-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b9200-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-246">Boolean</span></span>|<span data-ttu-id="b9200-247">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="b9200-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b9200-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="b9200-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="b9200-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-249">Boolean</span></span>|<span data-ttu-id="b9200-250">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="b9200-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="b9200-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="b9200-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="b9200-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-252">Boolean</span></span>|<span data-ttu-id="b9200-253">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="b9200-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="b9200-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-255">Boolean</span></span>|<span data-ttu-id="b9200-256">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="b9200-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="b9200-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="b9200-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="b9200-258">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-258">Boolean</span></span>|<span data-ttu-id="b9200-259">指示是否允许用户更改受监督设备上手机网络计划的设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="b9200-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b9200-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b9200-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-261">Boolean</span></span>|<span data-ttu-id="b9200-262">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="b9200-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b9200-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="b9200-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="b9200-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-264">Boolean</span></span>|<span data-ttu-id="b9200-265">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="b9200-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="b9200-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b9200-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b9200-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-267">Boolean</span></span>|<span data-ttu-id="b9200-268">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b9200-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b9200-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b9200-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-270">Boolean</span></span>|<span data-ttu-id="b9200-271">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="b9200-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="b9200-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="b9200-273">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-273">Boolean</span></span>|<span data-ttu-id="b9200-274">指示设备在监督模式下时是否自动授予对教师请求的权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="b9200-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="b9200-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="b9200-276">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-276">Boolean</span></span>|<span data-ttu-id="b9200-277">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="b9200-278">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="b9200-278">Supervised only.</span></span>|
|<span data-ttu-id="b9200-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b9200-279">compliantAppsList</span></span>|<span data-ttu-id="b9200-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b9200-281">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="b9200-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b9200-282">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b9200-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b9200-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b9200-283">compliantAppListType</span></span>|[<span data-ttu-id="b9200-284">appListType</span><span class="sxs-lookup"><span data-stu-id="b9200-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b9200-285">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="b9200-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b9200-286">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="b9200-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b9200-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="b9200-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="b9200-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-288">Boolean</span></span>|<span data-ttu-id="b9200-289">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="b9200-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-290">definitionLookupBlocked</span></span>|<span data-ttu-id="b9200-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-291">Boolean</span></span>|<span data-ttu-id="b9200-292">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="b9200-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="b9200-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="b9200-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-294">Boolean</span></span>|<span data-ttu-id="b9200-295">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="b9200-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="b9200-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-297">Boolean</span></span>|<span data-ttu-id="b9200-298">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="b9200-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="b9200-299">deviceBlockNameModification</span></span>|<span data-ttu-id="b9200-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-300">Boolean</span></span>|<span data-ttu-id="b9200-301">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b9200-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b9200-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-303">Boolean</span></span>|<span data-ttu-id="b9200-304">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="b9200-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b9200-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="b9200-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="b9200-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-306">Boolean</span></span>|<span data-ttu-id="b9200-307">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="b9200-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="b9200-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="b9200-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-309">Boolean</span></span>|<span data-ttu-id="b9200-310">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="b9200-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="b9200-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="b9200-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="b9200-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-312">Boolean</span></span>|<span data-ttu-id="b9200-313">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="b9200-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="b9200-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b9200-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="b9200-315">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-315">String collection</span></span>|<span data-ttu-id="b9200-316">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="b9200-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b9200-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="b9200-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="b9200-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-318">Boolean</span></span>|<span data-ttu-id="b9200-319">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="b9200-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="b9200-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="b9200-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="b9200-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-321">Boolean</span></span>|<span data-ttu-id="b9200-322">\[已弃用 \] 配置此设置，将值设置为"true"对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="b9200-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="b9200-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="b9200-323">esimBlockModification</span></span>|<span data-ttu-id="b9200-324">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-324">Boolean</span></span>|<span data-ttu-id="b9200-325">指示是否允许在受监督设备的 eSIM 上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="b9200-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="b9200-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-326">faceTimeBlocked</span></span>|<span data-ttu-id="b9200-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-327">Boolean</span></span>|<span data-ttu-id="b9200-328">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="b9200-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="b9200-329">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="b9200-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-331">Boolean</span></span>|<span data-ttu-id="b9200-332">指示设备在监督模式下时是否阻止对"查找我的好友"的更改。</span><span class="sxs-lookup"><span data-stu-id="b9200-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="b9200-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="b9200-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-334">Boolean</span></span>|<span data-ttu-id="b9200-335">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="b9200-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="b9200-336">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="b9200-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="b9200-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-338">Boolean</span></span>|<span data-ttu-id="b9200-339">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="b9200-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="b9200-340">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-341">gameCenterBlocked</span></span>|<span data-ttu-id="b9200-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-342">Boolean</span></span>|<span data-ttu-id="b9200-343">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="b9200-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-344">hostPairingBlocked</span></span>|<span data-ttu-id="b9200-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-345">Boolean</span></span>|<span data-ttu-id="b9200-346">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="b9200-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-348">Boolean</span></span>|<span data-ttu-id="b9200-349">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="b9200-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="b9200-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="b9200-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-351">Boolean</span></span>|<span data-ttu-id="b9200-352">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="b9200-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="b9200-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b9200-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b9200-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-354">Boolean</span></span>|<span data-ttu-id="b9200-355">指示是否阻止用户继续他们在 iOS 设备上启动的工作到其他 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="b9200-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b9200-356">iCloudBlockBackup</span></span>|<span data-ttu-id="b9200-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-357">Boolean</span></span>|<span data-ttu-id="b9200-358">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="b9200-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="b9200-359">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b9200-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b9200-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-361">Boolean</span></span>|<span data-ttu-id="b9200-362">指示是否阻止 iCloud 文档同步。需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="b9200-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="b9200-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-364">Boolean</span></span>|<span data-ttu-id="b9200-365">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="b9200-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="b9200-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b9200-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b9200-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-367">Boolean</span></span>|<span data-ttu-id="b9200-368">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="b9200-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b9200-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="b9200-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="b9200-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-370">Boolean</span></span>|<span data-ttu-id="b9200-371">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="b9200-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="b9200-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="b9200-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="b9200-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-373">Boolean</span></span>|<span data-ttu-id="b9200-374">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="b9200-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="b9200-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="b9200-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="b9200-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-376">Boolean</span></span>|<span data-ttu-id="b9200-377">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="b9200-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="b9200-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="b9200-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="b9200-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-379">Boolean</span></span>|<span data-ttu-id="b9200-380">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="b9200-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="b9200-381">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b9200-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="b9200-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-383">Boolean</span></span>|<span data-ttu-id="b9200-384">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b9200-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="b9200-385">iTunesBlockRadio</span></span>|<span data-ttu-id="b9200-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-386">Boolean</span></span>|<span data-ttu-id="b9200-387">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b9200-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="b9200-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="b9200-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-389">Boolean</span></span>|<span data-ttu-id="b9200-390">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b9200-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b9200-391">keyboardBlockDictation</span></span>|<span data-ttu-id="b9200-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-392">Boolean</span></span>|<span data-ttu-id="b9200-393">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="b9200-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="b9200-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="b9200-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-395">Boolean</span></span>|<span data-ttu-id="b9200-396">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b9200-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="b9200-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="b9200-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-398">Boolean</span></span>|<span data-ttu-id="b9200-399">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="b9200-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="b9200-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-401">Boolean</span></span>|<span data-ttu-id="b9200-402">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b9200-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="b9200-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="b9200-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-404">Boolean</span></span>|<span data-ttu-id="b9200-405">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="b9200-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="b9200-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-407">Boolean</span></span>|<span data-ttu-id="b9200-408">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="b9200-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="b9200-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-410">Boolean</span></span>|<span data-ttu-id="b9200-411">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="b9200-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="b9200-412">此属性的功能在操作系统默认设置下是冗余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="b9200-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b9200-413">请改为使用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="b9200-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="b9200-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="b9200-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="b9200-415">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-415">Boolean</span></span>|<span data-ttu-id="b9200-416">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="b9200-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="b9200-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-418">Boolean</span></span>|<span data-ttu-id="b9200-419">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b9200-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="b9200-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-421">Boolean</span></span>|<span data-ttu-id="b9200-422">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="b9200-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="b9200-423">此属性的功能在操作系统默认设置下是冗余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="b9200-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b9200-424">请改为使用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="b9200-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="b9200-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b9200-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="b9200-426">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-426">Boolean</span></span>|<span data-ttu-id="b9200-427">指示在展台模式下是否阻止使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="b9200-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b9200-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="b9200-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-429">Boolean</span></span>|<span data-ttu-id="b9200-430">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="b9200-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="b9200-431">此属性的功能在操作系统默认设置下是冗余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="b9200-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b9200-432">请改为使用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="b9200-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="b9200-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b9200-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="b9200-434">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-434">Boolean</span></span>|<span data-ttu-id="b9200-435">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="b9200-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="b9200-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="b9200-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-437">Boolean</span></span>|<span data-ttu-id="b9200-438">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="b9200-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="b9200-439">此属性的功能在操作系统默认设置下是冗余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="b9200-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b9200-440">请改为使用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="b9200-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="b9200-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="b9200-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="b9200-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-442">Boolean</span></span>|<span data-ttu-id="b9200-443">指示在展台模式下是否阻止使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="b9200-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b9200-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="b9200-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-445">Boolean</span></span>|<span data-ttu-id="b9200-446">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="b9200-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="b9200-447">此属性的功能在操作系统默认设置下是冗余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="b9200-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b9200-448">请改为使用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="b9200-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="b9200-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b9200-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="b9200-450">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-450">Boolean</span></span>|<span data-ttu-id="b9200-451">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="b9200-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="b9200-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="b9200-453">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-453">Boolean</span></span>|<span data-ttu-id="b9200-454">指示是否在展台模式下启用语音控制。</span><span class="sxs-lookup"><span data-stu-id="b9200-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="b9200-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="b9200-456">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-456">Boolean</span></span>|<span data-ttu-id="b9200-457">指示是否允许用户在展台模式下切换语音控制。</span><span class="sxs-lookup"><span data-stu-id="b9200-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="b9200-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-459">Boolean</span></span>|<span data-ttu-id="b9200-460">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b9200-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="b9200-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-462">Boolean</span></span>|<span data-ttu-id="b9200-463">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="b9200-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="b9200-464">此属性的功能在操作系统默认设置下是冗余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="b9200-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b9200-465">请改为使用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="b9200-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="b9200-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b9200-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="b9200-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-467">Boolean</span></span>|<span data-ttu-id="b9200-468">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="b9200-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="b9200-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="b9200-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-470">Boolean</span></span>|<span data-ttu-id="b9200-471">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b9200-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="b9200-473">String</span><span class="sxs-lookup"><span data-stu-id="b9200-473">String</span></span>|<span data-ttu-id="b9200-474">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="b9200-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="b9200-475">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="b9200-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="b9200-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="b9200-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="b9200-477">String</span><span class="sxs-lookup"><span data-stu-id="b9200-477">String</span></span>|<span data-ttu-id="b9200-478">用于展台模式的内置应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="b9200-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="b9200-479">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="b9200-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="b9200-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="b9200-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="b9200-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-481">Boolean</span></span>|<span data-ttu-id="b9200-482">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="b9200-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="b9200-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="b9200-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-484">Boolean</span></span>|<span data-ttu-id="b9200-485">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="b9200-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="b9200-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="b9200-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-487">Boolean</span></span>|<span data-ttu-id="b9200-488">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="b9200-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="b9200-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="b9200-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-490">Boolean</span></span>|<span data-ttu-id="b9200-491">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="b9200-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="b9200-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="b9200-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-493">Boolean</span></span>|<span data-ttu-id="b9200-494">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="b9200-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="b9200-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="b9200-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="b9200-496">String</span><span class="sxs-lookup"><span data-stu-id="b9200-496">String</span></span>|<span data-ttu-id="b9200-497">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="b9200-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="b9200-498">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="b9200-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="b9200-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="b9200-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="b9200-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-500">Boolean</span></span>|<span data-ttu-id="b9200-501">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="b9200-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="b9200-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="b9200-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="b9200-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-503">Boolean</span></span>|<span data-ttu-id="b9200-504">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="b9200-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="b9200-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="b9200-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="b9200-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-506">Boolean</span></span>|<span data-ttu-id="b9200-507">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="b9200-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="b9200-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="b9200-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="b9200-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-509">Boolean</span></span>|<span data-ttu-id="b9200-510">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="b9200-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="b9200-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b9200-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="b9200-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b9200-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="b9200-513">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="b9200-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b9200-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="b9200-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b9200-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="b9200-516">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="b9200-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b9200-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="b9200-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b9200-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="b9200-519">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="b9200-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b9200-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="b9200-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b9200-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="b9200-522">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="b9200-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b9200-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="b9200-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b9200-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="b9200-525">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="b9200-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b9200-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="b9200-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b9200-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="b9200-528">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="b9200-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b9200-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="b9200-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b9200-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="b9200-531">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="b9200-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b9200-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="b9200-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b9200-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="b9200-534">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="b9200-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b9200-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="b9200-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b9200-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="b9200-537">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="b9200-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="b9200-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="b9200-538">networkUsageRules</span></span>|<span data-ttu-id="b9200-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="b9200-540">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="b9200-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="b9200-541">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b9200-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b9200-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="b9200-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="b9200-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="b9200-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="b9200-544">应用的媒体内容分级设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="b9200-545">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="b9200-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="b9200-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-546">messagesBlocked</span></span>|<span data-ttu-id="b9200-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-547">Boolean</span></span>|<span data-ttu-id="b9200-548">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="b9200-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="b9200-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="b9200-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="b9200-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-550">Boolean</span></span>|<span data-ttu-id="b9200-551">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b9200-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b9200-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="b9200-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-553">Boolean</span></span>|<span data-ttu-id="b9200-554">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="b9200-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b9200-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="b9200-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="b9200-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-556">Boolean</span></span>|<span data-ttu-id="b9200-557">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="b9200-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="b9200-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="b9200-558">passcodeBlockModification</span></span>|<span data-ttu-id="b9200-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-559">Boolean</span></span>|<span data-ttu-id="b9200-560">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b9200-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b9200-561">passcodeBlockSimple</span></span>|<span data-ttu-id="b9200-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-562">Boolean</span></span>|<span data-ttu-id="b9200-563">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="b9200-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b9200-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b9200-564">passcodeExpirationDays</span></span>|<span data-ttu-id="b9200-565">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-565">Int32</span></span>|<span data-ttu-id="b9200-566">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="b9200-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="b9200-567">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="b9200-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b9200-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b9200-568">passcodeMinimumLength</span></span>|<span data-ttu-id="b9200-569">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-569">Int32</span></span>|<span data-ttu-id="b9200-570">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="b9200-570">Minimum length of passcode.</span></span> <span data-ttu-id="b9200-571">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="b9200-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b9200-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b9200-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b9200-573">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-573">Int32</span></span>|<span data-ttu-id="b9200-574">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b9200-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b9200-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b9200-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b9200-576">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-576">Int32</span></span>|<span data-ttu-id="b9200-577">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b9200-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b9200-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b9200-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b9200-579">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-579">Int32</span></span>|<span data-ttu-id="b9200-580">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b9200-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="b9200-581">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="b9200-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b9200-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b9200-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b9200-583">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-583">Int32</span></span>|<span data-ttu-id="b9200-584">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b9200-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="b9200-585">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="b9200-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b9200-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="b9200-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="b9200-587">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-587">Int32</span></span>|<span data-ttu-id="b9200-588">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="b9200-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="b9200-589">有效值 2 到 11</span><span class="sxs-lookup"><span data-stu-id="b9200-589">Valid values 2 to 11</span></span>|
|<span data-ttu-id="b9200-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b9200-590">passcodeRequiredType</span></span>|[<span data-ttu-id="b9200-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b9200-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b9200-592">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b9200-592">Type of passcode that is required.</span></span> <span data-ttu-id="b9200-593">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b9200-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b9200-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b9200-594">passcodeRequired</span></span>|<span data-ttu-id="b9200-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-595">Boolean</span></span>|<span data-ttu-id="b9200-596">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b9200-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b9200-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-597">podcastsBlocked</span></span>|<span data-ttu-id="b9200-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-598">Boolean</span></span>|<span data-ttu-id="b9200-599">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="b9200-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="b9200-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="b9200-601">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-601">Boolean</span></span>|<span data-ttu-id="b9200-602">指示是否启用提示以使用受监督的设备设置附近设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="b9200-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b9200-603">safariBlockAutofill</span></span>|<span data-ttu-id="b9200-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-604">Boolean</span></span>|<span data-ttu-id="b9200-605">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="b9200-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="b9200-606">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b9200-607">safariBlockJavaScript</span></span>|<span data-ttu-id="b9200-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-608">Boolean</span></span>|<span data-ttu-id="b9200-609">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="b9200-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="b9200-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b9200-610">safariBlockPopups</span></span>|<span data-ttu-id="b9200-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-611">Boolean</span></span>|<span data-ttu-id="b9200-612">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b9200-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="b9200-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-613">safariBlocked</span></span>|<span data-ttu-id="b9200-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-614">Boolean</span></span>|<span data-ttu-id="b9200-615">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="b9200-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="b9200-616">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-617">safariCookieSettings</span></span>|[<span data-ttu-id="b9200-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b9200-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="b9200-619">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="b9200-619">Cookie settings for Safari.</span></span> <span data-ttu-id="b9200-620">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="b9200-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="b9200-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="b9200-621">safariManagedDomains</span></span>|<span data-ttu-id="b9200-622">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-622">String collection</span></span>|<span data-ttu-id="b9200-623">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="b9200-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="b9200-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="b9200-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="b9200-625">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9200-625">String collection</span></span>|<span data-ttu-id="b9200-626">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="b9200-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="b9200-627">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b9200-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b9200-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="b9200-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-629">Boolean</span></span>|<span data-ttu-id="b9200-630">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="b9200-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="b9200-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-631">screenCaptureBlocked</span></span>|<span data-ttu-id="b9200-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-632">Boolean</span></span>|<span data-ttu-id="b9200-633">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="b9200-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b9200-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-634">siriBlocked</span></span>|<span data-ttu-id="b9200-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-635">Boolean</span></span>|<span data-ttu-id="b9200-636">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="b9200-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="b9200-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="b9200-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="b9200-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-638">Boolean</span></span>|<span data-ttu-id="b9200-639">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="b9200-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="b9200-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="b9200-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="b9200-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-641">Boolean</span></span>|<span data-ttu-id="b9200-642">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="b9200-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="b9200-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="b9200-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="b9200-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-644">Boolean</span></span>|<span data-ttu-id="b9200-645">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="b9200-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="b9200-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="b9200-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="b9200-647">Int32</span><span class="sxs-lookup"><span data-stu-id="b9200-647">Int32</span></span>|<span data-ttu-id="b9200-648">设置对受监督设备取消软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="b9200-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="b9200-649">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="b9200-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="b9200-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="b9200-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="b9200-651">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-651">Boolean</span></span>|<span data-ttu-id="b9200-652">指示设备在监督模式下时是否延迟软件更新的用户可见性。</span><span class="sxs-lookup"><span data-stu-id="b9200-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b9200-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b9200-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-654">Boolean</span></span>|<span data-ttu-id="b9200-655">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="b9200-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="b9200-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-656">voiceDialingBlocked</span></span>|<span data-ttu-id="b9200-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-657">Boolean</span></span>|<span data-ttu-id="b9200-658">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="b9200-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b9200-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="b9200-659">wallpaperBlockModification</span></span>|<span data-ttu-id="b9200-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-660">Boolean</span></span>|<span data-ttu-id="b9200-661">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="b9200-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="b9200-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="b9200-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="b9200-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9200-663">Boolean</span></span>|<span data-ttu-id="b9200-664">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="b9200-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b9200-665">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="b9200-665">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="b9200-666">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-666">Boolean</span></span>|<span data-ttu-id="b9200-667">指示通过 Classroom 注册非托管课程的学生在尝试离开 (iOS 11.3 及更高版本课程时是否将请求教师) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-667">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="b9200-668">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="b9200-668">keychainBlockCloudSync</span></span>|<span data-ttu-id="b9200-669">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-669">Boolean</span></span>|<span data-ttu-id="b9200-670">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="b9200-670">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="b9200-671">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-671">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-672">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="b9200-672">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="b9200-673">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-673">Boolean</span></span>|<span data-ttu-id="b9200-674">指示是否阻止高空 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="b9200-674">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="b9200-675">如果此限制设置为 false，则不禁用 iOS 7.0 (和更高版本的 CRL 和 OCSP) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-675">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b9200-676">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="b9200-676">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="b9200-677">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-677">Boolean</span></span>|<span data-ttu-id="b9200-678">指示广告跟踪是否受限。 (iOS 7.0 及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-678">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b9200-679">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b9200-679">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="b9200-680">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-680">Boolean</span></span>|<span data-ttu-id="b9200-681">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="b9200-681">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="b9200-682">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="b9200-682">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="b9200-683">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-683">Boolean</span></span>|<span data-ttu-id="b9200-684">指示是否阻止企业书籍备注和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="b9200-684">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="b9200-685">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-685">airPrintBlocked</span></span>|<span data-ttu-id="b9200-686">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-686">Boolean</span></span>|<span data-ttu-id="b9200-687">指示在 iOS 11.0 (中是否阻止 AirPrint) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-687">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b9200-688">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="b9200-688">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="b9200-689">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-689">Boolean</span></span>|<span data-ttu-id="b9200-690">指示在 iOS 11.0 及更高版本中是否阻止用于 Airprint 的用户名和密码 (密钥链) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-690">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b9200-691">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="b9200-691">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="b9200-692">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-692">Boolean</span></span>|<span data-ttu-id="b9200-693">指示在 iOS 11.0 及更高版本的 TLS 打印通信 (信任证书) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-693">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b9200-694">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="b9200-694">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="b9200-695">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-695">Boolean</span></span>|<span data-ttu-id="b9200-696">指示是否阻止了 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="b9200-696">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="b9200-697">这可以防止恶意的 AirPrint Bluetooth信号通过网络钓鱼 (iOS 11.0 及更高版本的网络流量) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-697">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b9200-698">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-698">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="b9200-699">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-699">Boolean</span></span>|<span data-ttu-id="b9200-700">指示设备能否使用 SMB 协议中的服务器消息阻止访问网络 (或其他) 资源。</span><span class="sxs-lookup"><span data-stu-id="b9200-700">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="b9200-701">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-701">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="b9200-702">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-702">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="b9200-703">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-703">Boolean</span></span>|<span data-ttu-id="b9200-704">指示具有访问权限的文件能否连接到 USB 驱动器上并打开文件。</span><span class="sxs-lookup"><span data-stu-id="b9200-704">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="b9200-705">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-705">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="b9200-706">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="b9200-706">wifiPowerOnForced</span></span>|<span data-ttu-id="b9200-707">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-707">Boolean</span></span>|<span data-ttu-id="b9200-708">指示设备是否Wi-Fi保持打开状态，即使设备处于飞行模式。</span><span class="sxs-lookup"><span data-stu-id="b9200-708">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="b9200-709">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-709">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="b9200-710">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="b9200-710">blockSystemAppRemoval</span></span>|<span data-ttu-id="b9200-711">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-711">Boolean</span></span>|<span data-ttu-id="b9200-712">指示在受监督的设备上是否阻止从设备删除系统应用 (iOS 11.0 及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-712">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b9200-713">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="b9200-713">vpnBlockCreation</span></span>|<span data-ttu-id="b9200-714">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-714">Boolean</span></span>|<span data-ttu-id="b9200-715">指示在 iOS 11.0 (更高版本中是否阻止创建 VPN) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-715">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b9200-716">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-716">appRemovalBlocked</span></span>|<span data-ttu-id="b9200-717">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-717">Boolean</span></span>|<span data-ttu-id="b9200-718">指示是否允许删除应用。</span><span class="sxs-lookup"><span data-stu-id="b9200-718">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="b9200-719">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-719">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="b9200-720">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-720">Boolean</span></span>|<span data-ttu-id="b9200-721">指示是否允许在 iOS 11.4.1 (设备锁定时连接到 USB) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-721">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="b9200-722">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="b9200-722">passwordBlockAutoFill</span></span>|<span data-ttu-id="b9200-723">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-723">Boolean</span></span>|<span data-ttu-id="b9200-724">指示是否允许在 iOS 12.0 (使用"自动填充密码") 。</span><span class="sxs-lookup"><span data-stu-id="b9200-724">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b9200-725">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="b9200-725">passwordBlockProximityRequests</span></span>|<span data-ttu-id="b9200-726">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-726">Boolean</span></span>|<span data-ttu-id="b9200-727">指示是否阻止从 iOS 12.0 (及更高版本的附近设备请求) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-727">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b9200-728">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="b9200-728">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="b9200-729">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-729">Boolean</span></span>|<span data-ttu-id="b9200-730">指示是否阻止使用 AirDrop 密码功能 iOS 12.0 及更高版本共享) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-730">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b9200-731">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="b9200-731">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="b9200-732">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-732">Boolean</span></span>|<span data-ttu-id="b9200-733">指示日期和时间"自动设置"功能是否已启用，并且用户 (iOS 12.0 及更高版本无法) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-733">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b9200-734">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="b9200-734">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="b9200-735">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-735">Boolean</span></span>|<span data-ttu-id="b9200-736">指示托管应用是否可以将联系人写入 iOS 12.0 及更高版本 (非托管联系人) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-736">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b9200-737">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="b9200-737">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="b9200-738">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-738">Boolean</span></span>|<span data-ttu-id="b9200-739">指示非托管应用是否可以从 iOS 12.0 (托管联系人帐户读取) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-739">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="b9200-740">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="b9200-740">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="b9200-741">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-741">Boolean</span></span>|<span data-ttu-id="b9200-742">指示是否阻止用户修改 iOS 12.2 (或更高版本的个人热点) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-742">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="b9200-743">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-743">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="b9200-744">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-744">Boolean</span></span>|<span data-ttu-id="b9200-745">指示在 iOS 13 或更高版本的设备受 (时是否阻止连续路径) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-745">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b9200-746">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-746">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="b9200-747">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-747">Boolean</span></span>|<span data-ttu-id="b9200-748">指示在 iOS 13 或更高版本中监督设备时是否阻止 (查找我的) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-748">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b9200-749">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-749">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="b9200-750">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-750">Boolean</span></span>|<span data-ttu-id="b9200-751">指示在 iOS 13 或更高版本的设备受 (时是否阻止"查找我的好友") 。</span><span class="sxs-lookup"><span data-stu-id="b9200-751">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b9200-752">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-752">iTunesBlocked</span></span>|<span data-ttu-id="b9200-753">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-753">Boolean</span></span>|<span data-ttu-id="b9200-754">指示是否阻止 iTunes 应用。</span><span class="sxs-lookup"><span data-stu-id="b9200-754">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="b9200-755">需要 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="b9200-755">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b9200-756">sharedDeviceBlockTemporarySessions</span><span class="sxs-lookup"><span data-stu-id="b9200-756">sharedDeviceBlockTemporarySessions</span></span>|<span data-ttu-id="b9200-757">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-757">Boolean</span></span>|<span data-ttu-id="b9200-758">指示是否阻止共享 iPad 上的临时会话 (iOS 13.4 或更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="b9200-758">Indicates whether or not to block temporary sessions on Shared iPads (iOS 13.4 or later).</span></span>|
|<span data-ttu-id="b9200-759">appClipsBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-759">appClipsBlocked</span></span>|<span data-ttu-id="b9200-760">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-760">Boolean</span></span>|<span data-ttu-id="b9200-761">阻止用户添加任何应用剪辑并删除设备上的任何现有应用剪辑。</span><span class="sxs-lookup"><span data-stu-id="b9200-761">Prevents a user from adding any App Clips and removes any existing App Clips on the device.</span></span>|
|<span data-ttu-id="b9200-762">applePersonalizedAdsBlocked</span><span class="sxs-lookup"><span data-stu-id="b9200-762">applePersonalizedAdsBlocked</span></span>|<span data-ttu-id="b9200-763">布尔</span><span class="sxs-lookup"><span data-stu-id="b9200-763">Boolean</span></span>|<span data-ttu-id="b9200-764">如果为 true，限制 Apple 个性化广告。</span><span class="sxs-lookup"><span data-stu-id="b9200-764">Limits Apple personalized advertising when true.</span></span> <span data-ttu-id="b9200-765">在 iOS 14 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="b9200-765">Available in iOS 14 and later.</span></span>|
|<span data-ttu-id="b9200-766">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="b9200-766">kioskModeAppType</span></span>|[<span data-ttu-id="b9200-767">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="b9200-767">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="b9200-768">在展台模式下运行的应用类型。</span><span class="sxs-lookup"><span data-stu-id="b9200-768">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="b9200-769">可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。</span><span class="sxs-lookup"><span data-stu-id="b9200-769">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="b9200-770">响应</span><span class="sxs-lookup"><span data-stu-id="b9200-770">Response</span></span>
<span data-ttu-id="b9200-771">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9200-771">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9200-772">示例</span><span class="sxs-lookup"><span data-stu-id="b9200-772">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9200-773">请求</span><span class="sxs-lookup"><span data-stu-id="b9200-773">Request</span></span>
<span data-ttu-id="b9200-774">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9200-774">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10633

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
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="b9200-775">响应</span><span class="sxs-lookup"><span data-stu-id="b9200-775">Response</span></span>
<span data-ttu-id="b9200-p158">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9200-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10805

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
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```




