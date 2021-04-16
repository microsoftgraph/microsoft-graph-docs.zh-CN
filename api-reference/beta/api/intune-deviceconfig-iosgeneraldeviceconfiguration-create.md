---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d0bc5f13e04576fe1095c352aa2c1063c5addf4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865696"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d1f7d-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1f7d-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d1f7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1f7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1f7d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1f7d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1f7d-107">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1f7d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1f7d-108">Prerequisites</span></span>
<span data-ttu-id="d1f7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f7d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1f7d-111">Permission type</span></span>|<span data-ttu-id="d1f7d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1f7d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1f7d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1f7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1f7d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f7d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1f7d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1f7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1f7d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-116">Not supported.</span></span>|
|<span data-ttu-id="d1f7d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1f7d-117">Application</span></span>|<span data-ttu-id="d1f7d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f7d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1f7d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1f7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1f7d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1f7d-120">Request headers</span></span>
|<span data-ttu-id="d1f7d-121">标头</span><span class="sxs-lookup"><span data-stu-id="d1f7d-121">Header</span></span>|<span data-ttu-id="d1f7d-122">值</span><span class="sxs-lookup"><span data-stu-id="d1f7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1f7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1f7d-123">Authorization</span></span>|<span data-ttu-id="d1f7d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1f7d-125">接受</span><span class="sxs-lookup"><span data-stu-id="d1f7d-125">Accept</span></span>|<span data-ttu-id="d1f7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1f7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f7d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1f7d-127">Request body</span></span>
<span data-ttu-id="d1f7d-128">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d1f7d-129">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d1f7d-130">属性</span><span class="sxs-lookup"><span data-stu-id="d1f7d-130">Property</span></span>|<span data-ttu-id="d1f7d-131">类型</span><span class="sxs-lookup"><span data-stu-id="d1f7d-131">Type</span></span>|<span data-ttu-id="d1f7d-132">说明</span><span class="sxs-lookup"><span data-stu-id="d1f7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f7d-133">id</span><span class="sxs-lookup"><span data-stu-id="d1f7d-133">id</span></span>|<span data-ttu-id="d1f7d-134">String</span><span class="sxs-lookup"><span data-stu-id="d1f7d-134">String</span></span>|<span data-ttu-id="d1f7d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-135">Key of the entity.</span></span> <span data-ttu-id="d1f7d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1f7d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d1f7d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1f7d-138">DateTimeOffset</span></span>|<span data-ttu-id="d1f7d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d1f7d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d1f7d-141">roleScopeTagIds</span></span>|<span data-ttu-id="d1f7d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-142">String collection</span></span>|<span data-ttu-id="d1f7d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1f7d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1f7d-145">supportsScopeTags</span></span>|<span data-ttu-id="d1f7d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-146">Boolean</span></span>|<span data-ttu-id="d1f7d-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1f7d-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1f7d-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1f7d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-150">This property is read-only.</span></span> <span data-ttu-id="d1f7d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1f7d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d1f7d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1f7d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d1f7d-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d1f7d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1f7d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d1f7d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1f7d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d1f7d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d1f7d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1f7d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d1f7d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1f7d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d1f7d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d1f7d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1f7d-164">createdDateTime</span></span>|<span data-ttu-id="d1f7d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1f7d-165">DateTimeOffset</span></span>|<span data-ttu-id="d1f7d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-166">DateTime the object was created.</span></span> <span data-ttu-id="d1f7d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-168">说明</span><span class="sxs-lookup"><span data-stu-id="d1f7d-168">description</span></span>|<span data-ttu-id="d1f7d-169">String</span><span class="sxs-lookup"><span data-stu-id="d1f7d-169">String</span></span>|<span data-ttu-id="d1f7d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1f7d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d1f7d-172">displayName</span></span>|<span data-ttu-id="d1f7d-173">String</span><span class="sxs-lookup"><span data-stu-id="d1f7d-173">String</span></span>|<span data-ttu-id="d1f7d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1f7d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-176">version</span><span class="sxs-lookup"><span data-stu-id="d1f7d-176">version</span></span>|<span data-ttu-id="d1f7d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-177">Int32</span></span>|<span data-ttu-id="d1f7d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-178">Version of the device configuration.</span></span> <span data-ttu-id="d1f7d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f7d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f7d-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-180">accountBlockModification</span></span>|<span data-ttu-id="d1f7d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-181">Boolean</span></span>|<span data-ttu-id="d1f7d-182">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="d1f7d-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="d1f7d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-184">Boolean</span></span>|<span data-ttu-id="d1f7d-185">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-186">airDropBlocked</span></span>|<span data-ttu-id="d1f7d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-187">Boolean</span></span>|<span data-ttu-id="d1f7d-188">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="d1f7d-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="d1f7d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-190">Boolean</span></span>|<span data-ttu-id="d1f7d-191">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="d1f7d-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="d1f7d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-193">Boolean</span></span>|<span data-ttu-id="d1f7d-194">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="d1f7d-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="d1f7d-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="d1f7d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-196">Boolean</span></span>|<span data-ttu-id="d1f7d-197">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="d1f7d-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="d1f7d-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-199">Boolean</span></span>|<span data-ttu-id="d1f7d-200">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="d1f7d-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-201">appleNewsBlocked</span></span>|<span data-ttu-id="d1f7d-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-202">Boolean</span></span>|<span data-ttu-id="d1f7d-203">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="d1f7d-204">appsSingleAppModeList</span></span>|<span data-ttu-id="d1f7d-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d1f7d-206">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="d1f7d-207">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-207">Supervised only.</span></span> <span data-ttu-id="d1f7d-208">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-208">iOS 7.0 and later.</span></span> <span data-ttu-id="d1f7d-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d1f7d-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="d1f7d-210">appsVisibilityList</span></span>|<span data-ttu-id="d1f7d-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d1f7d-212">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="d1f7d-213">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d1f7d-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-214">appsVisibilityListType</span></span>|[<span data-ttu-id="d1f7d-215">appListType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d1f7d-216">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="d1f7d-217">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d1f7d-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="d1f7d-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="d1f7d-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-219">Boolean</span></span>|<span data-ttu-id="d1f7d-220">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-221">appStoreBlocked</span></span>|<span data-ttu-id="d1f7d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-222">Boolean</span></span>|<span data-ttu-id="d1f7d-223">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="d1f7d-224">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="d1f7d-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="d1f7d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-226">Boolean</span></span>|<span data-ttu-id="d1f7d-227">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="d1f7d-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="d1f7d-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-229">Boolean</span></span>|<span data-ttu-id="d1f7d-230">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="d1f7d-231">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d1f7d-232">appStoreRequirePassword</span></span>|<span data-ttu-id="d1f7d-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-233">Boolean</span></span>|<span data-ttu-id="d1f7d-234">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="d1f7d-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="d1f7d-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="d1f7d-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-236">Boolean</span></span>|<span data-ttu-id="d1f7d-237">指示在 Safari 和其他受监督设备上应用自动填充密码和信用卡信息之前是否强制用户身份验证。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="d1f7d-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-238">bluetoothBlockModification</span></span>|<span data-ttu-id="d1f7d-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-239">Boolean</span></span>|<span data-ttu-id="d1f7d-240">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-241">cameraBlocked</span></span>|<span data-ttu-id="d1f7d-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-242">Boolean</span></span>|<span data-ttu-id="d1f7d-243">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="d1f7d-244">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d1f7d-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d1f7d-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-246">Boolean</span></span>|<span data-ttu-id="d1f7d-247">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d1f7d-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="d1f7d-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="d1f7d-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-249">Boolean</span></span>|<span data-ttu-id="d1f7d-250">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="d1f7d-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="d1f7d-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-252">Boolean</span></span>|<span data-ttu-id="d1f7d-253">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="d1f7d-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="d1f7d-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-255">Boolean</span></span>|<span data-ttu-id="d1f7d-256">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="d1f7d-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="d1f7d-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-258">Boolean</span></span>|<span data-ttu-id="d1f7d-259">指示是否允许用户在受监督的设备上更改手机网络计划的设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="d1f7d-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d1f7d-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d1f7d-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-261">Boolean</span></span>|<span data-ttu-id="d1f7d-262">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d1f7d-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="d1f7d-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="d1f7d-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-264">Boolean</span></span>|<span data-ttu-id="d1f7d-265">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="d1f7d-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d1f7d-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-267">Boolean</span></span>|<span data-ttu-id="d1f7d-268">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d1f7d-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-270">Boolean</span></span>|<span data-ttu-id="d1f7d-271">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="d1f7d-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="d1f7d-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-273">Boolean</span></span>|<span data-ttu-id="d1f7d-274">指示设备在监督模式下时是否自动授予对教师请求的权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d1f7d-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="d1f7d-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-276">Boolean</span></span>|<span data-ttu-id="d1f7d-277">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="d1f7d-278">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-278">Supervised only.</span></span>|
|<span data-ttu-id="d1f7d-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d1f7d-279">compliantAppsList</span></span>|<span data-ttu-id="d1f7d-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d1f7d-281">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d1f7d-282">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d1f7d-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-283">compliantAppListType</span></span>|[<span data-ttu-id="d1f7d-284">appListType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d1f7d-285">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d1f7d-286">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d1f7d-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d1f7d-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="d1f7d-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-288">Boolean</span></span>|<span data-ttu-id="d1f7d-289">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-290">definitionLookupBlocked</span></span>|<span data-ttu-id="d1f7d-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-291">Boolean</span></span>|<span data-ttu-id="d1f7d-292">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="d1f7d-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="d1f7d-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="d1f7d-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-294">Boolean</span></span>|<span data-ttu-id="d1f7d-295">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="d1f7d-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-297">Boolean</span></span>|<span data-ttu-id="d1f7d-298">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-299">deviceBlockNameModification</span></span>|<span data-ttu-id="d1f7d-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-300">Boolean</span></span>|<span data-ttu-id="d1f7d-301">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d1f7d-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d1f7d-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-303">Boolean</span></span>|<span data-ttu-id="d1f7d-304">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d1f7d-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="d1f7d-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-306">Boolean</span></span>|<span data-ttu-id="d1f7d-307">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="d1f7d-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="d1f7d-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="d1f7d-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-309">Boolean</span></span>|<span data-ttu-id="d1f7d-310">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="d1f7d-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="d1f7d-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="d1f7d-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-312">Boolean</span></span>|<span data-ttu-id="d1f7d-313">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="d1f7d-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d1f7d-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="d1f7d-315">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-315">String collection</span></span>|<span data-ttu-id="d1f7d-316">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d1f7d-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="d1f7d-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="d1f7d-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-318">Boolean</span></span>|<span data-ttu-id="d1f7d-319">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="d1f7d-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="d1f7d-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-321">Boolean</span></span>|<span data-ttu-id="d1f7d-322">\[已弃用 \] 配置此设置，将值设置为"true"对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="d1f7d-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-323">esimBlockModification</span></span>|<span data-ttu-id="d1f7d-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-324">Boolean</span></span>|<span data-ttu-id="d1f7d-325">指示是否允许在受监督设备的 eSIM 上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="d1f7d-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-326">faceTimeBlocked</span></span>|<span data-ttu-id="d1f7d-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-327">Boolean</span></span>|<span data-ttu-id="d1f7d-328">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="d1f7d-329">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="d1f7d-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-331">Boolean</span></span>|<span data-ttu-id="d1f7d-332">指示设备在监督模式下时是否阻止对"查找我的好友"的更改。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="d1f7d-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="d1f7d-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-334">Boolean</span></span>|<span data-ttu-id="d1f7d-335">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="d1f7d-336">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="d1f7d-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="d1f7d-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-338">Boolean</span></span>|<span data-ttu-id="d1f7d-339">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="d1f7d-340">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-341">gameCenterBlocked</span></span>|<span data-ttu-id="d1f7d-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-342">Boolean</span></span>|<span data-ttu-id="d1f7d-343">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-344">hostPairingBlocked</span></span>|<span data-ttu-id="d1f7d-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-345">Boolean</span></span>|<span data-ttu-id="d1f7d-346">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="d1f7d-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-348">Boolean</span></span>|<span data-ttu-id="d1f7d-349">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="d1f7d-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="d1f7d-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-351">Boolean</span></span>|<span data-ttu-id="d1f7d-352">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="d1f7d-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d1f7d-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-354">Boolean</span></span>|<span data-ttu-id="d1f7d-355">指示是否阻止用户继续在 iOS 设备上启动的工作到其他 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="d1f7d-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d1f7d-356">iCloudBlockBackup</span></span>|<span data-ttu-id="d1f7d-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-357">Boolean</span></span>|<span data-ttu-id="d1f7d-358">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="d1f7d-359">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d1f7d-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d1f7d-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-361">Boolean</span></span>|<span data-ttu-id="d1f7d-362">指示是否阻止 iCloud 文档同步。需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="d1f7d-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="d1f7d-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-364">Boolean</span></span>|<span data-ttu-id="d1f7d-365">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="d1f7d-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d1f7d-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d1f7d-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-367">Boolean</span></span>|<span data-ttu-id="d1f7d-368">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d1f7d-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="d1f7d-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="d1f7d-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-370">Boolean</span></span>|<span data-ttu-id="d1f7d-371">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="d1f7d-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="d1f7d-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="d1f7d-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-373">Boolean</span></span>|<span data-ttu-id="d1f7d-374">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="d1f7d-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="d1f7d-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="d1f7d-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-376">Boolean</span></span>|<span data-ttu-id="d1f7d-377">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="d1f7d-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="d1f7d-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="d1f7d-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-379">Boolean</span></span>|<span data-ttu-id="d1f7d-380">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="d1f7d-381">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d1f7d-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="d1f7d-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-383">Boolean</span></span>|<span data-ttu-id="d1f7d-384">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d1f7d-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="d1f7d-385">iTunesBlockRadio</span></span>|<span data-ttu-id="d1f7d-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-386">Boolean</span></span>|<span data-ttu-id="d1f7d-387">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="d1f7d-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="d1f7d-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-389">Boolean</span></span>|<span data-ttu-id="d1f7d-390">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-391">keyboardBlockDictation</span></span>|<span data-ttu-id="d1f7d-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-392">Boolean</span></span>|<span data-ttu-id="d1f7d-393">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="d1f7d-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="d1f7d-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-395">Boolean</span></span>|<span data-ttu-id="d1f7d-396">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="d1f7d-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="d1f7d-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-398">Boolean</span></span>|<span data-ttu-id="d1f7d-399">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="d1f7d-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="d1f7d-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-401">Boolean</span></span>|<span data-ttu-id="d1f7d-402">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="d1f7d-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="d1f7d-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-404">Boolean</span></span>|<span data-ttu-id="d1f7d-405">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="d1f7d-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-407">Boolean</span></span>|<span data-ttu-id="d1f7d-408">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="d1f7d-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="d1f7d-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-410">Boolean</span></span>|<span data-ttu-id="d1f7d-411">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="d1f7d-412">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d1f7d-413">请改为使用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="d1f7d-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="d1f7d-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="d1f7d-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-415">Boolean</span></span>|<span data-ttu-id="d1f7d-416">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="d1f7d-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-418">Boolean</span></span>|<span data-ttu-id="d1f7d-419">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d1f7d-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="d1f7d-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-421">Boolean</span></span>|<span data-ttu-id="d1f7d-422">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="d1f7d-423">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d1f7d-424">请改为使用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="d1f7d-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d1f7d-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="d1f7d-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-426">Boolean</span></span>|<span data-ttu-id="d1f7d-427">指示在展台模式下是否阻止使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="d1f7d-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-429">Boolean</span></span>|<span data-ttu-id="d1f7d-430">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="d1f7d-431">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d1f7d-432">请改为使用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="d1f7d-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="d1f7d-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-434">Boolean</span></span>|<span data-ttu-id="d1f7d-435">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="d1f7d-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="d1f7d-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-437">Boolean</span></span>|<span data-ttu-id="d1f7d-438">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="d1f7d-439">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d1f7d-440">请改为使用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="d1f7d-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="d1f7d-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="d1f7d-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-442">Boolean</span></span>|<span data-ttu-id="d1f7d-443">指示在展台模式下是否阻止使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d1f7d-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="d1f7d-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-445">Boolean</span></span>|<span data-ttu-id="d1f7d-446">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="d1f7d-447">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d1f7d-448">请改为使用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="d1f7d-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d1f7d-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="d1f7d-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-450">Boolean</span></span>|<span data-ttu-id="d1f7d-451">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="d1f7d-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="d1f7d-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-453">Boolean</span></span>|<span data-ttu-id="d1f7d-454">指示是否在展台模式下启用语音控制。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="d1f7d-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-456">Boolean</span></span>|<span data-ttu-id="d1f7d-457">指示是否允许用户在展台模式下切换语音控制。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="d1f7d-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-459">Boolean</span></span>|<span data-ttu-id="d1f7d-460">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d1f7d-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="d1f7d-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-462">Boolean</span></span>|<span data-ttu-id="d1f7d-463">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="d1f7d-464">对于操作系统默认设置，此属性的功能是多余的，并且已弃用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d1f7d-465">请改为使用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="d1f7d-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d1f7d-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="d1f7d-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-467">Boolean</span></span>|<span data-ttu-id="d1f7d-468">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="d1f7d-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="d1f7d-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-470">Boolean</span></span>|<span data-ttu-id="d1f7d-471">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d1f7d-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="d1f7d-473">String</span><span class="sxs-lookup"><span data-stu-id="d1f7d-473">String</span></span>|<span data-ttu-id="d1f7d-474">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="d1f7d-475">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="d1f7d-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="d1f7d-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="d1f7d-477">String</span><span class="sxs-lookup"><span data-stu-id="d1f7d-477">String</span></span>|<span data-ttu-id="d1f7d-478">用于展台模式的内置应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="d1f7d-479">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="d1f7d-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="d1f7d-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="d1f7d-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-481">Boolean</span></span>|<span data-ttu-id="d1f7d-482">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="d1f7d-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="d1f7d-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-484">Boolean</span></span>|<span data-ttu-id="d1f7d-485">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="d1f7d-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="d1f7d-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-487">Boolean</span></span>|<span data-ttu-id="d1f7d-488">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="d1f7d-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="d1f7d-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-490">Boolean</span></span>|<span data-ttu-id="d1f7d-491">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="d1f7d-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="d1f7d-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-493">Boolean</span></span>|<span data-ttu-id="d1f7d-494">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="d1f7d-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="d1f7d-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="d1f7d-496">String</span><span class="sxs-lookup"><span data-stu-id="d1f7d-496">String</span></span>|<span data-ttu-id="d1f7d-497">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="d1f7d-498">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="d1f7d-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="d1f7d-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="d1f7d-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-500">Boolean</span></span>|<span data-ttu-id="d1f7d-501">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="d1f7d-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="d1f7d-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="d1f7d-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-503">Boolean</span></span>|<span data-ttu-id="d1f7d-504">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="d1f7d-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="d1f7d-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="d1f7d-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-506">Boolean</span></span>|<span data-ttu-id="d1f7d-507">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="d1f7d-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="d1f7d-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="d1f7d-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-509">Boolean</span></span>|<span data-ttu-id="d1f7d-510">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="d1f7d-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d1f7d-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="d1f7d-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d1f7d-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="d1f7d-513">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="d1f7d-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d1f7d-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="d1f7d-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d1f7d-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="d1f7d-516">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="d1f7d-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d1f7d-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="d1f7d-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d1f7d-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="d1f7d-519">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="d1f7d-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d1f7d-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="d1f7d-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d1f7d-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="d1f7d-522">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="d1f7d-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d1f7d-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="d1f7d-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d1f7d-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="d1f7d-525">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="d1f7d-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d1f7d-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="d1f7d-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d1f7d-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="d1f7d-528">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="d1f7d-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d1f7d-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="d1f7d-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d1f7d-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="d1f7d-531">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="d1f7d-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d1f7d-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="d1f7d-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d1f7d-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="d1f7d-534">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="d1f7d-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d1f7d-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="d1f7d-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d1f7d-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="d1f7d-537">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="d1f7d-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="d1f7d-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="d1f7d-538">networkUsageRules</span></span>|<span data-ttu-id="d1f7d-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="d1f7d-540">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="d1f7d-541">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d1f7d-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="d1f7d-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="d1f7d-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="d1f7d-544">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="d1f7d-545">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="d1f7d-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-546">messagesBlocked</span></span>|<span data-ttu-id="d1f7d-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-547">Boolean</span></span>|<span data-ttu-id="d1f7d-548">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="d1f7d-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="d1f7d-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-550">Boolean</span></span>|<span data-ttu-id="d1f7d-551">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d1f7d-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="d1f7d-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-553">Boolean</span></span>|<span data-ttu-id="d1f7d-554">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d1f7d-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="d1f7d-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-556">Boolean</span></span>|<span data-ttu-id="d1f7d-557">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-558">passcodeBlockModification</span></span>|<span data-ttu-id="d1f7d-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-559">Boolean</span></span>|<span data-ttu-id="d1f7d-560">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d1f7d-561">passcodeBlockSimple</span></span>|<span data-ttu-id="d1f7d-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-562">Boolean</span></span>|<span data-ttu-id="d1f7d-563">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="d1f7d-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d1f7d-564">passcodeExpirationDays</span></span>|<span data-ttu-id="d1f7d-565">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-565">Int32</span></span>|<span data-ttu-id="d1f7d-566">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="d1f7d-567">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="d1f7d-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d1f7d-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d1f7d-568">passcodeMinimumLength</span></span>|<span data-ttu-id="d1f7d-569">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-569">Int32</span></span>|<span data-ttu-id="d1f7d-570">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-570">Minimum length of passcode.</span></span> <span data-ttu-id="d1f7d-571">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="d1f7d-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d1f7d-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d1f7d-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d1f7d-573">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-573">Int32</span></span>|<span data-ttu-id="d1f7d-574">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="d1f7d-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d1f7d-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d1f7d-576">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-576">Int32</span></span>|<span data-ttu-id="d1f7d-577">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d1f7d-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d1f7d-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="d1f7d-579">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-579">Int32</span></span>|<span data-ttu-id="d1f7d-580">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="d1f7d-581">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="d1f7d-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d1f7d-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="d1f7d-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="d1f7d-583">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-583">Int32</span></span>|<span data-ttu-id="d1f7d-584">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="d1f7d-585">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="d1f7d-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d1f7d-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="d1f7d-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="d1f7d-587">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-587">Int32</span></span>|<span data-ttu-id="d1f7d-588">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="d1f7d-589">有效值为 2 至 11</span><span class="sxs-lookup"><span data-stu-id="d1f7d-589">Valid values 2 to 11</span></span>|
|<span data-ttu-id="d1f7d-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-590">passcodeRequiredType</span></span>|[<span data-ttu-id="d1f7d-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d1f7d-592">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-592">Type of passcode that is required.</span></span> <span data-ttu-id="d1f7d-593">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d1f7d-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="d1f7d-594">passcodeRequired</span></span>|<span data-ttu-id="d1f7d-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-595">Boolean</span></span>|<span data-ttu-id="d1f7d-596">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="d1f7d-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-597">podcastsBlocked</span></span>|<span data-ttu-id="d1f7d-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-598">Boolean</span></span>|<span data-ttu-id="d1f7d-599">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="d1f7d-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="d1f7d-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-601">Boolean</span></span>|<span data-ttu-id="d1f7d-602">指示是否启用提示以使用受监督的设备设置附近设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="d1f7d-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d1f7d-603">safariBlockAutofill</span></span>|<span data-ttu-id="d1f7d-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-604">Boolean</span></span>|<span data-ttu-id="d1f7d-605">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="d1f7d-606">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d1f7d-607">safariBlockJavaScript</span></span>|<span data-ttu-id="d1f7d-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-608">Boolean</span></span>|<span data-ttu-id="d1f7d-609">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="d1f7d-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d1f7d-610">safariBlockPopups</span></span>|<span data-ttu-id="d1f7d-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-611">Boolean</span></span>|<span data-ttu-id="d1f7d-612">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="d1f7d-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-613">safariBlocked</span></span>|<span data-ttu-id="d1f7d-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-614">Boolean</span></span>|<span data-ttu-id="d1f7d-615">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="d1f7d-616">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-617">safariCookieSettings</span></span>|[<span data-ttu-id="d1f7d-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d1f7d-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="d1f7d-619">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-619">Cookie settings for Safari.</span></span> <span data-ttu-id="d1f7d-620">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="d1f7d-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="d1f7d-621">safariManagedDomains</span></span>|<span data-ttu-id="d1f7d-622">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-622">String collection</span></span>|<span data-ttu-id="d1f7d-623">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="d1f7d-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="d1f7d-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="d1f7d-625">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1f7d-625">String collection</span></span>|<span data-ttu-id="d1f7d-626">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="d1f7d-627">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d1f7d-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="d1f7d-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-629">Boolean</span></span>|<span data-ttu-id="d1f7d-630">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="d1f7d-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-631">screenCaptureBlocked</span></span>|<span data-ttu-id="d1f7d-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-632">Boolean</span></span>|<span data-ttu-id="d1f7d-633">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d1f7d-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-634">siriBlocked</span></span>|<span data-ttu-id="d1f7d-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-635">Boolean</span></span>|<span data-ttu-id="d1f7d-636">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="d1f7d-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="d1f7d-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-638">Boolean</span></span>|<span data-ttu-id="d1f7d-639">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="d1f7d-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="d1f7d-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="d1f7d-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-641">Boolean</span></span>|<span data-ttu-id="d1f7d-642">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="d1f7d-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="d1f7d-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="d1f7d-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-644">Boolean</span></span>|<span data-ttu-id="d1f7d-645">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="d1f7d-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="d1f7d-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="d1f7d-647">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f7d-647">Int32</span></span>|<span data-ttu-id="d1f7d-648">设置对受监督设备取消软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="d1f7d-649">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="d1f7d-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="d1f7d-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="d1f7d-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="d1f7d-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-651">Boolean</span></span>|<span data-ttu-id="d1f7d-652">指示设备在监督模式下时是否延迟软件更新的用户可见性。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d1f7d-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d1f7d-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-654">Boolean</span></span>|<span data-ttu-id="d1f7d-655">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="d1f7d-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-656">voiceDialingBlocked</span></span>|<span data-ttu-id="d1f7d-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-657">Boolean</span></span>|<span data-ttu-id="d1f7d-658">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d1f7d-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-659">wallpaperBlockModification</span></span>|<span data-ttu-id="d1f7d-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-660">Boolean</span></span>|<span data-ttu-id="d1f7d-661">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="d1f7d-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="d1f7d-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="d1f7d-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-663">Boolean</span></span>|<span data-ttu-id="d1f7d-664">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d1f7d-665">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="d1f7d-665">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="d1f7d-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-666">Boolean</span></span>|<span data-ttu-id="d1f7d-667">指示通过 Classroom 参加非托管课程的学生在尝试离开 iOS 11.3 及更高版本的 (课程时是否将请求教师) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-667">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="d1f7d-668">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="d1f7d-668">keychainBlockCloudSync</span></span>|<span data-ttu-id="d1f7d-669">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-669">Boolean</span></span>|<span data-ttu-id="d1f7d-670">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-670">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="d1f7d-671">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-671">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-672">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="d1f7d-672">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="d1f7d-673">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-673">Boolean</span></span>|<span data-ttu-id="d1f7d-674">指示是否阻止非空 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-674">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="d1f7d-675">如果此限制设置为 false，将不会在 iOS 7.0 (禁用 CRL 和 OCSP 检查) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-675">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-676">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="d1f7d-676">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="d1f7d-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-677">Boolean</span></span>|<span data-ttu-id="d1f7d-678">指示广告跟踪是否受限。 (iOS 7.0 及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-678">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-679">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d1f7d-679">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="d1f7d-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-680">Boolean</span></span>|<span data-ttu-id="d1f7d-681">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-681">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="d1f7d-682">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="d1f7d-682">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="d1f7d-683">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-683">Boolean</span></span>|<span data-ttu-id="d1f7d-684">指示是否阻止企业书籍备注和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-684">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="d1f7d-685">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-685">airPrintBlocked</span></span>|<span data-ttu-id="d1f7d-686">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-686">Boolean</span></span>|<span data-ttu-id="d1f7d-687">指示 iOS 11.0 (是否阻止 AirPrint) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-687">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-688">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="d1f7d-688">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="d1f7d-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-689">Boolean</span></span>|<span data-ttu-id="d1f7d-690">指示在 iOS 11.0 及更高版本 (是否阻止用于 Airprint 的用户名和密码的密钥链) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-690">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-691">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="d1f7d-691">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="d1f7d-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-692">Boolean</span></span>|<span data-ttu-id="d1f7d-693">指示在 iOS 11.0 及更高版本中，TLS 打印通信 (信任证书) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-693">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-694">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="d1f7d-694">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="d1f7d-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-695">Boolean</span></span>|<span data-ttu-id="d1f7d-696">指示是否阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-696">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="d1f7d-697">这可以防止恶意的 AirPrint Bluetooth信号对 iOS 11.0 (及更高版本的网络通信进行网络钓鱼) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-697">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-698">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-698">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="d1f7d-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-699">Boolean</span></span>|<span data-ttu-id="d1f7d-700">指示设备是否可以使用 SMB 协议中的服务器消息块访问网络 (或其他) 资源。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-700">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="d1f7d-701">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-701">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d1f7d-702">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-702">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="d1f7d-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-703">Boolean</span></span>|<span data-ttu-id="d1f7d-704">指示具有访问权限的设备能否连接到 USB 驱动器上并打开文件。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-704">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="d1f7d-705">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-705">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d1f7d-706">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="d1f7d-706">wifiPowerOnForced</span></span>|<span data-ttu-id="d1f7d-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-707">Boolean</span></span>|<span data-ttu-id="d1f7d-708">指示设备是否Wi-Fi保持打开状态，即使设备处于飞行模式。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-708">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="d1f7d-709">适用于运行 iOS 和 iPadOS 版本 13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-709">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d1f7d-710">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="d1f7d-710">blockSystemAppRemoval</span></span>|<span data-ttu-id="d1f7d-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-711">Boolean</span></span>|<span data-ttu-id="d1f7d-712">指示在受监督的设备 (iOS 11.0 及更高版本上是否阻止从设备删除系统) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-712">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-713">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="d1f7d-713">vpnBlockCreation</span></span>|<span data-ttu-id="d1f7d-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-714">Boolean</span></span>|<span data-ttu-id="d1f7d-715">指示在 iOS 11.0 (或更高版本中是否阻止创建 VPN) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-715">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-716">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-716">appRemovalBlocked</span></span>|<span data-ttu-id="d1f7d-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-717">Boolean</span></span>|<span data-ttu-id="d1f7d-718">指示是否允许删除应用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-718">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="d1f7d-719">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-719">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="d1f7d-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-720">Boolean</span></span>|<span data-ttu-id="d1f7d-721">指示是否允许在 iOS 11.4.1 (设备锁定时连接到 USB) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-721">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="d1f7d-722">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="d1f7d-722">passwordBlockAutoFill</span></span>|<span data-ttu-id="d1f7d-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-723">Boolean</span></span>|<span data-ttu-id="d1f7d-724">指示是否允许在 iOS 12.0 (自动填充密码) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-724">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-725">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="d1f7d-725">passwordBlockProximityRequests</span></span>|<span data-ttu-id="d1f7d-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-726">Boolean</span></span>|<span data-ttu-id="d1f7d-727">指示是否阻止从 iOS 12.0 (及更高版本的附近设备请求) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-727">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-728">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="d1f7d-728">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="d1f7d-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-729">Boolean</span></span>|<span data-ttu-id="d1f7d-730">指示是否阻止使用 iOS 12.0 及更高版本的 AirDrop 密码功能共享) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-730">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-731">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="d1f7d-731">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="d1f7d-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-732">Boolean</span></span>|<span data-ttu-id="d1f7d-733">指示日期和时间"自动设置"功能是否已启用，并且用户 (iOS 12.0 及更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-733">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-734">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="d1f7d-734">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="d1f7d-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-735">Boolean</span></span>|<span data-ttu-id="d1f7d-736">指示托管应用是否可以将联系人写入 iOS 12.0 及更高版本 (非托管联系人) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-736">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d1f7d-737">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="d1f7d-737">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="d1f7d-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-738">Boolean</span></span>|<span data-ttu-id="d1f7d-739">指示非托管应用是否可以从 iOS 12.0 (或更高版本的托管联系人帐户) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-739">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="d1f7d-740">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="d1f7d-740">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="d1f7d-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-741">Boolean</span></span>|<span data-ttu-id="d1f7d-742">指示是否阻止用户修改 iOS 12.2 (或更高版本的个人热点) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-742">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="d1f7d-743">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-743">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="d1f7d-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-744">Boolean</span></span>|<span data-ttu-id="d1f7d-745">指示在 iOS 13 或更高版本的设备受监督时 (连续路径) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-745">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d1f7d-746">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-746">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="d1f7d-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-747">Boolean</span></span>|<span data-ttu-id="d1f7d-748">指示在 iOS 13 或更高版本中监督设备时 (查找我的) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-748">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d1f7d-749">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-749">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="d1f7d-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-750">Boolean</span></span>|<span data-ttu-id="d1f7d-751">指示在 iOS 13 或更高版本中监督设备时是否 (查找我的好友) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-751">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d1f7d-752">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-752">iTunesBlocked</span></span>|<span data-ttu-id="d1f7d-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-753">Boolean</span></span>|<span data-ttu-id="d1f7d-754">指示是否阻止 iTunes 应用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-754">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="d1f7d-755">需要适用于 iOS 13 及更高版本的受监督设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-755">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d1f7d-756">sharedDeviceBlockTemporarySessions</span><span class="sxs-lookup"><span data-stu-id="d1f7d-756">sharedDeviceBlockTemporarySessions</span></span>|<span data-ttu-id="d1f7d-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-757">Boolean</span></span>|<span data-ttu-id="d1f7d-758">指示是否阻止 iOS 13.4 或更高版本上的共享 iPad (临时) 。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-758">Indicates whether or not to block temporary sessions on Shared iPads (iOS 13.4 or later).</span></span>|
|<span data-ttu-id="d1f7d-759">appClipsBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-759">appClipsBlocked</span></span>|<span data-ttu-id="d1f7d-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-760">Boolean</span></span>|<span data-ttu-id="d1f7d-761">阻止用户添加任何应用剪辑并删除设备上的任何现有应用剪辑。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-761">Prevents a user from adding any App Clips and removes any existing App Clips on the device.</span></span>|
|<span data-ttu-id="d1f7d-762">applePersonalizedAdsBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-762">applePersonalizedAdsBlocked</span></span>|<span data-ttu-id="d1f7d-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-763">Boolean</span></span>|<span data-ttu-id="d1f7d-764">如果为 true，限制 Apple 个性化广告。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-764">Limits Apple personalized advertising when true.</span></span> <span data-ttu-id="d1f7d-765">在 iOS 14 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-765">Available in iOS 14 and later.</span></span>|
|<span data-ttu-id="d1f7d-766">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="d1f7d-766">nfcBlocked</span></span>|<span data-ttu-id="d1f7d-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f7d-767">Boolean</span></span>|<span data-ttu-id="d1f7d-768">禁用 NFC 以防止设备与其他支持 NFC 的设备配对。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-768">Disable NFC to prevent devices from pairing with other NFC-enabled devices.</span></span> <span data-ttu-id="d1f7d-769">适用于运行 14.2 及更高版本的 iOS/iPadOS 设备。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-769">Available for iOS/iPadOS devices running 14.2 and later.</span></span>|
|<span data-ttu-id="d1f7d-770">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-770">kioskModeAppType</span></span>|[<span data-ttu-id="d1f7d-771">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="d1f7d-771">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="d1f7d-772">在展台模式下运行的应用类型。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-772">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="d1f7d-773">可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-773">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="d1f7d-774">响应</span><span class="sxs-lookup"><span data-stu-id="d1f7d-774">Response</span></span>
<span data-ttu-id="d1f7d-775">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-775">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1f7d-776">示例</span><span class="sxs-lookup"><span data-stu-id="d1f7d-776">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1f7d-777">请求</span><span class="sxs-lookup"><span data-stu-id="d1f7d-777">Request</span></span>
<span data-ttu-id="d1f7d-778">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-778">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10656

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
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="d1f7d-779">响应</span><span class="sxs-lookup"><span data-stu-id="d1f7d-779">Response</span></span>
<span data-ttu-id="d1f7d-p159">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1f7d-p159">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10828

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
  "kioskModeAppType": "appStoreApp"
}
```




