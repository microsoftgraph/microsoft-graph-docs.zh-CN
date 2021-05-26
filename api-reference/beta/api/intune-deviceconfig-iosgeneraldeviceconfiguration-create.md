---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a88b6e742afd253fd9eb370becfa4e566d39f729
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666181"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="0372e-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0372e-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="0372e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0372e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0372e-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0372e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0372e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0372e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0372e-107">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0372e-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0372e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0372e-108">Prerequisites</span></span>
<span data-ttu-id="0372e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0372e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0372e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0372e-111">Permission type</span></span>|<span data-ttu-id="0372e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0372e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0372e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0372e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0372e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0372e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0372e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0372e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0372e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0372e-116">Not supported.</span></span>|
|<span data-ttu-id="0372e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0372e-117">Application</span></span>|<span data-ttu-id="0372e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0372e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0372e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0372e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0372e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0372e-120">Request headers</span></span>
|<span data-ttu-id="0372e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0372e-121">Header</span></span>|<span data-ttu-id="0372e-122">值</span><span class="sxs-lookup"><span data-stu-id="0372e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0372e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0372e-123">Authorization</span></span>|<span data-ttu-id="0372e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0372e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0372e-125">接受</span><span class="sxs-lookup"><span data-stu-id="0372e-125">Accept</span></span>|<span data-ttu-id="0372e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0372e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0372e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0372e-127">Request body</span></span>
<span data-ttu-id="0372e-128">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0372e-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="0372e-129">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0372e-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="0372e-130">属性</span><span class="sxs-lookup"><span data-stu-id="0372e-130">Property</span></span>|<span data-ttu-id="0372e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0372e-131">Type</span></span>|<span data-ttu-id="0372e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0372e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0372e-133">id</span><span class="sxs-lookup"><span data-stu-id="0372e-133">id</span></span>|<span data-ttu-id="0372e-134">String</span><span class="sxs-lookup"><span data-stu-id="0372e-134">String</span></span>|<span data-ttu-id="0372e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0372e-135">Key of the entity.</span></span> <span data-ttu-id="0372e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0372e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0372e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0372e-138">DateTimeOffset</span></span>|<span data-ttu-id="0372e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0372e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0372e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0372e-141">roleScopeTagIds</span></span>|<span data-ttu-id="0372e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0372e-142">String collection</span></span>|<span data-ttu-id="0372e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0372e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0372e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0372e-145">supportsScopeTags</span></span>|<span data-ttu-id="0372e-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-146">Boolean</span></span>|<span data-ttu-id="0372e-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="0372e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0372e-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0372e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0372e-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="0372e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0372e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0372e-150">This property is read-only.</span></span> <span data-ttu-id="0372e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0372e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0372e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0372e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0372e-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="0372e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0372e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0372e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0372e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0372e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0372e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0372e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0372e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0372e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0372e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0372e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0372e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0372e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0372e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0372e-164">createdDateTime</span></span>|<span data-ttu-id="0372e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0372e-165">DateTimeOffset</span></span>|<span data-ttu-id="0372e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0372e-166">DateTime the object was created.</span></span> <span data-ttu-id="0372e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-168">说明</span><span class="sxs-lookup"><span data-stu-id="0372e-168">description</span></span>|<span data-ttu-id="0372e-169">String</span><span class="sxs-lookup"><span data-stu-id="0372e-169">String</span></span>|<span data-ttu-id="0372e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0372e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0372e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0372e-172">displayName</span></span>|<span data-ttu-id="0372e-173">String</span><span class="sxs-lookup"><span data-stu-id="0372e-173">String</span></span>|<span data-ttu-id="0372e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0372e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0372e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-176">version</span><span class="sxs-lookup"><span data-stu-id="0372e-176">version</span></span>|<span data-ttu-id="0372e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-177">Int32</span></span>|<span data-ttu-id="0372e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0372e-178">Version of the device configuration.</span></span> <span data-ttu-id="0372e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0372e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0372e-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="0372e-180">accountBlockModification</span></span>|<span data-ttu-id="0372e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-181">Boolean</span></span>|<span data-ttu-id="0372e-182">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="0372e-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="0372e-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="0372e-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-184">Boolean</span></span>|<span data-ttu-id="0372e-185">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="0372e-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="0372e-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-186">airDropBlocked</span></span>|<span data-ttu-id="0372e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-187">Boolean</span></span>|<span data-ttu-id="0372e-188">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="0372e-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="0372e-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="0372e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-190">Boolean</span></span>|<span data-ttu-id="0372e-191">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="0372e-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="0372e-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-193">Boolean</span></span>|<span data-ttu-id="0372e-194">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="0372e-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="0372e-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="0372e-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="0372e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-196">Boolean</span></span>|<span data-ttu-id="0372e-197">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="0372e-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="0372e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-199">Boolean</span></span>|<span data-ttu-id="0372e-200">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="0372e-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-201">appleNewsBlocked</span></span>|<span data-ttu-id="0372e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-202">Boolean</span></span>|<span data-ttu-id="0372e-203">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="0372e-204">appsSingleAppModeList</span></span>|<span data-ttu-id="0372e-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0372e-206">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="0372e-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="0372e-207">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="0372e-207">Supervised only.</span></span> <span data-ttu-id="0372e-208">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="0372e-208">iOS 7.0 and later.</span></span> <span data-ttu-id="0372e-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0372e-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0372e-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="0372e-210">appsVisibilityList</span></span>|<span data-ttu-id="0372e-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0372e-212">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="0372e-213">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0372e-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0372e-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="0372e-214">appsVisibilityListType</span></span>|[<span data-ttu-id="0372e-215">appListType</span><span class="sxs-lookup"><span data-stu-id="0372e-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="0372e-216">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="0372e-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="0372e-217">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="0372e-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="0372e-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="0372e-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="0372e-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-219">Boolean</span></span>|<span data-ttu-id="0372e-220">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-221">appStoreBlocked</span></span>|<span data-ttu-id="0372e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-222">Boolean</span></span>|<span data-ttu-id="0372e-223">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="0372e-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="0372e-224">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="0372e-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="0372e-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-226">Boolean</span></span>|<span data-ttu-id="0372e-227">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="0372e-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="0372e-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0372e-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="0372e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-229">Boolean</span></span>|<span data-ttu-id="0372e-230">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="0372e-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="0372e-231">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="0372e-232">appStoreRequirePassword</span></span>|<span data-ttu-id="0372e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-233">Boolean</span></span>|<span data-ttu-id="0372e-234">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="0372e-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="0372e-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="0372e-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="0372e-236">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-236">Boolean</span></span>|<span data-ttu-id="0372e-237">指示在 Safari 和其他受监督设备上应用自动填充密码和信用卡信息之前是否强制用户身份验证。</span><span class="sxs-lookup"><span data-stu-id="0372e-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="0372e-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="0372e-238">bluetoothBlockModification</span></span>|<span data-ttu-id="0372e-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-239">Boolean</span></span>|<span data-ttu-id="0372e-240">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="0372e-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-241">cameraBlocked</span></span>|<span data-ttu-id="0372e-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-242">Boolean</span></span>|<span data-ttu-id="0372e-243">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="0372e-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="0372e-244">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="0372e-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="0372e-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-246">Boolean</span></span>|<span data-ttu-id="0372e-247">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="0372e-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="0372e-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="0372e-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="0372e-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-249">Boolean</span></span>|<span data-ttu-id="0372e-250">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="0372e-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="0372e-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="0372e-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="0372e-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-252">Boolean</span></span>|<span data-ttu-id="0372e-253">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="0372e-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="0372e-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-255">Boolean</span></span>|<span data-ttu-id="0372e-256">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="0372e-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="0372e-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="0372e-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="0372e-258">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-258">Boolean</span></span>|<span data-ttu-id="0372e-259">指示是否允许用户在受监督的设备上更改手机网络计划的设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="0372e-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="0372e-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="0372e-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-261">Boolean</span></span>|<span data-ttu-id="0372e-262">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="0372e-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="0372e-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="0372e-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="0372e-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-264">Boolean</span></span>|<span data-ttu-id="0372e-265">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="0372e-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="0372e-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="0372e-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="0372e-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-267">Boolean</span></span>|<span data-ttu-id="0372e-268">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="0372e-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="0372e-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="0372e-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-270">Boolean</span></span>|<span data-ttu-id="0372e-271">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="0372e-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="0372e-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="0372e-273">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-273">Boolean</span></span>|<span data-ttu-id="0372e-274">指示设备在监督模式下时是否自动授予对教师请求的权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="0372e-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="0372e-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="0372e-276">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-276">Boolean</span></span>|<span data-ttu-id="0372e-277">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="0372e-278">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="0372e-278">Supervised only.</span></span>|
|<span data-ttu-id="0372e-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="0372e-279">compliantAppsList</span></span>|<span data-ttu-id="0372e-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0372e-281">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="0372e-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="0372e-282">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0372e-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0372e-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="0372e-283">compliantAppListType</span></span>|[<span data-ttu-id="0372e-284">appListType</span><span class="sxs-lookup"><span data-stu-id="0372e-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="0372e-285">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="0372e-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="0372e-286">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="0372e-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="0372e-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="0372e-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="0372e-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-288">Boolean</span></span>|<span data-ttu-id="0372e-289">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="0372e-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-290">definitionLookupBlocked</span></span>|<span data-ttu-id="0372e-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-291">Boolean</span></span>|<span data-ttu-id="0372e-292">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="0372e-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="0372e-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="0372e-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-294">Boolean</span></span>|<span data-ttu-id="0372e-295">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="0372e-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="0372e-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-297">Boolean</span></span>|<span data-ttu-id="0372e-298">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="0372e-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="0372e-299">deviceBlockNameModification</span></span>|<span data-ttu-id="0372e-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-300">Boolean</span></span>|<span data-ttu-id="0372e-301">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="0372e-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="0372e-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-303">Boolean</span></span>|<span data-ttu-id="0372e-304">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="0372e-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="0372e-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="0372e-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="0372e-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-306">Boolean</span></span>|<span data-ttu-id="0372e-307">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="0372e-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="0372e-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="0372e-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-309">Boolean</span></span>|<span data-ttu-id="0372e-310">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="0372e-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="0372e-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="0372e-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="0372e-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-312">Boolean</span></span>|<span data-ttu-id="0372e-313">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="0372e-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="0372e-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="0372e-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="0372e-315">String 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-315">String collection</span></span>|<span data-ttu-id="0372e-316">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="0372e-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="0372e-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="0372e-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="0372e-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-318">Boolean</span></span>|<span data-ttu-id="0372e-319">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="0372e-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="0372e-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="0372e-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="0372e-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-321">Boolean</span></span>|<span data-ttu-id="0372e-322">\[已弃用 \] 配置此设置，将值设置为"true"对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="0372e-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="0372e-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="0372e-323">esimBlockModification</span></span>|<span data-ttu-id="0372e-324">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-324">Boolean</span></span>|<span data-ttu-id="0372e-325">指示是否允许在受监督设备的 eSIM 上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="0372e-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="0372e-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-326">faceTimeBlocked</span></span>|<span data-ttu-id="0372e-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-327">Boolean</span></span>|<span data-ttu-id="0372e-328">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="0372e-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="0372e-329">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="0372e-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-331">Boolean</span></span>|<span data-ttu-id="0372e-332">指示设备在监督模式下时是否阻止对"查找我的好友"的更改。</span><span class="sxs-lookup"><span data-stu-id="0372e-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="0372e-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="0372e-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-334">Boolean</span></span>|<span data-ttu-id="0372e-335">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="0372e-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="0372e-336">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="0372e-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="0372e-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-338">Boolean</span></span>|<span data-ttu-id="0372e-339">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="0372e-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="0372e-340">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-341">gameCenterBlocked</span></span>|<span data-ttu-id="0372e-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-342">Boolean</span></span>|<span data-ttu-id="0372e-343">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="0372e-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-344">hostPairingBlocked</span></span>|<span data-ttu-id="0372e-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-345">Boolean</span></span>|<span data-ttu-id="0372e-346">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="0372e-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-348">Boolean</span></span>|<span data-ttu-id="0372e-349">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="0372e-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="0372e-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="0372e-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-351">Boolean</span></span>|<span data-ttu-id="0372e-352">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="0372e-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="0372e-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="0372e-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="0372e-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-354">Boolean</span></span>|<span data-ttu-id="0372e-355">指示是否阻止用户继续在 iOS 设备上启动的工作到其他 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="0372e-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="0372e-356">iCloudBlockBackup</span></span>|<span data-ttu-id="0372e-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-357">Boolean</span></span>|<span data-ttu-id="0372e-358">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="0372e-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="0372e-359">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="0372e-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="0372e-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-361">Boolean</span></span>|<span data-ttu-id="0372e-362">指示是否阻止 iCloud 文档同步。需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="0372e-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="0372e-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-364">Boolean</span></span>|<span data-ttu-id="0372e-365">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="0372e-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="0372e-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="0372e-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="0372e-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-367">Boolean</span></span>|<span data-ttu-id="0372e-368">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="0372e-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="0372e-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="0372e-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="0372e-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-370">Boolean</span></span>|<span data-ttu-id="0372e-371">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="0372e-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="0372e-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="0372e-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="0372e-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-373">Boolean</span></span>|<span data-ttu-id="0372e-374">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="0372e-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="0372e-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="0372e-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="0372e-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-376">Boolean</span></span>|<span data-ttu-id="0372e-377">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="0372e-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="0372e-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="0372e-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="0372e-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-379">Boolean</span></span>|<span data-ttu-id="0372e-380">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="0372e-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="0372e-381">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="0372e-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="0372e-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-383">Boolean</span></span>|<span data-ttu-id="0372e-384">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="0372e-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="0372e-385">iTunesBlockRadio</span></span>|<span data-ttu-id="0372e-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-386">Boolean</span></span>|<span data-ttu-id="0372e-387">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="0372e-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="0372e-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="0372e-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-389">Boolean</span></span>|<span data-ttu-id="0372e-390">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="0372e-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="0372e-391">keyboardBlockDictation</span></span>|<span data-ttu-id="0372e-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-392">Boolean</span></span>|<span data-ttu-id="0372e-393">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="0372e-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="0372e-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="0372e-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-395">Boolean</span></span>|<span data-ttu-id="0372e-396">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="0372e-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="0372e-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="0372e-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-398">Boolean</span></span>|<span data-ttu-id="0372e-399">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="0372e-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="0372e-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-401">Boolean</span></span>|<span data-ttu-id="0372e-402">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="0372e-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="0372e-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="0372e-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-404">Boolean</span></span>|<span data-ttu-id="0372e-405">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="0372e-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="0372e-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-407">Boolean</span></span>|<span data-ttu-id="0372e-408">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="0372e-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="0372e-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-410">Boolean</span></span>|<span data-ttu-id="0372e-411">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="0372e-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="0372e-412">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="0372e-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="0372e-413">请改为使用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="0372e-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="0372e-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="0372e-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="0372e-415">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-415">Boolean</span></span>|<span data-ttu-id="0372e-416">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="0372e-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="0372e-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-418">Boolean</span></span>|<span data-ttu-id="0372e-419">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="0372e-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="0372e-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-421">Boolean</span></span>|<span data-ttu-id="0372e-422">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="0372e-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="0372e-423">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="0372e-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="0372e-424">请改为使用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="0372e-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="0372e-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="0372e-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="0372e-426">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-426">Boolean</span></span>|<span data-ttu-id="0372e-427">指示在展台模式下是否阻止使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="0372e-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="0372e-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="0372e-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-429">Boolean</span></span>|<span data-ttu-id="0372e-430">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="0372e-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="0372e-431">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="0372e-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="0372e-432">请改为使用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="0372e-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="0372e-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="0372e-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="0372e-434">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-434">Boolean</span></span>|<span data-ttu-id="0372e-435">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="0372e-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="0372e-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="0372e-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-437">Boolean</span></span>|<span data-ttu-id="0372e-438">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="0372e-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="0372e-439">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="0372e-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="0372e-440">请改为使用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="0372e-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="0372e-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="0372e-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="0372e-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-442">Boolean</span></span>|<span data-ttu-id="0372e-443">指示在展台模式下是否阻止使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="0372e-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="0372e-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="0372e-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-445">Boolean</span></span>|<span data-ttu-id="0372e-446">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="0372e-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="0372e-447">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="0372e-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="0372e-448">请改为使用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="0372e-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="0372e-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="0372e-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="0372e-450">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-450">Boolean</span></span>|<span data-ttu-id="0372e-451">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="0372e-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="0372e-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="0372e-453">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-453">Boolean</span></span>|<span data-ttu-id="0372e-454">指示是否在展台模式下启用语音控制。</span><span class="sxs-lookup"><span data-stu-id="0372e-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="0372e-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="0372e-456">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-456">Boolean</span></span>|<span data-ttu-id="0372e-457">指示是否允许用户在展台模式下切换语音控制。</span><span class="sxs-lookup"><span data-stu-id="0372e-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="0372e-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-459">Boolean</span></span>|<span data-ttu-id="0372e-460">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="0372e-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="0372e-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-462">Boolean</span></span>|<span data-ttu-id="0372e-463">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="0372e-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="0372e-464">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="0372e-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="0372e-465">请改为使用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="0372e-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="0372e-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="0372e-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="0372e-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-467">Boolean</span></span>|<span data-ttu-id="0372e-468">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="0372e-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="0372e-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="0372e-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-470">Boolean</span></span>|<span data-ttu-id="0372e-471">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0372e-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="0372e-473">String</span><span class="sxs-lookup"><span data-stu-id="0372e-473">String</span></span>|<span data-ttu-id="0372e-474">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="0372e-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="0372e-475">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="0372e-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="0372e-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="0372e-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="0372e-477">String</span><span class="sxs-lookup"><span data-stu-id="0372e-477">String</span></span>|<span data-ttu-id="0372e-478">用于展台模式的内置应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="0372e-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="0372e-479">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="0372e-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="0372e-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="0372e-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="0372e-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-481">Boolean</span></span>|<span data-ttu-id="0372e-482">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="0372e-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="0372e-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="0372e-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-484">Boolean</span></span>|<span data-ttu-id="0372e-485">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="0372e-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="0372e-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="0372e-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-487">Boolean</span></span>|<span data-ttu-id="0372e-488">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="0372e-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="0372e-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="0372e-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-490">Boolean</span></span>|<span data-ttu-id="0372e-491">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="0372e-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="0372e-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="0372e-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-493">Boolean</span></span>|<span data-ttu-id="0372e-494">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="0372e-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="0372e-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="0372e-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="0372e-496">String</span><span class="sxs-lookup"><span data-stu-id="0372e-496">String</span></span>|<span data-ttu-id="0372e-497">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="0372e-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="0372e-498">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="0372e-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="0372e-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="0372e-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="0372e-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-500">Boolean</span></span>|<span data-ttu-id="0372e-501">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="0372e-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="0372e-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="0372e-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="0372e-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-503">Boolean</span></span>|<span data-ttu-id="0372e-504">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="0372e-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="0372e-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="0372e-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="0372e-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-506">Boolean</span></span>|<span data-ttu-id="0372e-507">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="0372e-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="0372e-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="0372e-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="0372e-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-509">Boolean</span></span>|<span data-ttu-id="0372e-510">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="0372e-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="0372e-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="0372e-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="0372e-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="0372e-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="0372e-513">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="0372e-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="0372e-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="0372e-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="0372e-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="0372e-516">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="0372e-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="0372e-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="0372e-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="0372e-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="0372e-519">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="0372e-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="0372e-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="0372e-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="0372e-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="0372e-522">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="0372e-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="0372e-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="0372e-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="0372e-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="0372e-525">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="0372e-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="0372e-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="0372e-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="0372e-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="0372e-528">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="0372e-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="0372e-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="0372e-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="0372e-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="0372e-531">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="0372e-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="0372e-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="0372e-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="0372e-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="0372e-534">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="0372e-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="0372e-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="0372e-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="0372e-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="0372e-537">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="0372e-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="0372e-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="0372e-538">networkUsageRules</span></span>|<span data-ttu-id="0372e-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="0372e-540">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="0372e-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="0372e-541">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0372e-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0372e-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="0372e-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="0372e-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="0372e-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="0372e-544">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="0372e-545">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="0372e-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="0372e-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-546">messagesBlocked</span></span>|<span data-ttu-id="0372e-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-547">Boolean</span></span>|<span data-ttu-id="0372e-548">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="0372e-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="0372e-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="0372e-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="0372e-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-550">Boolean</span></span>|<span data-ttu-id="0372e-551">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="0372e-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="0372e-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="0372e-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-553">Boolean</span></span>|<span data-ttu-id="0372e-554">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="0372e-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="0372e-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="0372e-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="0372e-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-556">Boolean</span></span>|<span data-ttu-id="0372e-557">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="0372e-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="0372e-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="0372e-558">passcodeBlockModification</span></span>|<span data-ttu-id="0372e-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-559">Boolean</span></span>|<span data-ttu-id="0372e-560">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="0372e-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0372e-561">passcodeBlockSimple</span></span>|<span data-ttu-id="0372e-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-562">Boolean</span></span>|<span data-ttu-id="0372e-563">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="0372e-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="0372e-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0372e-564">passcodeExpirationDays</span></span>|<span data-ttu-id="0372e-565">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-565">Int32</span></span>|<span data-ttu-id="0372e-566">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="0372e-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="0372e-567">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="0372e-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0372e-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0372e-568">passcodeMinimumLength</span></span>|<span data-ttu-id="0372e-569">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-569">Int32</span></span>|<span data-ttu-id="0372e-570">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="0372e-570">Minimum length of passcode.</span></span> <span data-ttu-id="0372e-571">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="0372e-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0372e-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0372e-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0372e-573">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-573">Int32</span></span>|<span data-ttu-id="0372e-574">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="0372e-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="0372e-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0372e-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0372e-576">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-576">Int32</span></span>|<span data-ttu-id="0372e-577">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="0372e-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="0372e-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0372e-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="0372e-579">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-579">Int32</span></span>|<span data-ttu-id="0372e-580">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="0372e-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="0372e-581">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="0372e-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="0372e-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="0372e-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="0372e-583">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-583">Int32</span></span>|<span data-ttu-id="0372e-584">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="0372e-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="0372e-585">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="0372e-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0372e-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="0372e-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="0372e-587">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-587">Int32</span></span>|<span data-ttu-id="0372e-588">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="0372e-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="0372e-589">有效值为 2 至 11</span><span class="sxs-lookup"><span data-stu-id="0372e-589">Valid values 2 to 11</span></span>|
|<span data-ttu-id="0372e-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="0372e-590">passcodeRequiredType</span></span>|[<span data-ttu-id="0372e-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0372e-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0372e-592">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="0372e-592">Type of passcode that is required.</span></span> <span data-ttu-id="0372e-593">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="0372e-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0372e-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="0372e-594">passcodeRequired</span></span>|<span data-ttu-id="0372e-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-595">Boolean</span></span>|<span data-ttu-id="0372e-596">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="0372e-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="0372e-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-597">podcastsBlocked</span></span>|<span data-ttu-id="0372e-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-598">Boolean</span></span>|<span data-ttu-id="0372e-599">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="0372e-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="0372e-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="0372e-601">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-601">Boolean</span></span>|<span data-ttu-id="0372e-602">指示是否启用提示以使用受监督的设备设置附近设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="0372e-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="0372e-603">safariBlockAutofill</span></span>|<span data-ttu-id="0372e-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-604">Boolean</span></span>|<span data-ttu-id="0372e-605">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="0372e-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="0372e-606">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="0372e-607">safariBlockJavaScript</span></span>|<span data-ttu-id="0372e-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-608">Boolean</span></span>|<span data-ttu-id="0372e-609">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="0372e-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="0372e-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="0372e-610">safariBlockPopups</span></span>|<span data-ttu-id="0372e-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-611">Boolean</span></span>|<span data-ttu-id="0372e-612">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="0372e-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="0372e-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-613">safariBlocked</span></span>|<span data-ttu-id="0372e-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-614">Boolean</span></span>|<span data-ttu-id="0372e-615">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="0372e-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="0372e-616">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-617">safariCookieSettings</span></span>|[<span data-ttu-id="0372e-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="0372e-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="0372e-619">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="0372e-619">Cookie settings for Safari.</span></span> <span data-ttu-id="0372e-620">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="0372e-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="0372e-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="0372e-621">safariManagedDomains</span></span>|<span data-ttu-id="0372e-622">String 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-622">String collection</span></span>|<span data-ttu-id="0372e-623">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="0372e-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="0372e-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="0372e-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="0372e-625">String 集合</span><span class="sxs-lookup"><span data-stu-id="0372e-625">String collection</span></span>|<span data-ttu-id="0372e-626">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="0372e-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="0372e-627">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="0372e-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="0372e-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="0372e-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-629">Boolean</span></span>|<span data-ttu-id="0372e-630">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="0372e-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="0372e-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-631">screenCaptureBlocked</span></span>|<span data-ttu-id="0372e-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-632">Boolean</span></span>|<span data-ttu-id="0372e-633">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="0372e-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="0372e-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-634">siriBlocked</span></span>|<span data-ttu-id="0372e-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-635">Boolean</span></span>|<span data-ttu-id="0372e-636">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="0372e-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="0372e-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="0372e-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="0372e-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-638">Boolean</span></span>|<span data-ttu-id="0372e-639">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="0372e-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="0372e-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="0372e-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="0372e-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-641">Boolean</span></span>|<span data-ttu-id="0372e-642">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="0372e-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="0372e-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="0372e-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="0372e-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-644">Boolean</span></span>|<span data-ttu-id="0372e-645">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="0372e-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="0372e-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="0372e-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="0372e-647">Int32</span><span class="sxs-lookup"><span data-stu-id="0372e-647">Int32</span></span>|<span data-ttu-id="0372e-648">设置对受监督设备取消软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="0372e-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="0372e-649">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="0372e-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="0372e-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="0372e-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="0372e-651">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-651">Boolean</span></span>|<span data-ttu-id="0372e-652">指示设备在监督模式下时是否延迟软件更新的用户可见性。</span><span class="sxs-lookup"><span data-stu-id="0372e-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="0372e-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="0372e-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="0372e-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-654">Boolean</span></span>|<span data-ttu-id="0372e-655">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="0372e-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="0372e-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-656">voiceDialingBlocked</span></span>|<span data-ttu-id="0372e-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-657">Boolean</span></span>|<span data-ttu-id="0372e-658">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="0372e-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="0372e-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="0372e-659">wallpaperBlockModification</span></span>|<span data-ttu-id="0372e-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-660">Boolean</span></span>|<span data-ttu-id="0372e-661">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="0372e-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="0372e-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="0372e-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="0372e-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-663">Boolean</span></span>|<span data-ttu-id="0372e-664">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="0372e-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="0372e-665">适用于运行 iOS 和 iPadOS 版本 14.4 及更早版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-665">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="0372e-666">运行 14.5+ 的设备应该使用设置"WiFiConnectToAllowedNetworksOnlyForced"。</span><span class="sxs-lookup"><span data-stu-id="0372e-666">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|
|<span data-ttu-id="0372e-667">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="0372e-667">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="0372e-668">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-668">Boolean</span></span>|<span data-ttu-id="0372e-669">指示通过 Classroom 参加非托管课程的学生在尝试离开 iOS 11.3 及更高版本的 (课程时是否将请求教师) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-669">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="0372e-670">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="0372e-670">keychainBlockCloudSync</span></span>|<span data-ttu-id="0372e-671">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-671">Boolean</span></span>|<span data-ttu-id="0372e-672">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="0372e-672">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="0372e-673">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-673">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-674">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="0372e-674">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="0372e-675">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-675">Boolean</span></span>|<span data-ttu-id="0372e-676">指示是否阻止非空 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="0372e-676">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="0372e-677">如果此限制设置为 false，将不会在 iOS 7.0 (禁用 CRL 和 OCSP 检查) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-677">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="0372e-678">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="0372e-678">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="0372e-679">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-679">Boolean</span></span>|<span data-ttu-id="0372e-680">指示广告跟踪是否受限。 (iOS 7.0 及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-680">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="0372e-681">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="0372e-681">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="0372e-682">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-682">Boolean</span></span>|<span data-ttu-id="0372e-683">指示是否阻止Enterprise备份书籍。</span><span class="sxs-lookup"><span data-stu-id="0372e-683">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="0372e-684">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="0372e-684">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="0372e-685">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-685">Boolean</span></span>|<span data-ttu-id="0372e-686">指示是否阻止Enterprise备注和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="0372e-686">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="0372e-687">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-687">airPrintBlocked</span></span>|<span data-ttu-id="0372e-688">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-688">Boolean</span></span>|<span data-ttu-id="0372e-689">指示 iOS 11.0 (是否阻止 AirPrint) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-689">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="0372e-690">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="0372e-690">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="0372e-691">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-691">Boolean</span></span>|<span data-ttu-id="0372e-692">指示在 iOS 11.0 及更高版本 (是否阻止用于 Airprint 的用户名和密码的密钥链) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-692">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="0372e-693">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="0372e-693">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="0372e-694">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-694">Boolean</span></span>|<span data-ttu-id="0372e-695">指示在 iOS 11.0 及更高版本中，TLS 打印通信 (信任证书) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-695">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="0372e-696">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="0372e-696">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="0372e-697">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-697">Boolean</span></span>|<span data-ttu-id="0372e-698">指示是否阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="0372e-698">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="0372e-699">这可以防止恶意的 AirPrint 蓝牙信号对 iOS 11.0 (及更高版本的网络通信进行网络钓鱼) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-699">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="0372e-700">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-700">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="0372e-701">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-701">Boolean</span></span>|<span data-ttu-id="0372e-702">指示设备是否可以使用 SMB 协议中的服务器消息块访问网络 (或其他) 资源。</span><span class="sxs-lookup"><span data-stu-id="0372e-702">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="0372e-703">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-703">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="0372e-704">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-704">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="0372e-705">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-705">Boolean</span></span>|<span data-ttu-id="0372e-706">指示具有访问权限的设备能否连接到 USB 驱动器上并打开文件。</span><span class="sxs-lookup"><span data-stu-id="0372e-706">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="0372e-707">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-707">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="0372e-708">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="0372e-708">wifiPowerOnForced</span></span>|<span data-ttu-id="0372e-709">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-709">Boolean</span></span>|<span data-ttu-id="0372e-710">指示设备是否Wi-Fi保持打开状态，即使设备处于飞行模式。</span><span class="sxs-lookup"><span data-stu-id="0372e-710">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="0372e-711">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-711">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="0372e-712">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="0372e-712">blockSystemAppRemoval</span></span>|<span data-ttu-id="0372e-713">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-713">Boolean</span></span>|<span data-ttu-id="0372e-714">指示在受监督的设备 (iOS 11.0 及更高版本上是否阻止从设备删除系统) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-714">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="0372e-715">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="0372e-715">vpnBlockCreation</span></span>|<span data-ttu-id="0372e-716">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-716">Boolean</span></span>|<span data-ttu-id="0372e-717">指示在 iOS 11.0 (或更高版本中是否阻止创建 VPN) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-717">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="0372e-718">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-718">appRemovalBlocked</span></span>|<span data-ttu-id="0372e-719">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-719">Boolean</span></span>|<span data-ttu-id="0372e-720">指示是否允许删除应用。</span><span class="sxs-lookup"><span data-stu-id="0372e-720">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="0372e-721">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-721">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="0372e-722">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-722">Boolean</span></span>|<span data-ttu-id="0372e-723">指示是否允许在 iOS 11.4.1 (设备锁定时连接到 USB) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-723">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="0372e-724">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="0372e-724">passwordBlockAutoFill</span></span>|<span data-ttu-id="0372e-725">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-725">Boolean</span></span>|<span data-ttu-id="0372e-726">指示是否允许在 iOS 12.0 (自动填充密码) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-726">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="0372e-727">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="0372e-727">passwordBlockProximityRequests</span></span>|<span data-ttu-id="0372e-728">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-728">Boolean</span></span>|<span data-ttu-id="0372e-729">指示是否阻止从 iOS 12.0 (及更高版本的附近设备请求) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-729">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="0372e-730">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="0372e-730">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="0372e-731">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-731">Boolean</span></span>|<span data-ttu-id="0372e-732">指示是否阻止使用 iOS 12.0 及更高版本的 AirDrop 密码功能共享) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-732">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="0372e-733">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="0372e-733">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="0372e-734">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-734">Boolean</span></span>|<span data-ttu-id="0372e-735">指示日期和时间"自动设置"功能是否已启用，并且用户 (iOS 12.0 及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-735">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="0372e-736">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="0372e-736">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="0372e-737">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-737">Boolean</span></span>|<span data-ttu-id="0372e-738">指示托管应用是否可以将联系人写入 iOS 12.0 及更高版本 (非托管联系人) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-738">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="0372e-739">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="0372e-739">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="0372e-740">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-740">Boolean</span></span>|<span data-ttu-id="0372e-741">指示非托管应用是否可以从 iOS 12.0 (或更高版本的托管联系人帐户) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-741">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="0372e-742">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="0372e-742">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="0372e-743">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-743">Boolean</span></span>|<span data-ttu-id="0372e-744">指示是否阻止用户修改 iOS 12.2 (或更高版本的个人热点) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-744">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="0372e-745">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-745">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="0372e-746">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-746">Boolean</span></span>|<span data-ttu-id="0372e-747">指示在 iOS 13 或更高版本的设备受监督时 (连续路径) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-747">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="0372e-748">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-748">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="0372e-749">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-749">Boolean</span></span>|<span data-ttu-id="0372e-750">指示在 iOS 13 或更高版本中监督设备时 (查找我的) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-750">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="0372e-751">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-751">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="0372e-752">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-752">Boolean</span></span>|<span data-ttu-id="0372e-753">指示在 iOS 13 或更高版本中监督设备时是否 (查找我的好友) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-753">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="0372e-754">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-754">iTunesBlocked</span></span>|<span data-ttu-id="0372e-755">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-755">Boolean</span></span>|<span data-ttu-id="0372e-756">指示是否阻止 iTunes 应用。</span><span class="sxs-lookup"><span data-stu-id="0372e-756">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="0372e-757">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-757">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="0372e-758">sharedDeviceBlockTemporarySessions</span><span class="sxs-lookup"><span data-stu-id="0372e-758">sharedDeviceBlockTemporarySessions</span></span>|<span data-ttu-id="0372e-759">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-759">Boolean</span></span>|<span data-ttu-id="0372e-760">指示是否阻止 iOS 13.4 或更高版本上的共享 iPad (临时) 。</span><span class="sxs-lookup"><span data-stu-id="0372e-760">Indicates whether or not to block temporary sessions on Shared iPads (iOS 13.4 or later).</span></span>|
|<span data-ttu-id="0372e-761">appClipsBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-761">appClipsBlocked</span></span>|<span data-ttu-id="0372e-762">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-762">Boolean</span></span>|<span data-ttu-id="0372e-763">阻止用户添加任何应用剪辑并删除设备上的任何现有应用剪辑。</span><span class="sxs-lookup"><span data-stu-id="0372e-763">Prevents a user from adding any App Clips and removes any existing App Clips on the device.</span></span>|
|<span data-ttu-id="0372e-764">applePersonalizedAdsBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-764">applePersonalizedAdsBlocked</span></span>|<span data-ttu-id="0372e-765">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-765">Boolean</span></span>|<span data-ttu-id="0372e-766">如果为 true，限制 Apple 个性化广告。</span><span class="sxs-lookup"><span data-stu-id="0372e-766">Limits Apple personalized advertising when true.</span></span> <span data-ttu-id="0372e-767">在 iOS 14 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="0372e-767">Available in iOS 14 and later.</span></span>|
|<span data-ttu-id="0372e-768">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-768">nfcBlocked</span></span>|<span data-ttu-id="0372e-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="0372e-769">Boolean</span></span>|<span data-ttu-id="0372e-770">禁用 NFC 以防止设备与其他支持 NFC 的设备配对。</span><span class="sxs-lookup"><span data-stu-id="0372e-770">Disable NFC to prevent devices from pairing with other NFC-enabled devices.</span></span> <span data-ttu-id="0372e-771">适用于运行 14.2 及更高版本的 iOS/iPadOS 设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-771">Available for iOS/iPadOS devices running 14.2 and later.</span></span>|
|<span data-ttu-id="0372e-772">autoUnlockBlocked</span><span class="sxs-lookup"><span data-stu-id="0372e-772">autoUnlockBlocked</span></span>|<span data-ttu-id="0372e-773">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-773">Boolean</span></span>|<span data-ttu-id="0372e-774">阻止用户使用 Apple Watch 解锁其设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-774">Blocks users from unlocking their device with Apple Watch.</span></span> <span data-ttu-id="0372e-775">适用于运行 iOS 和 iPadOS 版本 14.5 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-775">Available for devices running iOS and iPadOS versions 14.5 and later.</span></span>|
|<span data-ttu-id="0372e-776">unpairedExternalBootToRecoveryAllowed</span><span class="sxs-lookup"><span data-stu-id="0372e-776">unpairedExternalBootToRecoveryAllowed</span></span>|<span data-ttu-id="0372e-777">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-777">Boolean</span></span>|<span data-ttu-id="0372e-778">允许用户使用未配对的设备将设备启动到恢复模式。</span><span class="sxs-lookup"><span data-stu-id="0372e-778">Allow users to boot devices into recovery mode with unpaired devices.</span></span> <span data-ttu-id="0372e-779">适用于运行 iOS 和 iPadOS 版本 14.5 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-779">Available for devices running iOS and iPadOS versions 14.5 and later.</span></span>|
|<span data-ttu-id="0372e-780">onDeviceOnlyDictationForced</span><span class="sxs-lookup"><span data-stu-id="0372e-780">onDeviceOnlyDictationForced</span></span>|<span data-ttu-id="0372e-781">布尔值</span><span class="sxs-lookup"><span data-stu-id="0372e-781">Boolean</span></span>|<span data-ttu-id="0372e-782">禁用与 Siri 服务器的连接，以便用户不能使用 Siri 听写文本。</span><span class="sxs-lookup"><span data-stu-id="0372e-782">Disables connections to Siri servers so that users can’t use Siri to dictate text.</span></span> <span data-ttu-id="0372e-783">适用于运行 iOS 和 iPadOS 版本 14.5 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="0372e-783">Available for devices running iOS and iPadOS versions 14.5 and later.</span></span>|
|<span data-ttu-id="0372e-784">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="0372e-784">kioskModeAppType</span></span>|[<span data-ttu-id="0372e-785">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="0372e-785">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="0372e-786">在展台模式下运行的应用类型。</span><span class="sxs-lookup"><span data-stu-id="0372e-786">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="0372e-787">可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。</span><span class="sxs-lookup"><span data-stu-id="0372e-787">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="0372e-788">响应</span><span class="sxs-lookup"><span data-stu-id="0372e-788">Response</span></span>
<span data-ttu-id="0372e-789">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0372e-789">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0372e-790">示例</span><span class="sxs-lookup"><span data-stu-id="0372e-790">Example</span></span>

### <a name="request"></a><span data-ttu-id="0372e-791">请求</span><span class="sxs-lookup"><span data-stu-id="0372e-791">Request</span></span>
<span data-ttu-id="0372e-792">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0372e-792">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10776

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
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="0372e-793">响应</span><span class="sxs-lookup"><span data-stu-id="0372e-793">Response</span></span>
<span data-ttu-id="0372e-p163">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0372e-p163">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10948

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
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "kioskModeAppType": "appStoreApp"
}
```




