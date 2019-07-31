---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ffd7c496bd385a783cb96b63ddcfa4beeb97258
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948234"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="5fb3b-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5fb3b-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="5fb3b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fb3b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fb3b-106">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fb3b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5fb3b-107">Prerequisites</span></span>
<span data-ttu-id="5fb3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fb3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fb3b-110">Permission type</span></span>|<span data-ttu-id="5fb3b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5fb3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fb3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fb3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fb3b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fb3b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fb3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fb3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fb3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-115">Not supported.</span></span>|
|<span data-ttu-id="5fb3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fb3b-116">Application</span></span>|<span data-ttu-id="5fb3b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fb3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fb3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5fb3b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fb3b-119">Request headers</span></span>
|<span data-ttu-id="5fb3b-120">标头</span><span class="sxs-lookup"><span data-stu-id="5fb3b-120">Header</span></span>|<span data-ttu-id="5fb3b-121">值</span><span class="sxs-lookup"><span data-stu-id="5fb3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fb3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fb3b-122">Authorization</span></span>|<span data-ttu-id="5fb3b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fb3b-124">接受</span><span class="sxs-lookup"><span data-stu-id="5fb3b-124">Accept</span></span>|<span data-ttu-id="5fb3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5fb3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fb3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fb3b-126">Request body</span></span>
<span data-ttu-id="5fb3b-127">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="5fb3b-128">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="5fb3b-129">属性</span><span class="sxs-lookup"><span data-stu-id="5fb3b-129">Property</span></span>|<span data-ttu-id="5fb3b-130">类型</span><span class="sxs-lookup"><span data-stu-id="5fb3b-130">Type</span></span>|<span data-ttu-id="5fb3b-131">说明</span><span class="sxs-lookup"><span data-stu-id="5fb3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb3b-132">id</span><span class="sxs-lookup"><span data-stu-id="5fb3b-132">id</span></span>|<span data-ttu-id="5fb3b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5fb3b-133">String</span></span>|<span data-ttu-id="5fb3b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-134">Key of the entity.</span></span> <span data-ttu-id="5fb3b-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fb3b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5fb3b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fb3b-137">DateTimeOffset</span></span>|<span data-ttu-id="5fb3b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5fb3b-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5fb3b-140">roleScopeTagIds</span></span>|<span data-ttu-id="5fb3b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5fb3b-141">String collection</span></span>|<span data-ttu-id="5fb3b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5fb3b-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5fb3b-144">supportsScopeTags</span></span>|<span data-ttu-id="5fb3b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-145">Boolean</span></span>|<span data-ttu-id="5fb3b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5fb3b-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5fb3b-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5fb3b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-149">This property is read-only.</span></span> <span data-ttu-id="5fb3b-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5fb3b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5fb3b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5fb3b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5fb3b-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5fb3b-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5fb3b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5fb3b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5fb3b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5fb3b-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5fb3b-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5fb3b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5fb3b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5fb3b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5fb3b-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5fb3b-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fb3b-163">createdDateTime</span></span>|<span data-ttu-id="5fb3b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fb3b-164">DateTimeOffset</span></span>|<span data-ttu-id="5fb3b-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-165">DateTime the object was created.</span></span> <span data-ttu-id="5fb3b-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-167">说明</span><span class="sxs-lookup"><span data-stu-id="5fb3b-167">description</span></span>|<span data-ttu-id="5fb3b-168">String</span><span class="sxs-lookup"><span data-stu-id="5fb3b-168">String</span></span>|<span data-ttu-id="5fb3b-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5fb3b-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5fb3b-171">displayName</span></span>|<span data-ttu-id="5fb3b-172">String</span><span class="sxs-lookup"><span data-stu-id="5fb3b-172">String</span></span>|<span data-ttu-id="5fb3b-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5fb3b-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-175">version</span><span class="sxs-lookup"><span data-stu-id="5fb3b-175">version</span></span>|<span data-ttu-id="5fb3b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-176">Int32</span></span>|<span data-ttu-id="5fb3b-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-177">Version of the device configuration.</span></span> <span data-ttu-id="5fb3b-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fb3b-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fb3b-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-179">accountBlockModification</span></span>|<span data-ttu-id="5fb3b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-180">Boolean</span></span>|<span data-ttu-id="5fb3b-181">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="5fb3b-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="5fb3b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-183">Boolean</span></span>|<span data-ttu-id="5fb3b-184">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-185">airDropBlocked</span></span>|<span data-ttu-id="5fb3b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-186">Boolean</span></span>|<span data-ttu-id="5fb3b-187">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="5fb3b-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="5fb3b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-189">Boolean</span></span>|<span data-ttu-id="5fb3b-190">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="5fb3b-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="5fb3b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-192">Boolean</span></span>|<span data-ttu-id="5fb3b-193">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="5fb3b-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="5fb3b-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="5fb3b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-195">Boolean</span></span>|<span data-ttu-id="5fb3b-196">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="5fb3b-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="5fb3b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-198">Boolean</span></span>|<span data-ttu-id="5fb3b-199">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="5fb3b-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-200">appleNewsBlocked</span></span>|<span data-ttu-id="5fb3b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-201">Boolean</span></span>|<span data-ttu-id="5fb3b-202">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="5fb3b-203">appsSingleAppModeList</span></span>|<span data-ttu-id="5fb3b-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fb3b-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5fb3b-205">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="5fb3b-206">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-206">Supervised only.</span></span> <span data-ttu-id="5fb3b-207">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-207">iOS 7.0 and later.</span></span> <span data-ttu-id="5fb3b-208">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5fb3b-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="5fb3b-209">appsVisibilityList</span></span>|<span data-ttu-id="5fb3b-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fb3b-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5fb3b-211">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="5fb3b-212">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="5fb3b-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-213">appsVisibilityListType</span></span>|[<span data-ttu-id="5fb3b-214">appListType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="5fb3b-215">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="5fb3b-216">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="5fb3b-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="5fb3b-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="5fb3b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-218">Boolean</span></span>|<span data-ttu-id="5fb3b-219">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-220">appStoreBlocked</span></span>|<span data-ttu-id="5fb3b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-221">Boolean</span></span>|<span data-ttu-id="5fb3b-222">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-222">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="5fb3b-223">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="5fb3b-223">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="5fb3b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-224">Boolean</span></span>|<span data-ttu-id="5fb3b-225">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-225">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="5fb3b-226">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-226">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="5fb3b-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-227">Boolean</span></span>|<span data-ttu-id="5fb3b-228">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-228">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="5fb3b-229">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-229">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-230">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="5fb3b-230">appStoreRequirePassword</span></span>|<span data-ttu-id="5fb3b-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-231">Boolean</span></span>|<span data-ttu-id="5fb3b-232">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-232">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="5fb3b-233">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="5fb3b-233">autoFillForceAuthentication</span></span>|<span data-ttu-id="5fb3b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-234">Boolean</span></span>|<span data-ttu-id="5fb3b-235">指示在 Safari 中的 autofilling 密码和信用卡信息之前是否强制进行用户身份验证, 以及受监督的设备上的其他应用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-235">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="5fb3b-236">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-236">bluetoothBlockModification</span></span>|<span data-ttu-id="5fb3b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-237">Boolean</span></span>|<span data-ttu-id="5fb3b-238">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-238">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-239">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-239">cameraBlocked</span></span>|<span data-ttu-id="5fb3b-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-240">Boolean</span></span>|<span data-ttu-id="5fb3b-241">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-241">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="5fb3b-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="5fb3b-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="5fb3b-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-243">Boolean</span></span>|<span data-ttu-id="5fb3b-244">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="5fb3b-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="5fb3b-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="5fb3b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-246">Boolean</span></span>|<span data-ttu-id="5fb3b-247">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-247">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="5fb3b-248">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-248">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="5fb3b-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-249">Boolean</span></span>|<span data-ttu-id="5fb3b-250">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-250">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-251">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="5fb3b-251">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="5fb3b-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-252">Boolean</span></span>|<span data-ttu-id="5fb3b-253">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-253">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="5fb3b-254">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-254">cellularBlockPlanModification</span></span>|<span data-ttu-id="5fb3b-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-255">Boolean</span></span>|<span data-ttu-id="5fb3b-256">指示是否允许用户在受监督的设备上更改移动电话计划的设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-256">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="5fb3b-257">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="5fb3b-257">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="5fb3b-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-258">Boolean</span></span>|<span data-ttu-id="5fb3b-259">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-259">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="5fb3b-260">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="5fb3b-260">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="5fb3b-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-261">Boolean</span></span>|<span data-ttu-id="5fb3b-262">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-262">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="5fb3b-263">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-263">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="5fb3b-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-264">Boolean</span></span>|<span data-ttu-id="5fb3b-265">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-265">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-266">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-266">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="5fb3b-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-267">Boolean</span></span>|<span data-ttu-id="5fb3b-268">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-268">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-269">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="5fb3b-269">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="5fb3b-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-270">Boolean</span></span>|<span data-ttu-id="5fb3b-271">指示设备处于监督模式时是否自动向教师的请求授予权限, 而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-271">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-272">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="5fb3b-272">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="5fb3b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-273">Boolean</span></span>|<span data-ttu-id="5fb3b-274">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-274">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="5fb3b-275">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-275">Supervised only.</span></span>|
|<span data-ttu-id="5fb3b-276">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="5fb3b-276">compliantAppsList</span></span>|<span data-ttu-id="5fb3b-277">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fb3b-277">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5fb3b-278">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-278">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="5fb3b-279">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-279">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="5fb3b-280">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-280">compliantAppListType</span></span>|[<span data-ttu-id="5fb3b-281">appListType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-281">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="5fb3b-282">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-282">List that is in the AppComplianceList.</span></span> <span data-ttu-id="5fb3b-283">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-283">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="5fb3b-284">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="5fb3b-284">configurationProfileBlockChanges</span></span>|<span data-ttu-id="5fb3b-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-285">Boolean</span></span>|<span data-ttu-id="5fb3b-286">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-286">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-287">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-287">definitionLookupBlocked</span></span>|<span data-ttu-id="5fb3b-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-288">Boolean</span></span>|<span data-ttu-id="5fb3b-289">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-289">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="5fb3b-290">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="5fb3b-290">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="5fb3b-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-291">Boolean</span></span>|<span data-ttu-id="5fb3b-292">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-292">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-293">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-293">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="5fb3b-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-294">Boolean</span></span>|<span data-ttu-id="5fb3b-295">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-295">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-296">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-296">deviceBlockNameModification</span></span>|<span data-ttu-id="5fb3b-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-297">Boolean</span></span>|<span data-ttu-id="5fb3b-298">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-298">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-299">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="5fb3b-299">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="5fb3b-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-300">Boolean</span></span>|<span data-ttu-id="5fb3b-301">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-301">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="5fb3b-302">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-302">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="5fb3b-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-303">Boolean</span></span>|<span data-ttu-id="5fb3b-304">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-304">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="5fb3b-305">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="5fb3b-305">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="5fb3b-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-306">Boolean</span></span>|<span data-ttu-id="5fb3b-307">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-307">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="5fb3b-308">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="5fb3b-308">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="5fb3b-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-309">Boolean</span></span>|<span data-ttu-id="5fb3b-310">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-310">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="5fb3b-311">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="5fb3b-311">emailInDomainSuffixes</span></span>|<span data-ttu-id="5fb3b-312">String 集合</span><span class="sxs-lookup"><span data-stu-id="5fb3b-312">String collection</span></span>|<span data-ttu-id="5fb3b-313">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-313">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="5fb3b-314">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="5fb3b-314">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="5fb3b-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-315">Boolean</span></span>|<span data-ttu-id="5fb3b-316">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-316">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="5fb3b-317">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-317">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="5fb3b-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-318">Boolean</span></span>|<span data-ttu-id="5fb3b-319">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-319">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="5fb3b-320">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-320">esimBlockModification</span></span>|<span data-ttu-id="5fb3b-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-321">Boolean</span></span>|<span data-ttu-id="5fb3b-322">指示是否允许在受监督的设备的 eSIM 卡上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-322">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="5fb3b-323">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-323">faceTimeBlocked</span></span>|<span data-ttu-id="5fb3b-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-324">Boolean</span></span>|<span data-ttu-id="5fb3b-325">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-325">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="5fb3b-326">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-326">findMyFriendsBlocked</span></span>|<span data-ttu-id="5fb3b-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-327">Boolean</span></span>|<span data-ttu-id="5fb3b-328">指示设备处于监督模式时是否阻止查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-328">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-329">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="5fb3b-329">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="5fb3b-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-330">Boolean</span></span>|<span data-ttu-id="5fb3b-331">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-331">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="5fb3b-332">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="5fb3b-332">gamingBlockMultiplayer</span></span>|<span data-ttu-id="5fb3b-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-333">Boolean</span></span>|<span data-ttu-id="5fb3b-334">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-334">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="5fb3b-335">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-335">gameCenterBlocked</span></span>|<span data-ttu-id="5fb3b-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-336">Boolean</span></span>|<span data-ttu-id="5fb3b-337">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-337">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-338">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-338">hostPairingBlocked</span></span>|<span data-ttu-id="5fb3b-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-339">Boolean</span></span>|<span data-ttu-id="5fb3b-340">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-340">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-341">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-341">iBooksStoreBlocked</span></span>|<span data-ttu-id="5fb3b-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-342">Boolean</span></span>|<span data-ttu-id="5fb3b-343">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-343">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-344">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="5fb3b-344">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="5fb3b-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-345">Boolean</span></span>|<span data-ttu-id="5fb3b-346">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-346">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="5fb3b-347">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-347">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="5fb3b-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-348">Boolean</span></span>|<span data-ttu-id="5fb3b-349">指示是否阻止用户将其在 iOS 设备上启动的工作继续到另一个 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-349">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="5fb3b-350">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="5fb3b-350">iCloudBlockBackup</span></span>|<span data-ttu-id="5fb3b-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-351">Boolean</span></span>|<span data-ttu-id="5fb3b-352">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-352">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="5fb3b-353">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="5fb3b-353">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="5fb3b-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-354">Boolean</span></span>|<span data-ttu-id="5fb3b-355">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-355">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="5fb3b-356">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="5fb3b-356">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="5fb3b-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-357">Boolean</span></span>|<span data-ttu-id="5fb3b-358">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-358">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="5fb3b-359">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="5fb3b-359">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="5fb3b-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-360">Boolean</span></span>|<span data-ttu-id="5fb3b-361">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-361">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="5fb3b-362">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="5fb3b-362">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="5fb3b-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-363">Boolean</span></span>|<span data-ttu-id="5fb3b-364">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-364">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="5fb3b-365">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="5fb3b-365">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="5fb3b-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-366">Boolean</span></span>|<span data-ttu-id="5fb3b-367">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-367">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="5fb3b-368">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="5fb3b-368">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="5fb3b-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-369">Boolean</span></span>|<span data-ttu-id="5fb3b-370">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-370">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="5fb3b-371">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="5fb3b-371">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="5fb3b-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-372">Boolean</span></span>|<span data-ttu-id="5fb3b-373">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-373">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="5fb3b-374">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="5fb3b-374">iTunesBlockMusicService</span></span>|<span data-ttu-id="5fb3b-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-375">Boolean</span></span>|<span data-ttu-id="5fb3b-376">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-376">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="5fb3b-377">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="5fb3b-377">iTunesBlockRadio</span></span>|<span data-ttu-id="5fb3b-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-378">Boolean</span></span>|<span data-ttu-id="5fb3b-379">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-379">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-380">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="5fb3b-380">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="5fb3b-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-381">Boolean</span></span>|<span data-ttu-id="5fb3b-382">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-382">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-383">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-383">keyboardBlockDictation</span></span>|<span data-ttu-id="5fb3b-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-384">Boolean</span></span>|<span data-ttu-id="5fb3b-385">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-385">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-386">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="5fb3b-386">keyboardBlockPredictive</span></span>|<span data-ttu-id="5fb3b-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-387">Boolean</span></span>|<span data-ttu-id="5fb3b-388">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-388">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-389">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="5fb3b-389">keyboardBlockShortcuts</span></span>|<span data-ttu-id="5fb3b-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-390">Boolean</span></span>|<span data-ttu-id="5fb3b-391">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-391">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-392">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="5fb3b-392">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="5fb3b-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-393">Boolean</span></span>|<span data-ttu-id="5fb3b-394">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-394">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-395">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="5fb3b-395">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="5fb3b-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-396">Boolean</span></span>|<span data-ttu-id="5fb3b-397">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-397">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-398">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-398">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="5fb3b-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-399">Boolean</span></span>|<span data-ttu-id="5fb3b-400">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-400">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-401">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="5fb3b-401">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="5fb3b-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-402">Boolean</span></span>|<span data-ttu-id="5fb3b-403">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-403">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="5fb3b-404">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-404">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="5fb3b-405">请改用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-405">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="5fb3b-406">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="5fb3b-406">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="5fb3b-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-407">Boolean</span></span>|<span data-ttu-id="5fb3b-408">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-408">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-409">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-409">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="5fb3b-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-410">Boolean</span></span>|<span data-ttu-id="5fb3b-411">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-411">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-412">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="5fb3b-412">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="5fb3b-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-413">Boolean</span></span>|<span data-ttu-id="5fb3b-414">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-414">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="5fb3b-415">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-415">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="5fb3b-416">请改用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-416">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="5fb3b-417">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="5fb3b-417">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="5fb3b-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-418">Boolean</span></span>|<span data-ttu-id="5fb3b-419">指示在展台模式下是否阻止使用铃声开关。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-419">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-420">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-420">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="5fb3b-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-421">Boolean</span></span>|<span data-ttu-id="5fb3b-422">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-422">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="5fb3b-423">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="5fb3b-424">请改用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-424">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="5fb3b-425">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-425">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="5fb3b-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-426">Boolean</span></span>|<span data-ttu-id="5fb3b-427">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-427">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-428">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="5fb3b-428">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="5fb3b-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-429">Boolean</span></span>|<span data-ttu-id="5fb3b-430">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-430">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="5fb3b-431">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="5fb3b-432">请改用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-432">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="5fb3b-433">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="5fb3b-433">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="5fb3b-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-434">Boolean</span></span>|<span data-ttu-id="5fb3b-435">指示在展台模式下是否阻止使用 "睡眠" 按钮。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-435">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-436">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="5fb3b-436">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="5fb3b-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-437">Boolean</span></span>|<span data-ttu-id="5fb3b-438">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-438">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="5fb3b-439">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="5fb3b-440">请改用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-440">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="5fb3b-441">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="5fb3b-441">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="5fb3b-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-442">Boolean</span></span>|<span data-ttu-id="5fb3b-443">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-443">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-444">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-444">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="5fb3b-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-445">Boolean</span></span>|<span data-ttu-id="5fb3b-446">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-446">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-447">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="5fb3b-447">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="5fb3b-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-448">Boolean</span></span>|<span data-ttu-id="5fb3b-449">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-449">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="5fb3b-450">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-450">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="5fb3b-451">请改用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-451">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="5fb3b-452">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="5fb3b-452">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="5fb3b-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-453">Boolean</span></span>|<span data-ttu-id="5fb3b-454">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-454">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="5fb3b-455">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-455">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="5fb3b-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-456">Boolean</span></span>|<span data-ttu-id="5fb3b-457">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-457">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-458">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5fb3b-458">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="5fb3b-459">String</span><span class="sxs-lookup"><span data-stu-id="5fb3b-459">String</span></span>|<span data-ttu-id="5fb3b-460">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-460">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="5fb3b-461">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-461">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="5fb3b-462">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="5fb3b-462">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="5fb3b-463">String</span><span class="sxs-lookup"><span data-stu-id="5fb3b-463">String</span></span>|<span data-ttu-id="5fb3b-464">用于展台模式的内置应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-464">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="5fb3b-465">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-465">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="5fb3b-466">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="5fb3b-466">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="5fb3b-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-467">Boolean</span></span>|<span data-ttu-id="5fb3b-468">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-468">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-469">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="5fb3b-469">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="5fb3b-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-470">Boolean</span></span>|<span data-ttu-id="5fb3b-471">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-471">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-472">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="5fb3b-472">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="5fb3b-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-473">Boolean</span></span>|<span data-ttu-id="5fb3b-474">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-474">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-475">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="5fb3b-475">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="5fb3b-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-476">Boolean</span></span>|<span data-ttu-id="5fb3b-477">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-477">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-478">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="5fb3b-478">kioskModeRequireZoom</span></span>|<span data-ttu-id="5fb3b-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-479">Boolean</span></span>|<span data-ttu-id="5fb3b-480">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-480">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="5fb3b-481">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="5fb3b-481">kioskModeManagedAppId</span></span>|<span data-ttu-id="5fb3b-482">String</span><span class="sxs-lookup"><span data-stu-id="5fb3b-482">String</span></span>|<span data-ttu-id="5fb3b-483">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-483">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="5fb3b-484">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-484">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="5fb3b-485">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="5fb3b-485">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="5fb3b-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-486">Boolean</span></span>|<span data-ttu-id="5fb3b-487">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-487">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="5fb3b-488">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="5fb3b-488">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="5fb3b-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-489">Boolean</span></span>|<span data-ttu-id="5fb3b-490">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-490">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="5fb3b-491">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="5fb3b-491">lockScreenBlockPassbook</span></span>|<span data-ttu-id="5fb3b-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-492">Boolean</span></span>|<span data-ttu-id="5fb3b-493">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-493">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="5fb3b-494">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="5fb3b-494">lockScreenBlockTodayView</span></span>|<span data-ttu-id="5fb3b-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-495">Boolean</span></span>|<span data-ttu-id="5fb3b-496">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-496">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="5fb3b-497">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="5fb3b-497">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="5fb3b-498">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="5fb3b-498">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="5fb3b-499">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-499">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="5fb3b-500">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="5fb3b-500">mediaContentRatingCanada</span></span>|[<span data-ttu-id="5fb3b-501">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="5fb3b-501">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="5fb3b-502">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-502">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="5fb3b-503">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="5fb3b-503">mediaContentRatingFrance</span></span>|[<span data-ttu-id="5fb3b-504">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="5fb3b-504">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="5fb3b-505">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-505">Media content rating settings for France</span></span>|
|<span data-ttu-id="5fb3b-506">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="5fb3b-506">mediaContentRatingGermany</span></span>|[<span data-ttu-id="5fb3b-507">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="5fb3b-507">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="5fb3b-508">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-508">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="5fb3b-509">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="5fb3b-509">mediaContentRatingIreland</span></span>|[<span data-ttu-id="5fb3b-510">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="5fb3b-510">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="5fb3b-511">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-511">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="5fb3b-512">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="5fb3b-512">mediaContentRatingJapan</span></span>|[<span data-ttu-id="5fb3b-513">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="5fb3b-513">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="5fb3b-514">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-514">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="5fb3b-515">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="5fb3b-515">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="5fb3b-516">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="5fb3b-516">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="5fb3b-517">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-517">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="5fb3b-518">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="5fb3b-518">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="5fb3b-519">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="5fb3b-519">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="5fb3b-520">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-520">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="5fb3b-521">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="5fb3b-521">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="5fb3b-522">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="5fb3b-522">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="5fb3b-523">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="5fb3b-523">Media content rating settings for United States</span></span>|
|<span data-ttu-id="5fb3b-524">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="5fb3b-524">networkUsageRules</span></span>|<span data-ttu-id="5fb3b-525">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fb3b-525">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="5fb3b-526">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-526">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="5fb3b-527">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-527">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="5fb3b-528">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="5fb3b-528">mediaContentRatingApps</span></span>|[<span data-ttu-id="5fb3b-529">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-529">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="5fb3b-530">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-530">Media content rating settings for Apps.</span></span> <span data-ttu-id="5fb3b-531">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-531">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="5fb3b-532">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-532">messagesBlocked</span></span>|<span data-ttu-id="5fb3b-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-533">Boolean</span></span>|<span data-ttu-id="5fb3b-534">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-534">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="5fb3b-535">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-535">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="5fb3b-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-536">Boolean</span></span>|<span data-ttu-id="5fb3b-537">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-537">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-538">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="5fb3b-538">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="5fb3b-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-539">Boolean</span></span>|<span data-ttu-id="5fb3b-540">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-540">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="5fb3b-541">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-541">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="5fb3b-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-542">Boolean</span></span>|<span data-ttu-id="5fb3b-543">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-543">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-544">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-544">passcodeBlockModification</span></span>|<span data-ttu-id="5fb3b-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-545">Boolean</span></span>|<span data-ttu-id="5fb3b-546">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-546">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-547">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5fb3b-547">passcodeBlockSimple</span></span>|<span data-ttu-id="5fb3b-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-548">Boolean</span></span>|<span data-ttu-id="5fb3b-549">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-549">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="5fb3b-550">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5fb3b-550">passcodeExpirationDays</span></span>|<span data-ttu-id="5fb3b-551">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-551">Int32</span></span>|<span data-ttu-id="5fb3b-552">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-552">Number of days before the passcode expires.</span></span> <span data-ttu-id="5fb3b-553">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="5fb3b-553">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="5fb3b-554">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5fb3b-554">passcodeMinimumLength</span></span>|<span data-ttu-id="5fb3b-555">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-555">Int32</span></span>|<span data-ttu-id="5fb3b-556">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-556">Minimum length of passcode.</span></span> <span data-ttu-id="5fb3b-557">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="5fb3b-557">Valid values 4 to 14</span></span>|
|<span data-ttu-id="5fb3b-558">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5fb3b-558">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5fb3b-559">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-559">Int32</span></span>|<span data-ttu-id="5fb3b-560">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-560">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="5fb3b-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5fb3b-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5fb3b-562">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-562">Int32</span></span>|<span data-ttu-id="5fb3b-563">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-563">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="5fb3b-564">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5fb3b-564">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="5fb3b-565">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-565">Int32</span></span>|<span data-ttu-id="5fb3b-566">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-566">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="5fb3b-567">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="5fb3b-567">Valid values 0 to 4</span></span>|
|<span data-ttu-id="5fb3b-568">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="5fb3b-568">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="5fb3b-569">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-569">Int32</span></span>|<span data-ttu-id="5fb3b-570">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-570">Number of previous passcodes to block.</span></span> <span data-ttu-id="5fb3b-571">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="5fb3b-571">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5fb3b-572">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="5fb3b-572">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="5fb3b-573">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-573">Int32</span></span>|<span data-ttu-id="5fb3b-574">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-574">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="5fb3b-575">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="5fb3b-575">Valid values 4 to 11</span></span>|
|<span data-ttu-id="5fb3b-576">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-576">passcodeRequiredType</span></span>|[<span data-ttu-id="5fb3b-577">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5fb3b-577">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5fb3b-578">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-578">Type of passcode that is required.</span></span> <span data-ttu-id="5fb3b-579">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-579">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5fb3b-580">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="5fb3b-580">passcodeRequired</span></span>|<span data-ttu-id="5fb3b-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-581">Boolean</span></span>|<span data-ttu-id="5fb3b-582">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-582">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="5fb3b-583">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-583">podcastsBlocked</span></span>|<span data-ttu-id="5fb3b-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-584">Boolean</span></span>|<span data-ttu-id="5fb3b-585">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-585">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-586">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="5fb3b-586">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="5fb3b-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-587">Boolean</span></span>|<span data-ttu-id="5fb3b-588">指示是否启用提示以在受监督的设备上安装附近设备。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-588">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="5fb3b-589">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="5fb3b-589">safariBlockAutofill</span></span>|<span data-ttu-id="5fb3b-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-590">Boolean</span></span>|<span data-ttu-id="5fb3b-591">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-591">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="5fb3b-592">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="5fb3b-592">safariBlockJavaScript</span></span>|<span data-ttu-id="5fb3b-593">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-593">Boolean</span></span>|<span data-ttu-id="5fb3b-594">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-594">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="5fb3b-595">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="5fb3b-595">safariBlockPopups</span></span>|<span data-ttu-id="5fb3b-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-596">Boolean</span></span>|<span data-ttu-id="5fb3b-597">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-597">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="5fb3b-598">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-598">safariBlocked</span></span>|<span data-ttu-id="5fb3b-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-599">Boolean</span></span>|<span data-ttu-id="5fb3b-600">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-600">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="5fb3b-601">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-601">safariCookieSettings</span></span>|[<span data-ttu-id="5fb3b-602">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="5fb3b-602">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="5fb3b-603">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-603">Cookie settings for Safari.</span></span> <span data-ttu-id="5fb3b-604">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-604">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="5fb3b-605">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="5fb3b-605">safariManagedDomains</span></span>|<span data-ttu-id="5fb3b-606">String collection</span><span class="sxs-lookup"><span data-stu-id="5fb3b-606">String collection</span></span>|<span data-ttu-id="5fb3b-607">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-607">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="5fb3b-608">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="5fb3b-608">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="5fb3b-609">String 集合</span><span class="sxs-lookup"><span data-stu-id="5fb3b-609">String collection</span></span>|<span data-ttu-id="5fb3b-610">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-610">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="5fb3b-611">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-611">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-612">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="5fb3b-612">safariRequireFraudWarning</span></span>|<span data-ttu-id="5fb3b-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-613">Boolean</span></span>|<span data-ttu-id="5fb3b-614">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-614">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="5fb3b-615">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-615">screenCaptureBlocked</span></span>|<span data-ttu-id="5fb3b-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-616">Boolean</span></span>|<span data-ttu-id="5fb3b-617">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-617">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="5fb3b-618">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-618">siriBlocked</span></span>|<span data-ttu-id="5fb3b-619">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-619">Boolean</span></span>|<span data-ttu-id="5fb3b-620">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-620">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="5fb3b-621">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-621">siriBlockedWhenLocked</span></span>|<span data-ttu-id="5fb3b-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-622">Boolean</span></span>|<span data-ttu-id="5fb3b-623">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-623">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="5fb3b-624">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="5fb3b-624">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="5fb3b-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-625">Boolean</span></span>|<span data-ttu-id="5fb3b-626">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-626">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="5fb3b-627">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="5fb3b-627">siriRequireProfanityFilter</span></span>|<span data-ttu-id="5fb3b-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-628">Boolean</span></span>|<span data-ttu-id="5fb3b-629">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-629">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="5fb3b-630">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="5fb3b-630">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="5fb3b-631">Int32</span><span class="sxs-lookup"><span data-stu-id="5fb3b-631">Int32</span></span>|<span data-ttu-id="5fb3b-632">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-632">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="5fb3b-633">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="5fb3b-633">Valid values 0 to 90</span></span>|
|<span data-ttu-id="5fb3b-634">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="5fb3b-634">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="5fb3b-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-635">Boolean</span></span>|<span data-ttu-id="5fb3b-636">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-636">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-637">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="5fb3b-637">spotlightBlockInternetResults</span></span>|<span data-ttu-id="5fb3b-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-638">Boolean</span></span>|<span data-ttu-id="5fb3b-639">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-639">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="5fb3b-640">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-640">voiceDialingBlocked</span></span>|<span data-ttu-id="5fb3b-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-641">Boolean</span></span>|<span data-ttu-id="5fb3b-642">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-642">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="5fb3b-643">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-643">wallpaperBlockModification</span></span>|<span data-ttu-id="5fb3b-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-644">Boolean</span></span>|<span data-ttu-id="5fb3b-645">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-645">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="5fb3b-646">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="5fb3b-646">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="5fb3b-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-647">Boolean</span></span>|<span data-ttu-id="5fb3b-648">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-648">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="5fb3b-649">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="5fb3b-649">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="5fb3b-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-650">Boolean</span></span>|<span data-ttu-id="5fb3b-651">指示在非托管课程中通过教室注册的学生是否会在尝试离开该课程 (iOS 11.3 及更高版本) 时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-651">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="5fb3b-652">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="5fb3b-652">keychainBlockCloudSync</span></span>|<span data-ttu-id="5fb3b-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-653">Boolean</span></span>|<span data-ttu-id="5fb3b-654">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-654">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="5fb3b-655">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="5fb3b-655">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="5fb3b-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-656">Boolean</span></span>|<span data-ttu-id="5fb3b-657">指示是否阻止无线 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-657">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="5fb3b-658">将此限制设置为 false 不会禁用 CRL 和 OCSP 检查 (iOS 7.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-658">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-659">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="5fb3b-659">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="5fb3b-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-660">Boolean</span></span>|<span data-ttu-id="5fb3b-661">指示广告跟踪是否受限制。(iOS 7.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-661">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-662">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="5fb3b-662">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="5fb3b-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-663">Boolean</span></span>|<span data-ttu-id="5fb3b-664">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-664">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="5fb3b-665">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="5fb3b-665">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="5fb3b-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-666">Boolean</span></span>|<span data-ttu-id="5fb3b-667">指示是否阻止企业书籍笔记和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-667">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="5fb3b-668">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-668">airPrintBlocked</span></span>|<span data-ttu-id="5fb3b-669">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-669">Boolean</span></span>|<span data-ttu-id="5fb3b-670">指示是否阻止 AirPrint (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-670">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-671">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="5fb3b-671">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="5fb3b-672">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-672">Boolean</span></span>|<span data-ttu-id="5fb3b-673">指示是否阻止 Airprint 的用户名和密码的密钥链存储 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-673">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-674">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="5fb3b-674">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="5fb3b-675">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-675">Boolean</span></span>|<span data-ttu-id="5fb3b-676">指示 TLS 打印通信是否需要受信任的证书 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-676">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-677">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="5fb3b-677">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="5fb3b-678">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-678">Boolean</span></span>|<span data-ttu-id="5fb3b-679">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-679">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="5fb3b-680">这样可以防止虚假的 AirPrint 蓝牙信号免受网络流量 (iOS 11.0 及更高版本) 的欺骗。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-680">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-681">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="5fb3b-681">blockSystemAppRemoval</span></span>|<span data-ttu-id="5fb3b-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-682">Boolean</span></span>|<span data-ttu-id="5fb3b-683">指示是否在受监督的设备 (iOS 11.0 及更高版本) 上阻止从设备中删除系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-683">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-684">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="5fb3b-684">vpnBlockCreation</span></span>|<span data-ttu-id="5fb3b-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-685">Boolean</span></span>|<span data-ttu-id="5fb3b-686">指示是否阻止创建 VPN 配置 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-686">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-687">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-687">appRemovalBlocked</span></span>|<span data-ttu-id="5fb3b-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-688">Boolean</span></span>|<span data-ttu-id="5fb3b-689">指示是否允许删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-689">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="5fb3b-690">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="5fb3b-690">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="5fb3b-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-691">Boolean</span></span>|<span data-ttu-id="5fb3b-692">指示是否允许在锁定设备时连接到 USB 附件 (iOS 11.4.1 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-692">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="5fb3b-693">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="5fb3b-693">passwordBlockAutoFill</span></span>|<span data-ttu-id="5fb3b-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-694">Boolean</span></span>|<span data-ttu-id="5fb3b-695">指示是否允许自动填充密码功能 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-695">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-696">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="5fb3b-696">passwordBlockProximityRequests</span></span>|<span data-ttu-id="5fb3b-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-697">Boolean</span></span>|<span data-ttu-id="5fb3b-698">指示是否阻止来自附近设备 (iOS 12.0 及更高版本) 发出请求的密码。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-698">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-699">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="5fb3b-699">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="5fb3b-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-700">Boolean</span></span>|<span data-ttu-id="5fb3b-701">指示是否阻止使用 AirDrop 密码的共享密码功能 iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-701">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-702">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="5fb3b-702">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="5fb3b-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-703">Boolean</span></span>|<span data-ttu-id="5fb3b-704">指示是否启用日期和时间 "设置自动设置" 功能, 以及用户是否无法关闭该功能 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-704">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-705">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="5fb3b-705">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="5fb3b-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-706">Boolean</span></span>|<span data-ttu-id="5fb3b-707">指示托管应用程序是否可以将联系人写入非托管联系人帐户 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-707">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="5fb3b-708">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="5fb3b-708">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="5fb3b-709">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-709">Boolean</span></span>|<span data-ttu-id="5fb3b-710">指示非托管应用是否可以从托管联系人帐户读取 (iOS 12.0 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-710">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="5fb3b-711">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="5fb3b-711">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="5fb3b-712">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-712">Boolean</span></span>|<span data-ttu-id="5fb3b-713">指示是否阻止用户修改个人热点设置 (iOS 12.2 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-713">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="5fb3b-714">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="5fb3b-714">siriDisableServerLogging</span></span>|<span data-ttu-id="5fb3b-715">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fb3b-715">Boolean</span></span>|<span data-ttu-id="5fb3b-716">指示是否禁用服务器端 Siri 日志记录 (iOS 12.2 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-716">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="5fb3b-717">响应</span><span class="sxs-lookup"><span data-stu-id="5fb3b-717">Response</span></span>
<span data-ttu-id="5fb3b-718">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-718">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fb3b-719">示例</span><span class="sxs-lookup"><span data-stu-id="5fb3b-719">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fb3b-720">请求</span><span class="sxs-lookup"><span data-stu-id="5fb3b-720">Request</span></span>
<span data-ttu-id="5fb3b-721">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-721">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10159

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
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true
}
```

### <a name="response"></a><span data-ttu-id="5fb3b-722">响应</span><span class="sxs-lookup"><span data-stu-id="5fb3b-722">Response</span></span>
<span data-ttu-id="5fb3b-p142">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fb3b-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10331

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
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true
}
```





