---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42896574ce799467bb3f4591b719bd41139e1582
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439054"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="120df-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="120df-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="120df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="120df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="120df-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="120df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="120df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="120df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="120df-107">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="120df-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="120df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="120df-108">Prerequisites</span></span>
<span data-ttu-id="120df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="120df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="120df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="120df-111">Permission type</span></span>|<span data-ttu-id="120df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="120df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="120df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="120df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="120df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="120df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="120df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="120df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="120df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="120df-116">Not supported.</span></span>|
|<span data-ttu-id="120df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="120df-117">Application</span></span>|<span data-ttu-id="120df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="120df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="120df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="120df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="120df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="120df-120">Request headers</span></span>
|<span data-ttu-id="120df-121">标头</span><span class="sxs-lookup"><span data-stu-id="120df-121">Header</span></span>|<span data-ttu-id="120df-122">值</span><span class="sxs-lookup"><span data-stu-id="120df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="120df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="120df-123">Authorization</span></span>|<span data-ttu-id="120df-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="120df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="120df-125">接受</span><span class="sxs-lookup"><span data-stu-id="120df-125">Accept</span></span>|<span data-ttu-id="120df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="120df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="120df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="120df-127">Request body</span></span>
<span data-ttu-id="120df-128">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="120df-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="120df-129">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="120df-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="120df-130">属性</span><span class="sxs-lookup"><span data-stu-id="120df-130">Property</span></span>|<span data-ttu-id="120df-131">类型</span><span class="sxs-lookup"><span data-stu-id="120df-131">Type</span></span>|<span data-ttu-id="120df-132">说明</span><span class="sxs-lookup"><span data-stu-id="120df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120df-133">id</span><span class="sxs-lookup"><span data-stu-id="120df-133">id</span></span>|<span data-ttu-id="120df-134">字符串</span><span class="sxs-lookup"><span data-stu-id="120df-134">String</span></span>|<span data-ttu-id="120df-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="120df-135">Key of the entity.</span></span> <span data-ttu-id="120df-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="120df-137">lastModifiedDateTime</span></span>|<span data-ttu-id="120df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="120df-138">DateTimeOffset</span></span>|<span data-ttu-id="120df-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="120df-139">DateTime the object was last modified.</span></span> <span data-ttu-id="120df-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="120df-141">roleScopeTagIds</span></span>|<span data-ttu-id="120df-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="120df-142">String collection</span></span>|<span data-ttu-id="120df-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="120df-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="120df-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="120df-145">supportsScopeTags</span></span>|<span data-ttu-id="120df-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-146">Boolean</span></span>|<span data-ttu-id="120df-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="120df-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="120df-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="120df-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="120df-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="120df-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="120df-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="120df-150">This property is read-only.</span></span> <span data-ttu-id="120df-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="120df-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="120df-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="120df-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="120df-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="120df-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="120df-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="120df-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="120df-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="120df-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="120df-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="120df-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="120df-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="120df-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="120df-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="120df-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="120df-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="120df-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="120df-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="120df-164">createdDateTime</span></span>|<span data-ttu-id="120df-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="120df-165">DateTimeOffset</span></span>|<span data-ttu-id="120df-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="120df-166">DateTime the object was created.</span></span> <span data-ttu-id="120df-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-168">description</span><span class="sxs-lookup"><span data-stu-id="120df-168">description</span></span>|<span data-ttu-id="120df-169">String</span><span class="sxs-lookup"><span data-stu-id="120df-169">String</span></span>|<span data-ttu-id="120df-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="120df-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="120df-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-172">displayName</span><span class="sxs-lookup"><span data-stu-id="120df-172">displayName</span></span>|<span data-ttu-id="120df-173">String</span><span class="sxs-lookup"><span data-stu-id="120df-173">String</span></span>|<span data-ttu-id="120df-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="120df-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="120df-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-176">version</span><span class="sxs-lookup"><span data-stu-id="120df-176">version</span></span>|<span data-ttu-id="120df-177">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-177">Int32</span></span>|<span data-ttu-id="120df-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="120df-178">Version of the device configuration.</span></span> <span data-ttu-id="120df-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="120df-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="120df-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="120df-180">accountBlockModification</span></span>|<span data-ttu-id="120df-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-181">Boolean</span></span>|<span data-ttu-id="120df-182">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="120df-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="120df-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="120df-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-184">Boolean</span></span>|<span data-ttu-id="120df-185">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="120df-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="120df-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-186">airDropBlocked</span></span>|<span data-ttu-id="120df-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-187">Boolean</span></span>|<span data-ttu-id="120df-188">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="120df-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="120df-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="120df-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-190">Boolean</span></span>|<span data-ttu-id="120df-191">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="120df-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="120df-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-193">Boolean</span></span>|<span data-ttu-id="120df-194">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="120df-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="120df-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="120df-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="120df-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-196">Boolean</span></span>|<span data-ttu-id="120df-197">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="120df-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="120df-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-199">Boolean</span></span>|<span data-ttu-id="120df-200">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="120df-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-201">appleNewsBlocked</span></span>|<span data-ttu-id="120df-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-202">Boolean</span></span>|<span data-ttu-id="120df-203">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="120df-204">appsSingleAppModeList</span></span>|<span data-ttu-id="120df-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="120df-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="120df-206">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="120df-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="120df-207">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="120df-207">Supervised only.</span></span> <span data-ttu-id="120df-208">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-208">iOS 7.0 and later.</span></span> <span data-ttu-id="120df-209">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="120df-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="120df-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="120df-210">appsVisibilityList</span></span>|<span data-ttu-id="120df-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="120df-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="120df-212">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="120df-213">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="120df-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="120df-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="120df-214">appsVisibilityListType</span></span>|[<span data-ttu-id="120df-215">appListType</span><span class="sxs-lookup"><span data-stu-id="120df-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="120df-216">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="120df-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="120df-217">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="120df-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="120df-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="120df-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="120df-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-219">Boolean</span></span>|<span data-ttu-id="120df-220">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-221">appStoreBlocked</span></span>|<span data-ttu-id="120df-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-222">Boolean</span></span>|<span data-ttu-id="120df-223">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="120df-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="120df-224">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="120df-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="120df-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-226">Boolean</span></span>|<span data-ttu-id="120df-227">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="120df-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="120df-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="120df-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="120df-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-229">Boolean</span></span>|<span data-ttu-id="120df-230">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="120df-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="120df-231">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="120df-232">appStoreRequirePassword</span></span>|<span data-ttu-id="120df-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-233">Boolean</span></span>|<span data-ttu-id="120df-234">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="120df-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="120df-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="120df-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="120df-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-236">Boolean</span></span>|<span data-ttu-id="120df-237">指示在 Safari 中的 autofilling 密码和信用卡信息之前是否强制进行用户身份验证，以及受监督的设备上的其他应用。</span><span class="sxs-lookup"><span data-stu-id="120df-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="120df-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="120df-238">bluetoothBlockModification</span></span>|<span data-ttu-id="120df-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-239">Boolean</span></span>|<span data-ttu-id="120df-240">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="120df-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-241">cameraBlocked</span></span>|<span data-ttu-id="120df-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-242">Boolean</span></span>|<span data-ttu-id="120df-243">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="120df-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="120df-244">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="120df-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="120df-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-246">Boolean</span></span>|<span data-ttu-id="120df-247">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="120df-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="120df-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="120df-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="120df-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-249">Boolean</span></span>|<span data-ttu-id="120df-250">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="120df-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="120df-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="120df-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="120df-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-252">Boolean</span></span>|<span data-ttu-id="120df-253">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="120df-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="120df-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="120df-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-255">Boolean</span></span>|<span data-ttu-id="120df-256">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="120df-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="120df-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="120df-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="120df-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-258">Boolean</span></span>|<span data-ttu-id="120df-259">指示是否允许用户在受监督的设备上更改移动电话计划的设置。</span><span class="sxs-lookup"><span data-stu-id="120df-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="120df-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="120df-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="120df-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-261">Boolean</span></span>|<span data-ttu-id="120df-262">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="120df-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="120df-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="120df-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="120df-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-264">Boolean</span></span>|<span data-ttu-id="120df-265">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="120df-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="120df-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="120df-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="120df-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-267">Boolean</span></span>|<span data-ttu-id="120df-268">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="120df-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="120df-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="120df-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-270">Boolean</span></span>|<span data-ttu-id="120df-271">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="120df-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="120df-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="120df-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-273">Boolean</span></span>|<span data-ttu-id="120df-274">指示设备处于监督模式时是否自动向教师的请求授予权限，而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="120df-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="120df-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="120df-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-276">Boolean</span></span>|<span data-ttu-id="120df-277">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="120df-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="120df-278">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="120df-278">Supervised only.</span></span>|
|<span data-ttu-id="120df-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="120df-279">compliantAppsList</span></span>|<span data-ttu-id="120df-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="120df-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="120df-281">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="120df-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="120df-282">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="120df-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="120df-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="120df-283">compliantAppListType</span></span>|[<span data-ttu-id="120df-284">appListType</span><span class="sxs-lookup"><span data-stu-id="120df-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="120df-285">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="120df-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="120df-286">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="120df-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="120df-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="120df-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="120df-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-288">Boolean</span></span>|<span data-ttu-id="120df-289">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="120df-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-290">definitionLookupBlocked</span></span>|<span data-ttu-id="120df-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-291">Boolean</span></span>|<span data-ttu-id="120df-292">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="120df-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="120df-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="120df-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-294">Boolean</span></span>|<span data-ttu-id="120df-295">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="120df-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="120df-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="120df-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-297">Boolean</span></span>|<span data-ttu-id="120df-298">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="120df-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="120df-299">deviceBlockNameModification</span></span>|<span data-ttu-id="120df-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-300">Boolean</span></span>|<span data-ttu-id="120df-301">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="120df-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="120df-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-303">Boolean</span></span>|<span data-ttu-id="120df-304">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="120df-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="120df-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="120df-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="120df-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-306">Boolean</span></span>|<span data-ttu-id="120df-307">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="120df-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="120df-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="120df-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-309">Boolean</span></span>|<span data-ttu-id="120df-310">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="120df-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="120df-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="120df-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="120df-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-312">Boolean</span></span>|<span data-ttu-id="120df-313">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="120df-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="120df-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="120df-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="120df-315">String 集合</span><span class="sxs-lookup"><span data-stu-id="120df-315">String collection</span></span>|<span data-ttu-id="120df-316">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="120df-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="120df-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="120df-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="120df-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-318">Boolean</span></span>|<span data-ttu-id="120df-319">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="120df-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="120df-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="120df-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="120df-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-321">Boolean</span></span>|<span data-ttu-id="120df-322">\[已\]弃用配置此设置并将值设置为 "true" 对设备没有影响。</span><span class="sxs-lookup"><span data-stu-id="120df-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="120df-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="120df-323">esimBlockModification</span></span>|<span data-ttu-id="120df-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-324">Boolean</span></span>|<span data-ttu-id="120df-325">指示是否允许在受监督的设备的 eSIM 卡上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="120df-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="120df-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-326">faceTimeBlocked</span></span>|<span data-ttu-id="120df-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-327">Boolean</span></span>|<span data-ttu-id="120df-328">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="120df-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="120df-329">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="120df-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-331">Boolean</span></span>|<span data-ttu-id="120df-332">指示设备处于监督模式时是否阻止更改以查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="120df-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="120df-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="120df-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-334">Boolean</span></span>|<span data-ttu-id="120df-335">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="120df-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="120df-336">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="120df-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="120df-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-338">Boolean</span></span>|<span data-ttu-id="120df-339">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="120df-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="120df-340">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-341">gameCenterBlocked</span></span>|<span data-ttu-id="120df-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-342">Boolean</span></span>|<span data-ttu-id="120df-343">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="120df-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-344">hostPairingBlocked</span></span>|<span data-ttu-id="120df-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-345">Boolean</span></span>|<span data-ttu-id="120df-346">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="120df-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="120df-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-348">Boolean</span></span>|<span data-ttu-id="120df-349">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="120df-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="120df-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="120df-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-351">Boolean</span></span>|<span data-ttu-id="120df-352">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="120df-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="120df-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="120df-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="120df-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-354">Boolean</span></span>|<span data-ttu-id="120df-355">指示是否阻止用户将其在 iOS 设备上启动的工作继续到另一个 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="120df-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="120df-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="120df-356">iCloudBlockBackup</span></span>|<span data-ttu-id="120df-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-357">Boolean</span></span>|<span data-ttu-id="120df-358">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="120df-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="120df-359">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="120df-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="120df-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-361">Boolean</span></span>|<span data-ttu-id="120df-362">指示是否阻止 iCloud 文档同步。需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="120df-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="120df-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-364">Boolean</span></span>|<span data-ttu-id="120df-365">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="120df-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="120df-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="120df-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="120df-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-367">Boolean</span></span>|<span data-ttu-id="120df-368">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="120df-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="120df-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="120df-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="120df-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-370">Boolean</span></span>|<span data-ttu-id="120df-371">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="120df-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="120df-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="120df-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="120df-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-373">Boolean</span></span>|<span data-ttu-id="120df-374">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="120df-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="120df-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="120df-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="120df-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-376">Boolean</span></span>|<span data-ttu-id="120df-377">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="120df-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="120df-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="120df-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="120df-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-379">Boolean</span></span>|<span data-ttu-id="120df-380">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="120df-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="120df-381">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="120df-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="120df-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-383">Boolean</span></span>|<span data-ttu-id="120df-384">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="120df-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="120df-385">iTunesBlockRadio</span></span>|<span data-ttu-id="120df-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-386">Boolean</span></span>|<span data-ttu-id="120df-387">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="120df-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="120df-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="120df-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-389">Boolean</span></span>|<span data-ttu-id="120df-390">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="120df-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="120df-391">keyboardBlockDictation</span></span>|<span data-ttu-id="120df-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-392">Boolean</span></span>|<span data-ttu-id="120df-393">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="120df-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="120df-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="120df-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-395">Boolean</span></span>|<span data-ttu-id="120df-396">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="120df-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="120df-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="120df-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-398">Boolean</span></span>|<span data-ttu-id="120df-399">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="120df-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="120df-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-401">Boolean</span></span>|<span data-ttu-id="120df-402">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="120df-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="120df-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="120df-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-404">Boolean</span></span>|<span data-ttu-id="120df-405">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="120df-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="120df-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="120df-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-407">Boolean</span></span>|<span data-ttu-id="120df-408">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="120df-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="120df-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="120df-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-410">Boolean</span></span>|<span data-ttu-id="120df-411">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="120df-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="120df-412">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="120df-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="120df-413">请改用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="120df-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="120df-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="120df-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="120df-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-415">Boolean</span></span>|<span data-ttu-id="120df-416">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="120df-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="120df-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="120df-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-418">Boolean</span></span>|<span data-ttu-id="120df-419">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="120df-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="120df-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="120df-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-421">Boolean</span></span>|<span data-ttu-id="120df-422">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="120df-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="120df-423">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="120df-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="120df-424">请改用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="120df-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="120df-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="120df-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="120df-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-426">Boolean</span></span>|<span data-ttu-id="120df-427">指示在展台模式下是否阻止使用铃声开关。</span><span class="sxs-lookup"><span data-stu-id="120df-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="120df-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="120df-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-429">Boolean</span></span>|<span data-ttu-id="120df-430">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="120df-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="120df-431">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="120df-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="120df-432">请改用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="120df-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="120df-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="120df-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="120df-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-434">Boolean</span></span>|<span data-ttu-id="120df-435">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="120df-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="120df-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="120df-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-437">Boolean</span></span>|<span data-ttu-id="120df-438">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="120df-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="120df-439">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="120df-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="120df-440">请改用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="120df-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="120df-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="120df-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="120df-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-442">Boolean</span></span>|<span data-ttu-id="120df-443">指示在展台模式下是否阻止使用 "睡眠" 按钮。</span><span class="sxs-lookup"><span data-stu-id="120df-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="120df-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="120df-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-445">Boolean</span></span>|<span data-ttu-id="120df-446">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="120df-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="120df-447">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="120df-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="120df-448">请改用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="120df-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="120df-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="120df-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="120df-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-450">Boolean</span></span>|<span data-ttu-id="120df-451">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="120df-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="120df-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="120df-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-453">Boolean</span></span>|<span data-ttu-id="120df-454">指示是否在展台模式下启用语音控制。</span><span class="sxs-lookup"><span data-stu-id="120df-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="120df-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="120df-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="120df-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-456">Boolean</span></span>|<span data-ttu-id="120df-457">指示是否允许用户在展台模式下切换语音控件。</span><span class="sxs-lookup"><span data-stu-id="120df-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="120df-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="120df-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="120df-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-459">Boolean</span></span>|<span data-ttu-id="120df-460">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="120df-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="120df-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="120df-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-462">Boolean</span></span>|<span data-ttu-id="120df-463">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="120df-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="120df-464">此属性的功能对于 OS 默认值是多余的，已弃用。</span><span class="sxs-lookup"><span data-stu-id="120df-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="120df-465">请改用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="120df-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="120df-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="120df-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="120df-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-467">Boolean</span></span>|<span data-ttu-id="120df-468">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="120df-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="120df-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="120df-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="120df-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-470">Boolean</span></span>|<span data-ttu-id="120df-471">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="120df-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="120df-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="120df-473">String</span><span class="sxs-lookup"><span data-stu-id="120df-473">String</span></span>|<span data-ttu-id="120df-474">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="120df-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="120df-475">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="120df-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="120df-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="120df-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="120df-477">String</span><span class="sxs-lookup"><span data-stu-id="120df-477">String</span></span>|<span data-ttu-id="120df-478">用于展台模式的内置应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="120df-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="120df-479">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="120df-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="120df-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="120df-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="120df-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-481">Boolean</span></span>|<span data-ttu-id="120df-482">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="120df-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="120df-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="120df-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-484">Boolean</span></span>|<span data-ttu-id="120df-485">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="120df-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="120df-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="120df-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-487">Boolean</span></span>|<span data-ttu-id="120df-488">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="120df-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="120df-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="120df-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-490">Boolean</span></span>|<span data-ttu-id="120df-491">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="120df-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="120df-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="120df-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-493">Boolean</span></span>|<span data-ttu-id="120df-494">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="120df-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="120df-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="120df-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="120df-496">String</span><span class="sxs-lookup"><span data-stu-id="120df-496">String</span></span>|<span data-ttu-id="120df-497">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="120df-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="120df-498">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="120df-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="120df-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="120df-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="120df-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-500">Boolean</span></span>|<span data-ttu-id="120df-501">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="120df-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="120df-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="120df-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="120df-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-503">Boolean</span></span>|<span data-ttu-id="120df-504">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="120df-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="120df-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="120df-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="120df-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-506">Boolean</span></span>|<span data-ttu-id="120df-507">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="120df-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="120df-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="120df-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="120df-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-509">Boolean</span></span>|<span data-ttu-id="120df-510">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="120df-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="120df-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="120df-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="120df-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="120df-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="120df-513">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="120df-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="120df-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="120df-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="120df-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="120df-516">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="120df-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="120df-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="120df-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="120df-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="120df-519">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="120df-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="120df-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="120df-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="120df-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="120df-522">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="120df-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="120df-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="120df-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="120df-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="120df-525">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="120df-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="120df-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="120df-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="120df-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="120df-528">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="120df-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="120df-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="120df-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="120df-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="120df-531">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="120df-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="120df-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="120df-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="120df-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="120df-534">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="120df-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="120df-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="120df-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="120df-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="120df-537">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="120df-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="120df-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="120df-538">networkUsageRules</span></span>|<span data-ttu-id="120df-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="120df-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="120df-540">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="120df-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="120df-541">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="120df-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="120df-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="120df-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="120df-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="120df-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="120df-544">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="120df-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="120df-545">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="120df-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="120df-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-546">messagesBlocked</span></span>|<span data-ttu-id="120df-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-547">Boolean</span></span>|<span data-ttu-id="120df-548">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="120df-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="120df-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="120df-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="120df-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-550">Boolean</span></span>|<span data-ttu-id="120df-551">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="120df-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="120df-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="120df-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-553">Boolean</span></span>|<span data-ttu-id="120df-554">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="120df-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="120df-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="120df-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="120df-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-556">Boolean</span></span>|<span data-ttu-id="120df-557">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="120df-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="120df-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="120df-558">passcodeBlockModification</span></span>|<span data-ttu-id="120df-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-559">Boolean</span></span>|<span data-ttu-id="120df-560">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="120df-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="120df-561">passcodeBlockSimple</span></span>|<span data-ttu-id="120df-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-562">Boolean</span></span>|<span data-ttu-id="120df-563">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="120df-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="120df-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="120df-564">passcodeExpirationDays</span></span>|<span data-ttu-id="120df-565">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-565">Int32</span></span>|<span data-ttu-id="120df-566">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="120df-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="120df-567">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="120df-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="120df-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="120df-568">passcodeMinimumLength</span></span>|<span data-ttu-id="120df-569">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-569">Int32</span></span>|<span data-ttu-id="120df-570">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="120df-570">Minimum length of passcode.</span></span> <span data-ttu-id="120df-571">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="120df-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="120df-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="120df-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="120df-573">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-573">Int32</span></span>|<span data-ttu-id="120df-574">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="120df-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="120df-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="120df-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="120df-576">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-576">Int32</span></span>|<span data-ttu-id="120df-577">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="120df-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="120df-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="120df-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="120df-579">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-579">Int32</span></span>|<span data-ttu-id="120df-580">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="120df-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="120df-581">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="120df-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="120df-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="120df-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="120df-583">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-583">Int32</span></span>|<span data-ttu-id="120df-584">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="120df-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="120df-585">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="120df-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="120df-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="120df-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="120df-587">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-587">Int32</span></span>|<span data-ttu-id="120df-588">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="120df-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="120df-589">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="120df-589">Valid values 4 to 11</span></span>|
|<span data-ttu-id="120df-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="120df-590">passcodeRequiredType</span></span>|[<span data-ttu-id="120df-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="120df-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="120df-592">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="120df-592">Type of passcode that is required.</span></span> <span data-ttu-id="120df-593">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="120df-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="120df-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="120df-594">passcodeRequired</span></span>|<span data-ttu-id="120df-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-595">Boolean</span></span>|<span data-ttu-id="120df-596">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="120df-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="120df-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-597">podcastsBlocked</span></span>|<span data-ttu-id="120df-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-598">Boolean</span></span>|<span data-ttu-id="120df-599">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="120df-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="120df-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="120df-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-601">Boolean</span></span>|<span data-ttu-id="120df-602">指示是否启用提示以在受监督的设备上安装附近设备。</span><span class="sxs-lookup"><span data-stu-id="120df-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="120df-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="120df-603">safariBlockAutofill</span></span>|<span data-ttu-id="120df-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-604">Boolean</span></span>|<span data-ttu-id="120df-605">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="120df-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="120df-606">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="120df-607">safariBlockJavaScript</span></span>|<span data-ttu-id="120df-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-608">Boolean</span></span>|<span data-ttu-id="120df-609">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="120df-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="120df-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="120df-610">safariBlockPopups</span></span>|<span data-ttu-id="120df-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-611">Boolean</span></span>|<span data-ttu-id="120df-612">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="120df-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="120df-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-613">safariBlocked</span></span>|<span data-ttu-id="120df-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-614">Boolean</span></span>|<span data-ttu-id="120df-615">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="120df-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="120df-616">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="120df-617">safariCookieSettings</span></span>|[<span data-ttu-id="120df-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="120df-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="120df-619">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="120df-619">Cookie settings for Safari.</span></span> <span data-ttu-id="120df-620">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="120df-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="120df-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="120df-621">safariManagedDomains</span></span>|<span data-ttu-id="120df-622">String 集合</span><span class="sxs-lookup"><span data-stu-id="120df-622">String collection</span></span>|<span data-ttu-id="120df-623">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="120df-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="120df-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="120df-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="120df-625">String 集合</span><span class="sxs-lookup"><span data-stu-id="120df-625">String collection</span></span>|<span data-ttu-id="120df-626">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="120df-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="120df-627">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="120df-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="120df-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="120df-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-629">Boolean</span></span>|<span data-ttu-id="120df-630">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="120df-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="120df-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-631">screenCaptureBlocked</span></span>|<span data-ttu-id="120df-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-632">Boolean</span></span>|<span data-ttu-id="120df-633">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="120df-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="120df-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-634">siriBlocked</span></span>|<span data-ttu-id="120df-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-635">Boolean</span></span>|<span data-ttu-id="120df-636">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="120df-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="120df-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="120df-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="120df-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-638">Boolean</span></span>|<span data-ttu-id="120df-639">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="120df-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="120df-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="120df-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="120df-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-641">Boolean</span></span>|<span data-ttu-id="120df-642">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="120df-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="120df-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="120df-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="120df-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-644">Boolean</span></span>|<span data-ttu-id="120df-645">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="120df-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="120df-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="120df-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="120df-647">Int32</span><span class="sxs-lookup"><span data-stu-id="120df-647">Int32</span></span>|<span data-ttu-id="120df-648">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="120df-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="120df-649">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="120df-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="120df-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="120df-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="120df-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-651">Boolean</span></span>|<span data-ttu-id="120df-652">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="120df-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="120df-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="120df-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-654">Boolean</span></span>|<span data-ttu-id="120df-655">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="120df-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="120df-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-656">voiceDialingBlocked</span></span>|<span data-ttu-id="120df-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-657">Boolean</span></span>|<span data-ttu-id="120df-658">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="120df-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="120df-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="120df-659">wallpaperBlockModification</span></span>|<span data-ttu-id="120df-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-660">Boolean</span></span>|<span data-ttu-id="120df-661">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="120df-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="120df-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="120df-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-663">Boolean</span></span>|<span data-ttu-id="120df-664">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="120df-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="120df-665">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="120df-665">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="120df-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-666">Boolean</span></span>|<span data-ttu-id="120df-667">指示在非托管课程中通过教室注册的学生是否会在尝试离开该课程（iOS 11.3 及更高版本）时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="120df-667">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="120df-668">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="120df-668">keychainBlockCloudSync</span></span>|<span data-ttu-id="120df-669">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-669">Boolean</span></span>|<span data-ttu-id="120df-670">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="120df-670">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="120df-671">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-671">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-672">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="120df-672">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="120df-673">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-673">Boolean</span></span>|<span data-ttu-id="120df-674">指示是否阻止无线 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="120df-674">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="120df-675">将此限制设置为 false 不会禁用 CRL 和 OCSP 检查（iOS 7.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-675">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="120df-676">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="120df-676">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="120df-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-677">Boolean</span></span>|<span data-ttu-id="120df-678">指示广告跟踪是否受限制。（iOS 7.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-678">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="120df-679">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="120df-679">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="120df-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-680">Boolean</span></span>|<span data-ttu-id="120df-681">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="120df-681">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="120df-682">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="120df-682">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="120df-683">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-683">Boolean</span></span>|<span data-ttu-id="120df-684">指示是否阻止企业书籍笔记和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="120df-684">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="120df-685">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-685">airPrintBlocked</span></span>|<span data-ttu-id="120df-686">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-686">Boolean</span></span>|<span data-ttu-id="120df-687">指示是否阻止 AirPrint （iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-687">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="120df-688">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="120df-688">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="120df-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-689">Boolean</span></span>|<span data-ttu-id="120df-690">指示是否阻止 Airprint 的用户名和密码的密钥链存储（iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-690">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="120df-691">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="120df-691">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="120df-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-692">Boolean</span></span>|<span data-ttu-id="120df-693">指示 TLS 打印通信是否需要受信任的证书（iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-693">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="120df-694">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="120df-694">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="120df-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-695">Boolean</span></span>|<span data-ttu-id="120df-696">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="120df-696">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="120df-697">这样可以防止虚假的 AirPrint 蓝牙信号免受网络流量（iOS 11.0 及更高版本）的欺骗。</span><span class="sxs-lookup"><span data-stu-id="120df-697">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="120df-698">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-698">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="120df-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-699">Boolean</span></span>|<span data-ttu-id="120df-700">指示设备是否可以使用服务器消息块（SMB）协议访问网络服务器上的文件或其他资源。</span><span class="sxs-lookup"><span data-stu-id="120df-700">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="120df-701">适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="120df-701">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="120df-702">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-702">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="120df-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-703">Boolean</span></span>|<span data-ttu-id="120df-704">指示带 access 的 sevices 是否可以连接到 USB 驱动器上的文件并打开文件。</span><span class="sxs-lookup"><span data-stu-id="120df-704">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="120df-705">适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="120df-705">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="120df-706">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="120df-706">wifiPowerOnForced</span></span>|<span data-ttu-id="120df-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-707">Boolean</span></span>|<span data-ttu-id="120df-708">指示 Wi-fi 是否仍处于打开状态，即使设备处于飞行模式时也是如此。</span><span class="sxs-lookup"><span data-stu-id="120df-708">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="120df-709">适用于运行 iOS 和 iPadOS 版本13.0 及更高版本的设备。</span><span class="sxs-lookup"><span data-stu-id="120df-709">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="120df-710">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="120df-710">blockSystemAppRemoval</span></span>|<span data-ttu-id="120df-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-711">Boolean</span></span>|<span data-ttu-id="120df-712">指示是否在受监督的设备（iOS 11.0 及更高版本）上阻止从设备中删除系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="120df-712">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="120df-713">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="120df-713">vpnBlockCreation</span></span>|<span data-ttu-id="120df-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-714">Boolean</span></span>|<span data-ttu-id="120df-715">指示是否阻止创建 VPN 配置（iOS 11.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-715">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="120df-716">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-716">appRemovalBlocked</span></span>|<span data-ttu-id="120df-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-717">Boolean</span></span>|<span data-ttu-id="120df-718">指示是否允许删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="120df-718">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="120df-719">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-719">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="120df-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-720">Boolean</span></span>|<span data-ttu-id="120df-721">指示是否允许在锁定设备时连接到 USB 附件（iOS 11.4.1 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-721">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="120df-722">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="120df-722">passwordBlockAutoFill</span></span>|<span data-ttu-id="120df-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-723">Boolean</span></span>|<span data-ttu-id="120df-724">指示是否允许自动填充密码功能（iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-724">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="120df-725">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="120df-725">passwordBlockProximityRequests</span></span>|<span data-ttu-id="120df-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-726">Boolean</span></span>|<span data-ttu-id="120df-727">指示是否阻止来自附近设备（iOS 12.0 及更高版本）发出请求的密码。</span><span class="sxs-lookup"><span data-stu-id="120df-727">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="120df-728">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="120df-728">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="120df-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-729">Boolean</span></span>|<span data-ttu-id="120df-730">指示是否阻止使用 AirDrop 密码的共享密码功能 iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-730">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="120df-731">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="120df-731">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="120df-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-732">Boolean</span></span>|<span data-ttu-id="120df-733">指示是否启用日期和时间 "设置自动设置" 功能，以及用户是否无法关闭该功能（iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-733">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="120df-734">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="120df-734">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="120df-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-735">Boolean</span></span>|<span data-ttu-id="120df-736">指示托管应用程序是否可以将联系人写入非托管联系人帐户（iOS 12.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-736">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="120df-737">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="120df-737">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="120df-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-738">Boolean</span></span>|<span data-ttu-id="120df-739">指示非托管应用是否可以从托管联系人帐户读取（iOS 12.0 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-739">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="120df-740">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="120df-740">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="120df-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-741">Boolean</span></span>|<span data-ttu-id="120df-742">指示是否阻止用户修改个人热点设置（iOS 12.2 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-742">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="120df-743">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-743">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="120df-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-744">Boolean</span></span>|<span data-ttu-id="120df-745">指示设备受到监督时是否阻止连续路径键盘（iOS 13 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-745">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="120df-746">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-746">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="120df-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-747">Boolean</span></span>|<span data-ttu-id="120df-748">指示设备受到监督时是否阻止查找我的设备（iOS 13 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-748">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="120df-749">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-749">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="120df-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-750">Boolean</span></span>|<span data-ttu-id="120df-751">指示设备受到监督时是否阻止查找我的好友（iOS 13 或更高版本）。</span><span class="sxs-lookup"><span data-stu-id="120df-751">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="120df-752">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="120df-752">iTunesBlocked</span></span>|<span data-ttu-id="120df-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="120df-753">Boolean</span></span>|<span data-ttu-id="120df-754">指示是否阻止 iTunes 应用。</span><span class="sxs-lookup"><span data-stu-id="120df-754">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="120df-755">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="120df-755">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="120df-756">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="120df-756">kioskModeAppType</span></span>|[<span data-ttu-id="120df-757">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="120df-757">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="120df-758">在展台模式下运行的应用类型。</span><span class="sxs-lookup"><span data-stu-id="120df-758">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="120df-759">可取值为：`notConfigured`、`appStoreApp`、`managedApp`、`builtInApp`。</span><span class="sxs-lookup"><span data-stu-id="120df-759">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="120df-760">响应</span><span class="sxs-lookup"><span data-stu-id="120df-760">Response</span></span>
<span data-ttu-id="120df-761">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="120df-761">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="120df-762">示例</span><span class="sxs-lookup"><span data-stu-id="120df-762">Example</span></span>

### <a name="request"></a><span data-ttu-id="120df-763">请求</span><span class="sxs-lookup"><span data-stu-id="120df-763">Request</span></span>
<span data-ttu-id="120df-764">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="120df-764">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="120df-765">响应</span><span class="sxs-lookup"><span data-stu-id="120df-765">Response</span></span>
<span data-ttu-id="120df-p157">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="120df-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



