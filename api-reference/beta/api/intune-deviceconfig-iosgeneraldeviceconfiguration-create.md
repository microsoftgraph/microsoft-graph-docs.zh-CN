---
title: 创建 iosGeneralDeviceConfiguration
description: 创建新的 iosGeneralDeviceConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 507b190d719d20991419a573ae7f1025b8070f06
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315917"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="c6931-103">创建 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6931-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c6931-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6931-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6931-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6931-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6931-106">创建新的 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6931-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6931-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6931-107">Prerequisites</span></span>
<span data-ttu-id="c6931-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6931-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6931-110">Permission type</span></span>|<span data-ttu-id="c6931-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6931-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6931-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6931-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6931-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6931-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6931-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6931-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6931-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6931-115">Not supported.</span></span>|
|<span data-ttu-id="c6931-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6931-116">Application</span></span>|<span data-ttu-id="c6931-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6931-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6931-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6931-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c6931-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6931-119">Request headers</span></span>
|<span data-ttu-id="c6931-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6931-120">Header</span></span>|<span data-ttu-id="c6931-121">值</span><span class="sxs-lookup"><span data-stu-id="c6931-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6931-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6931-122">Authorization</span></span>|<span data-ttu-id="c6931-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6931-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6931-124">接受</span><span class="sxs-lookup"><span data-stu-id="c6931-124">Accept</span></span>|<span data-ttu-id="c6931-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6931-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6931-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6931-126">Request body</span></span>
<span data-ttu-id="c6931-127">在请求正文中，提供 iosGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6931-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c6931-128">下表显示创建 iosGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6931-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c6931-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6931-129">Property</span></span>|<span data-ttu-id="c6931-130">类型</span><span class="sxs-lookup"><span data-stu-id="c6931-130">Type</span></span>|<span data-ttu-id="c6931-131">说明</span><span class="sxs-lookup"><span data-stu-id="c6931-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6931-132">id</span><span class="sxs-lookup"><span data-stu-id="c6931-132">id</span></span>|<span data-ttu-id="c6931-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c6931-133">String</span></span>|<span data-ttu-id="c6931-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c6931-134">Key of the entity.</span></span> <span data-ttu-id="c6931-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6931-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c6931-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6931-137">DateTimeOffset</span></span>|<span data-ttu-id="c6931-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c6931-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c6931-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c6931-140">roleScopeTagIds</span></span>|<span data-ttu-id="c6931-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c6931-141">String collection</span></span>|<span data-ttu-id="c6931-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c6931-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c6931-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c6931-144">supportsScopeTags</span></span>|<span data-ttu-id="c6931-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-145">Boolean</span></span>|<span data-ttu-id="c6931-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c6931-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c6931-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c6931-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c6931-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c6931-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c6931-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c6931-149">This property is read-only.</span></span> <span data-ttu-id="c6931-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c6931-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c6931-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c6931-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c6931-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c6931-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c6931-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c6931-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c6931-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c6931-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c6931-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c6931-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c6931-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c6931-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c6931-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c6931-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c6931-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c6931-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6931-163">createdDateTime</span></span>|<span data-ttu-id="c6931-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6931-164">DateTimeOffset</span></span>|<span data-ttu-id="c6931-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c6931-165">DateTime the object was created.</span></span> <span data-ttu-id="c6931-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-167">说明</span><span class="sxs-lookup"><span data-stu-id="c6931-167">description</span></span>|<span data-ttu-id="c6931-168">String</span><span class="sxs-lookup"><span data-stu-id="c6931-168">String</span></span>|<span data-ttu-id="c6931-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c6931-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c6931-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c6931-171">displayName</span></span>|<span data-ttu-id="c6931-172">String</span><span class="sxs-lookup"><span data-stu-id="c6931-172">String</span></span>|<span data-ttu-id="c6931-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c6931-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c6931-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-175">version</span><span class="sxs-lookup"><span data-stu-id="c6931-175">version</span></span>|<span data-ttu-id="c6931-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-176">Int32</span></span>|<span data-ttu-id="c6931-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-177">Version of the device configuration.</span></span> <span data-ttu-id="c6931-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6931-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c6931-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="c6931-179">accountBlockModification</span></span>|<span data-ttu-id="c6931-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-180">Boolean</span></span>|<span data-ttu-id="c6931-181">指示设备处于监督模式时是否允许帐户修改。</span><span class="sxs-lookup"><span data-stu-id="c6931-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="c6931-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="c6931-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-183">Boolean</span></span>|<span data-ttu-id="c6931-184">指示设备处于监督模式时是否允许激活锁定。</span><span class="sxs-lookup"><span data-stu-id="c6931-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="c6931-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-185">airDropBlocked</span></span>|<span data-ttu-id="c6931-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-186">Boolean</span></span>|<span data-ttu-id="c6931-187">指示设备处于监督模式时是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="c6931-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="c6931-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="c6931-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-189">Boolean</span></span>|<span data-ttu-id="c6931-190">指示是否导致将 AirDrop 视为非托管放置目标（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="c6931-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="c6931-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-192">Boolean</span></span>|<span data-ttu-id="c6931-193">指示是否强制所有接收来自此设备的 AirPlay 请求的设备使用配对密码。</span><span class="sxs-lookup"><span data-stu-id="c6931-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="c6931-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="c6931-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="c6931-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-195">Boolean</span></span>|<span data-ttu-id="c6931-196">指示设备处于监督模式时是否允许 Apple Watch 配对（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="c6931-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="c6931-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-198">Boolean</span></span>|<span data-ttu-id="c6931-199">指示是否强制已配对的 Apple Watch 使用手腕检测（iOS 8.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="c6931-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-200">appleNewsBlocked</span></span>|<span data-ttu-id="c6931-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-201">Boolean</span></span>|<span data-ttu-id="c6931-202">指示设备处于监督模式时是否阻止用户使用新闻（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="c6931-203">appsSingleAppModeList</span></span>|<span data-ttu-id="c6931-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6931-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c6931-205">获取或设置允许自主进入单个应用模式的 iOS 应用列表。</span><span class="sxs-lookup"><span data-stu-id="c6931-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="c6931-206">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="c6931-206">Supervised only.</span></span> <span data-ttu-id="c6931-207">iOS 7.0 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-207">iOS 7.0 and later.</span></span> <span data-ttu-id="c6931-208">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c6931-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c6931-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="c6931-209">appsVisibilityList</span></span>|<span data-ttu-id="c6931-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6931-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c6931-211">可见性列表中的应用列表（可见/可启动应用列表或隐藏/不可启动应用列表，由 AppsVisibilityListType 控制）（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="c6931-212">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c6931-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c6931-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="c6931-213">appsVisibilityListType</span></span>|[<span data-ttu-id="c6931-214">appListType</span><span class="sxs-lookup"><span data-stu-id="c6931-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c6931-215">位于 AppsVisibilityList 中的列表类型。</span><span class="sxs-lookup"><span data-stu-id="c6931-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="c6931-216">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="c6931-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c6931-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="c6931-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="c6931-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-218">Boolean</span></span>|<span data-ttu-id="c6931-219">指示设备处于监督模式时是否阻止自动下载在其他设备上购买的应用（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-220">appStoreBlocked</span></span>|<span data-ttu-id="c6931-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-221">Boolean</span></span>|<span data-ttu-id="c6931-222">指示是否阻止用户使用 App Store。</span><span class="sxs-lookup"><span data-stu-id="c6931-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="c6931-223">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="c6931-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="c6931-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-225">Boolean</span></span>|<span data-ttu-id="c6931-226">指示是否阻止用户进行应用内购买。</span><span class="sxs-lookup"><span data-stu-id="c6931-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="c6931-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c6931-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="c6931-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-228">Boolean</span></span>|<span data-ttu-id="c6931-229">指示是否阻止 App Store 应用，而不通过主机应用限制安装。</span><span class="sxs-lookup"><span data-stu-id="c6931-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="c6931-230">仅适用于监督模式（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="c6931-231">appStoreRequirePassword</span></span>|<span data-ttu-id="c6931-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-232">Boolean</span></span>|<span data-ttu-id="c6931-233">指示使用 App Store 时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c6931-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="c6931-234">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="c6931-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="c6931-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-235">Boolean</span></span>|<span data-ttu-id="c6931-236">指示在 Safari 中的 autofilling 密码和信用卡信息之前是否强制进行用户身份验证, 以及受监督的设备上的其他应用。</span><span class="sxs-lookup"><span data-stu-id="c6931-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="c6931-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="c6931-237">bluetoothBlockModification</span></span>|<span data-ttu-id="c6931-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-238">Boolean</span></span>|<span data-ttu-id="c6931-239">指示设备处于监督模式时是否允许修改蓝牙设置（iOS 10.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="c6931-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-240">cameraBlocked</span></span>|<span data-ttu-id="c6931-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-241">Boolean</span></span>|<span data-ttu-id="c6931-242">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="c6931-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="c6931-243">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c6931-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c6931-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-245">Boolean</span></span>|<span data-ttu-id="c6931-246">指示是否阻止数据漫游。</span><span class="sxs-lookup"><span data-stu-id="c6931-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c6931-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="c6931-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="c6931-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-248">Boolean</span></span>|<span data-ttu-id="c6931-249">指示漫游时是否阻止全局背景提取。</span><span class="sxs-lookup"><span data-stu-id="c6931-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="c6931-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="c6931-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="c6931-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-251">Boolean</span></span>|<span data-ttu-id="c6931-252">指示设备处于监督模式时是否允许更改手机应用数据使用设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="c6931-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="c6931-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-254">Boolean</span></span>|<span data-ttu-id="c6931-255">指示是否阻止个人热点。</span><span class="sxs-lookup"><span data-stu-id="c6931-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="c6931-256">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="c6931-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="c6931-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-257">Boolean</span></span>|<span data-ttu-id="c6931-258">指示是否允许用户在受监督的设备上更改移动电话计划的设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="c6931-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="c6931-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="c6931-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-260">Boolean</span></span>|<span data-ttu-id="c6931-261">指示是否阻止语音漫游。</span><span class="sxs-lookup"><span data-stu-id="c6931-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="c6931-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="c6931-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="c6931-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-263">Boolean</span></span>|<span data-ttu-id="c6931-264">指示是否阻止不受信任的 TLS 证书。</span><span class="sxs-lookup"><span data-stu-id="c6931-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="c6931-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c6931-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="c6931-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-266">Boolean</span></span>|<span data-ttu-id="c6931-267">指示设备处于监督模式时是否允许 Classroom 应用进行远程屏幕观察（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c6931-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c6931-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="c6931-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-269">Boolean</span></span>|<span data-ttu-id="c6931-270">指示是否自动授予 Classroom 应用上托管课程的教师权限，以便在设备处于监督模式时查看学生的屏幕且不会出现提示。</span><span class="sxs-lookup"><span data-stu-id="c6931-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-271">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="c6931-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="c6931-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-272">Boolean</span></span>|<span data-ttu-id="c6931-273">指示设备处于监督模式时是否自动向教师的请求授予权限, 而不提示学生。</span><span class="sxs-lookup"><span data-stu-id="c6931-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-274">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="c6931-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="c6931-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-275">Boolean</span></span>|<span data-ttu-id="c6931-276">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="c6931-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="c6931-277">仅限监督模式。</span><span class="sxs-lookup"><span data-stu-id="c6931-277">Supervised only.</span></span>|
|<span data-ttu-id="c6931-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c6931-278">compliantAppsList</span></span>|<span data-ttu-id="c6931-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6931-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c6931-280">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="c6931-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c6931-281">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c6931-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c6931-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c6931-282">compliantAppListType</span></span>|[<span data-ttu-id="c6931-283">appListType</span><span class="sxs-lookup"><span data-stu-id="c6931-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c6931-284">位于 AppComplianceList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="c6931-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="c6931-285">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="c6931-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c6931-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="c6931-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="c6931-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-287">Boolean</span></span>|<span data-ttu-id="c6931-288">指示设备处于监督模式时是否阻止用户以交互方式安装配置文件和证书。</span><span class="sxs-lookup"><span data-stu-id="c6931-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-289">definitionLookupBlocked</span></span>|<span data-ttu-id="c6931-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-290">Boolean</span></span>|<span data-ttu-id="c6931-291">指示设备处于监督模式时是否阻止定义查找（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="c6931-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="c6931-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="c6931-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-293">Boolean</span></span>|<span data-ttu-id="c6931-294">指示设备处于监督模式时是否允许用户在设备设置中启用限制。</span><span class="sxs-lookup"><span data-stu-id="c6931-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="c6931-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-296">Boolean</span></span>|<span data-ttu-id="c6931-297">指示设备处于监督模式时是否允许使用设备上的“擦除所有内容和设置”选项。</span><span class="sxs-lookup"><span data-stu-id="c6931-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="c6931-298">deviceBlockNameModification</span></span>|<span data-ttu-id="c6931-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-299">Boolean</span></span>|<span data-ttu-id="c6931-300">指示设备处于监督模式时是否允许修改设备名称（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c6931-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c6931-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-302">Boolean</span></span>|<span data-ttu-id="c6931-303">指示是否阻止诊断数据提交。</span><span class="sxs-lookup"><span data-stu-id="c6931-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c6931-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="c6931-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="c6931-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-305">Boolean</span></span>|<span data-ttu-id="c6931-306">指示设备处于监督模式时是否允许修改诊断提交设置（iOS 9.3.2 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="c6931-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="c6931-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="c6931-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-308">Boolean</span></span>|<span data-ttu-id="c6931-309">指示是否阻止用户查看非托管应用中的托管文档。</span><span class="sxs-lookup"><span data-stu-id="c6931-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="c6931-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="c6931-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="c6931-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-311">Boolean</span></span>|<span data-ttu-id="c6931-312">指示是否阻止用户查看托管应用中的非托管文档。</span><span class="sxs-lookup"><span data-stu-id="c6931-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="c6931-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c6931-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="c6931-314">String 集合</span><span class="sxs-lookup"><span data-stu-id="c6931-314">String collection</span></span>|<span data-ttu-id="c6931-315">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="c6931-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c6931-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="c6931-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="c6931-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-317">Boolean</span></span>|<span data-ttu-id="c6931-318">指示是否阻止用户信任企业应用。</span><span class="sxs-lookup"><span data-stu-id="c6931-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="c6931-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="c6931-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="c6931-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-320">Boolean</span></span>|<span data-ttu-id="c6931-321">指示是否阻止用户修改企业应用信任设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-321">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="c6931-322">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="c6931-322">esimBlockModification</span></span>|<span data-ttu-id="c6931-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-323">Boolean</span></span>|<span data-ttu-id="c6931-324">指示是否允许在受监督的设备的 eSIM 卡上添加或删除手机网络计划。</span><span class="sxs-lookup"><span data-stu-id="c6931-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="c6931-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-325">faceTimeBlocked</span></span>|<span data-ttu-id="c6931-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-326">Boolean</span></span>|<span data-ttu-id="c6931-327">指示是否阻止用户使用 FaceTime。</span><span class="sxs-lookup"><span data-stu-id="c6931-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="c6931-328">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="c6931-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-330">Boolean</span></span>|<span data-ttu-id="c6931-331">指示设备处于监督模式时是否阻止更改以查找我的好友。</span><span class="sxs-lookup"><span data-stu-id="c6931-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="c6931-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="c6931-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-333">Boolean</span></span>|<span data-ttu-id="c6931-334">指示是否阻止用户在 Game Center 中拥有好友。</span><span class="sxs-lookup"><span data-stu-id="c6931-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="c6931-335">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="c6931-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="c6931-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-337">Boolean</span></span>|<span data-ttu-id="c6931-338">指示是否阻止用户使用多人游戏。</span><span class="sxs-lookup"><span data-stu-id="c6931-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="c6931-339">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-340">gameCenterBlocked</span></span>|<span data-ttu-id="c6931-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-341">Boolean</span></span>|<span data-ttu-id="c6931-342">指示设备处于监督模式时是否阻止用户使用 Game Center。</span><span class="sxs-lookup"><span data-stu-id="c6931-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-343">hostPairingBlocked</span></span>|<span data-ttu-id="c6931-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-344">Boolean</span></span>|<span data-ttu-id="c6931-345">指示 iOS 设备处于监督模式时是否允许主机配对控制 iOS 设备可以与之配对的设备。</span><span class="sxs-lookup"><span data-stu-id="c6931-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="c6931-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-347">Boolean</span></span>|<span data-ttu-id="c6931-348">指示设备处于监督模式时是否阻止用户使用 iBooks Store。</span><span class="sxs-lookup"><span data-stu-id="c6931-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="c6931-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="c6931-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-350">Boolean</span></span>|<span data-ttu-id="c6931-351">指示是否阻止用户从已标记为情色的 iBookstore 下载媒体。</span><span class="sxs-lookup"><span data-stu-id="c6931-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="c6931-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="c6931-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="c6931-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-353">Boolean</span></span>|<span data-ttu-id="c6931-354">指示是否阻止用户将其在 iOS 设备上启动的工作继续到另一个 iOS 或 macOS 设备。</span><span class="sxs-lookup"><span data-stu-id="c6931-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="c6931-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="c6931-355">iCloudBlockBackup</span></span>|<span data-ttu-id="c6931-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-356">Boolean</span></span>|<span data-ttu-id="c6931-357">指示是否阻止 iCloud 备份。</span><span class="sxs-lookup"><span data-stu-id="c6931-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="c6931-358">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="c6931-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="c6931-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-360">Boolean</span></span>|<span data-ttu-id="c6931-361">指示是否阻止 iCloud 文档同步。需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="c6931-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="c6931-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-363">Boolean</span></span>|<span data-ttu-id="c6931-364">指示是否阻止托管应用云同步。</span><span class="sxs-lookup"><span data-stu-id="c6931-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="c6931-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="c6931-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="c6931-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-366">Boolean</span></span>|<span data-ttu-id="c6931-367">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="c6931-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="c6931-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="c6931-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="c6931-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-369">Boolean</span></span>|<span data-ttu-id="c6931-370">指示是否阻止 iCloud 照片流同步。</span><span class="sxs-lookup"><span data-stu-id="c6931-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="c6931-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="c6931-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="c6931-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-372">Boolean</span></span>|<span data-ttu-id="c6931-373">指示是否阻止共享照片流。</span><span class="sxs-lookup"><span data-stu-id="c6931-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="c6931-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="c6931-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="c6931-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-375">Boolean</span></span>|<span data-ttu-id="c6931-376">指示是否要求加密备份到 iCloud 的数据。</span><span class="sxs-lookup"><span data-stu-id="c6931-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="c6931-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="c6931-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="c6931-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-378">Boolean</span></span>|<span data-ttu-id="c6931-379">指示是否阻止用户访问 iTunes 和 App Store 中的显式内容。</span><span class="sxs-lookup"><span data-stu-id="c6931-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="c6931-380">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="c6931-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="c6931-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-382">Boolean</span></span>|<span data-ttu-id="c6931-383">指示设备处于监督模式时是否阻止音乐服务并将音乐应用恢复为经典模式（iOS 9.3 及更高版本和 MacOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c6931-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="c6931-384">iTunesBlockRadio</span></span>|<span data-ttu-id="c6931-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-385">Boolean</span></span>|<span data-ttu-id="c6931-386">指示设备处于监督模式时是否阻止用户使用 iTunes Radio（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c6931-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="c6931-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="c6931-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-388">Boolean</span></span>|<span data-ttu-id="c6931-389">指示设备处于监督模式时是否阻止键盘自动更正（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="c6931-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="c6931-390">keyboardBlockDictation</span></span>|<span data-ttu-id="c6931-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-391">Boolean</span></span>|<span data-ttu-id="c6931-392">指示设备处于监督模式时是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="c6931-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="c6931-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="c6931-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-394">Boolean</span></span>|<span data-ttu-id="c6931-395">指示设备处于监督模式时是否阻止预测键盘（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="c6931-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="c6931-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="c6931-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-397">Boolean</span></span>|<span data-ttu-id="c6931-398">指示设备处于监督模式时是否阻止键盘快捷键（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="c6931-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="c6931-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-400">Boolean</span></span>|<span data-ttu-id="c6931-401">指示设备处于监督模式时是否阻止键盘拼写检查（iOS 8.1.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="c6931-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="c6931-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="c6931-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-403">Boolean</span></span>|<span data-ttu-id="c6931-404">指示在展台模式下是否允许辅助朗读。</span><span class="sxs-lookup"><span data-stu-id="c6931-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="c6931-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-406">Boolean</span></span>|<span data-ttu-id="c6931-407">指示在展台模式下是否允许访问辅助触摸设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="c6931-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="c6931-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-409">Boolean</span></span>|<span data-ttu-id="c6931-410">指示在展台模式下是否允许设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="c6931-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="c6931-411">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="c6931-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="c6931-412">请改用 KioskModeBlockAutoLock。</span><span class="sxs-lookup"><span data-stu-id="c6931-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="c6931-413">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="c6931-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="c6931-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-414">Boolean</span></span>|<span data-ttu-id="c6931-415">指示在展台模式下是否阻止设备自动锁定。</span><span class="sxs-lookup"><span data-stu-id="c6931-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="c6931-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-417">Boolean</span></span>|<span data-ttu-id="c6931-418">指示在展台模式下是否允许访问颜色反转设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="c6931-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="c6931-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-420">Boolean</span></span>|<span data-ttu-id="c6931-421">指示在展台模式下是否允许使用响铃开关。</span><span class="sxs-lookup"><span data-stu-id="c6931-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="c6931-422">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="c6931-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="c6931-423">请改用 KioskModeBlockRingerSwitch。</span><span class="sxs-lookup"><span data-stu-id="c6931-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="c6931-424">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="c6931-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="c6931-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-425">Boolean</span></span>|<span data-ttu-id="c6931-426">指示在展台模式下是否阻止使用铃声开关。</span><span class="sxs-lookup"><span data-stu-id="c6931-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="c6931-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="c6931-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-428">Boolean</span></span>|<span data-ttu-id="c6931-429">指示在展台模式下是否允许屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="c6931-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="c6931-430">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="c6931-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="c6931-431">请改用 KioskModeBlockScreenRotation。</span><span class="sxs-lookup"><span data-stu-id="c6931-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="c6931-432">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="c6931-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="c6931-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-433">Boolean</span></span>|<span data-ttu-id="c6931-434">指示在展台模式下是否阻止屏幕旋转。</span><span class="sxs-lookup"><span data-stu-id="c6931-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="c6931-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="c6931-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-436">Boolean</span></span>|<span data-ttu-id="c6931-437">指示在展台模式下是否允许使用睡眠按钮。</span><span class="sxs-lookup"><span data-stu-id="c6931-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="c6931-438">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="c6931-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="c6931-439">请改用 KioskModeBlockSleepButton。</span><span class="sxs-lookup"><span data-stu-id="c6931-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="c6931-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="c6931-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="c6931-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-441">Boolean</span></span>|<span data-ttu-id="c6931-442">指示在展台模式下是否阻止使用 "睡眠" 按钮。</span><span class="sxs-lookup"><span data-stu-id="c6931-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="c6931-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="c6931-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-444">Boolean</span></span>|<span data-ttu-id="c6931-445">指示在展台模式下是否允许使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="c6931-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="c6931-446">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="c6931-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="c6931-447">请改用 KioskModeBlockTouchscreen。</span><span class="sxs-lookup"><span data-stu-id="c6931-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="c6931-448">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="c6931-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="c6931-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-449">Boolean</span></span>|<span data-ttu-id="c6931-450">指示在展台模式下是否阻止使用触摸屏。</span><span class="sxs-lookup"><span data-stu-id="c6931-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-451">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-451">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="c6931-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-452">Boolean</span></span>|<span data-ttu-id="c6931-453">指示在展台模式下是否允许访问语音插入设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-453">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-454">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="c6931-454">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="c6931-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-455">Boolean</span></span>|<span data-ttu-id="c6931-456">指示在展台模式下是否允许使用音量按钮。</span><span class="sxs-lookup"><span data-stu-id="c6931-456">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="c6931-457">此属性的功能对于 OS 默认值是多余的, 已弃用。</span><span class="sxs-lookup"><span data-stu-id="c6931-457">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="c6931-458">请改用 KioskModeBlockVolumeButtons。</span><span class="sxs-lookup"><span data-stu-id="c6931-458">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="c6931-459">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="c6931-459">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="c6931-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-460">Boolean</span></span>|<span data-ttu-id="c6931-461">指示在展台模式下是否阻止音量按钮。</span><span class="sxs-lookup"><span data-stu-id="c6931-461">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c6931-462">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-462">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="c6931-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-463">Boolean</span></span>|<span data-ttu-id="c6931-464">指示在展台模式下是否允许访问缩放设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-464">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-465">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c6931-465">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="c6931-466">String</span><span class="sxs-lookup"><span data-stu-id="c6931-466">String</span></span>|<span data-ttu-id="c6931-467">指向 App Store 中要用于展台模式的应用的 URL。</span><span class="sxs-lookup"><span data-stu-id="c6931-467">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="c6931-468">如果 KioskModeManagedAppId 未知，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="c6931-468">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="c6931-469">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="c6931-469">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="c6931-470">String</span><span class="sxs-lookup"><span data-stu-id="c6931-470">String</span></span>|<span data-ttu-id="c6931-471">用于展台模式的内置应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6931-471">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="c6931-472">在未设置 KioskModeManagedAppId 和 KioskModeAppStoreUrl 时使用。</span><span class="sxs-lookup"><span data-stu-id="c6931-472">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="c6931-473">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="c6931-473">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="c6931-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-474">Boolean</span></span>|<span data-ttu-id="c6931-475">指示在展台模式下是否要求辅助触摸。</span><span class="sxs-lookup"><span data-stu-id="c6931-475">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-476">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="c6931-476">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="c6931-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-477">Boolean</span></span>|<span data-ttu-id="c6931-478">指示在展台模式下是否要求颜色反转。</span><span class="sxs-lookup"><span data-stu-id="c6931-478">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-479">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="c6931-479">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="c6931-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-480">Boolean</span></span>|<span data-ttu-id="c6931-481">指示在展台模式下是否要求单声道音频。</span><span class="sxs-lookup"><span data-stu-id="c6931-481">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-482">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="c6931-482">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="c6931-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-483">Boolean</span></span>|<span data-ttu-id="c6931-484">指示在展台模式下是否要求语音插入。</span><span class="sxs-lookup"><span data-stu-id="c6931-484">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-485">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="c6931-485">kioskModeRequireZoom</span></span>|<span data-ttu-id="c6931-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-486">Boolean</span></span>|<span data-ttu-id="c6931-487">指示在展台模式下是否要求缩放。</span><span class="sxs-lookup"><span data-stu-id="c6931-487">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="c6931-488">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="c6931-488">kioskModeManagedAppId</span></span>|<span data-ttu-id="c6931-489">String</span><span class="sxs-lookup"><span data-stu-id="c6931-489">String</span></span>|<span data-ttu-id="c6931-490">用于展台模式的应用的托管应用 ID。</span><span class="sxs-lookup"><span data-stu-id="c6931-490">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="c6931-491">如果指定了 KioskModeManagedAppId，则将忽略 KioskModeAppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="c6931-491">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="c6931-492">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="c6931-492">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="c6931-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-493">Boolean</span></span>|<span data-ttu-id="c6931-494">指示是否阻止用户在锁定屏幕上使用控制中心。</span><span class="sxs-lookup"><span data-stu-id="c6931-494">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="c6931-495">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="c6931-495">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="c6931-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-496">Boolean</span></span>|<span data-ttu-id="c6931-497">指示是否阻止用户在锁定屏幕上使用通知视图。</span><span class="sxs-lookup"><span data-stu-id="c6931-497">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="c6931-498">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="c6931-498">lockScreenBlockPassbook</span></span>|<span data-ttu-id="c6931-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-499">Boolean</span></span>|<span data-ttu-id="c6931-500">指示设备处于锁定状态时是否阻止用户使用 Passbook。</span><span class="sxs-lookup"><span data-stu-id="c6931-500">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="c6931-501">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="c6931-501">lockScreenBlockTodayView</span></span>|<span data-ttu-id="c6931-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-502">Boolean</span></span>|<span data-ttu-id="c6931-503">指示是否阻止用户在锁定屏幕上使用今日视图。</span><span class="sxs-lookup"><span data-stu-id="c6931-503">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="c6931-504">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c6931-504">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="c6931-505">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c6931-505">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="c6931-506">澳大利亚的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-506">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="c6931-507">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="c6931-507">mediaContentRatingCanada</span></span>|[<span data-ttu-id="c6931-508">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="c6931-508">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="c6931-509">加拿大的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-509">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="c6931-510">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="c6931-510">mediaContentRatingFrance</span></span>|[<span data-ttu-id="c6931-511">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="c6931-511">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="c6931-512">法国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-512">Media content rating settings for France</span></span>|
|<span data-ttu-id="c6931-513">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c6931-513">mediaContentRatingGermany</span></span>|[<span data-ttu-id="c6931-514">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c6931-514">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="c6931-515">德国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-515">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="c6931-516">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="c6931-516">mediaContentRatingIreland</span></span>|[<span data-ttu-id="c6931-517">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="c6931-517">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="c6931-518">爱尔兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-518">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="c6931-519">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="c6931-519">mediaContentRatingJapan</span></span>|[<span data-ttu-id="c6931-520">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="c6931-520">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="c6931-521">日本的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-521">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="c6931-522">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="c6931-522">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="c6931-523">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="c6931-523">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="c6931-524">新西兰的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-524">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="c6931-525">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="c6931-525">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="c6931-526">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="c6931-526">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="c6931-527">英国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-527">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="c6931-528">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="c6931-528">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="c6931-529">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="c6931-529">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="c6931-530">美国的媒体内容评级设置</span><span class="sxs-lookup"><span data-stu-id="c6931-530">Media content rating settings for United States</span></span>|
|<span data-ttu-id="c6931-531">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="c6931-531">networkUsageRules</span></span>|<span data-ttu-id="c6931-532">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6931-532">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="c6931-533">托管应用列表以及适用于它们的网络规则。</span><span class="sxs-lookup"><span data-stu-id="c6931-533">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="c6931-534">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c6931-534">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c6931-535">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="c6931-535">mediaContentRatingApps</span></span>|[<span data-ttu-id="c6931-536">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="c6931-536">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="c6931-537">应用的媒体内容评级设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-537">Media content rating settings for Apps.</span></span> <span data-ttu-id="c6931-538">可取值为：`allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="c6931-538">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="c6931-539">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-539">messagesBlocked</span></span>|<span data-ttu-id="c6931-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-540">Boolean</span></span>|<span data-ttu-id="c6931-541">指示是否阻止用户使用受监督设备上的消息应用。</span><span class="sxs-lookup"><span data-stu-id="c6931-541">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="c6931-542">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="c6931-542">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="c6931-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-543">Boolean</span></span>|<span data-ttu-id="c6931-544">指示是否允许修改通知设置（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-544">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c6931-545">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c6931-545">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="c6931-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-546">Boolean</span></span>|<span data-ttu-id="c6931-547">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="c6931-547">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c6931-548">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="c6931-548">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="c6931-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-549">Boolean</span></span>|<span data-ttu-id="c6931-550">在监督模式下阻止修改已注册的 Touch ID 指纹。</span><span class="sxs-lookup"><span data-stu-id="c6931-550">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="c6931-551">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="c6931-551">passcodeBlockModification</span></span>|<span data-ttu-id="c6931-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-552">Boolean</span></span>|<span data-ttu-id="c6931-553">指示是否允许在受监督的设备中修改密码（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-553">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="c6931-554">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c6931-554">passcodeBlockSimple</span></span>|<span data-ttu-id="c6931-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-555">Boolean</span></span>|<span data-ttu-id="c6931-556">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="c6931-556">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="c6931-557">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c6931-557">passcodeExpirationDays</span></span>|<span data-ttu-id="c6931-558">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-558">Int32</span></span>|<span data-ttu-id="c6931-559">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c6931-559">Number of days before the passcode expires.</span></span> <span data-ttu-id="c6931-560">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="c6931-560">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c6931-561">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c6931-561">passcodeMinimumLength</span></span>|<span data-ttu-id="c6931-562">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-562">Int32</span></span>|<span data-ttu-id="c6931-563">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c6931-563">Minimum length of passcode.</span></span> <span data-ttu-id="c6931-564">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="c6931-564">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c6931-565">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c6931-565">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c6931-566">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-566">Int32</span></span>|<span data-ttu-id="c6931-567">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="c6931-567">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="c6931-568">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c6931-568">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c6931-569">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-569">Int32</span></span>|<span data-ttu-id="c6931-570">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="c6931-570">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c6931-571">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c6931-571">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="c6931-572">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-572">Int32</span></span>|<span data-ttu-id="c6931-573">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c6931-573">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="c6931-574">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="c6931-574">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c6931-575">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="c6931-575">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="c6931-576">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-576">Int32</span></span>|<span data-ttu-id="c6931-577">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c6931-577">Number of previous passcodes to block.</span></span> <span data-ttu-id="c6931-578">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="c6931-578">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c6931-579">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="c6931-579">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="c6931-580">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-580">Int32</span></span>|<span data-ttu-id="c6931-581">擦除设备前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="c6931-581">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="c6931-582">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="c6931-582">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c6931-583">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="c6931-583">passcodeRequiredType</span></span>|[<span data-ttu-id="c6931-584">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c6931-584">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c6931-585">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c6931-585">Type of passcode that is required.</span></span> <span data-ttu-id="c6931-586">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c6931-586">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c6931-587">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="c6931-587">passcodeRequired</span></span>|<span data-ttu-id="c6931-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-588">Boolean</span></span>|<span data-ttu-id="c6931-589">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c6931-589">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="c6931-590">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-590">podcastsBlocked</span></span>|<span data-ttu-id="c6931-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-591">Boolean</span></span>|<span data-ttu-id="c6931-592">指示在受监督的设备上是否阻止用户使用播客（iOS 8.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-592">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="c6931-593">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="c6931-593">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="c6931-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-594">Boolean</span></span>|<span data-ttu-id="c6931-595">指示是否启用提示以在受监督的设备上安装附近设备。</span><span class="sxs-lookup"><span data-stu-id="c6931-595">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="c6931-596">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c6931-596">safariBlockAutofill</span></span>|<span data-ttu-id="c6931-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-597">Boolean</span></span>|<span data-ttu-id="c6931-598">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="c6931-598">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="c6931-599">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-599">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-600">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c6931-600">safariBlockJavaScript</span></span>|<span data-ttu-id="c6931-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-601">Boolean</span></span>|<span data-ttu-id="c6931-602">指示在 Safari 中是否阻止 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="c6931-602">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="c6931-603">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c6931-603">safariBlockPopups</span></span>|<span data-ttu-id="c6931-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-604">Boolean</span></span>|<span data-ttu-id="c6931-605">指示在 Safari 中是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="c6931-605">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="c6931-606">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-606">safariBlocked</span></span>|<span data-ttu-id="c6931-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-607">Boolean</span></span>|<span data-ttu-id="c6931-608">指示是否阻止用户使用 Safari。</span><span class="sxs-lookup"><span data-stu-id="c6931-608">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="c6931-609">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-609">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-610">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-610">safariCookieSettings</span></span>|[<span data-ttu-id="c6931-611">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c6931-611">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="c6931-612">Safari 的 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="c6931-612">Cookie settings for Safari.</span></span> <span data-ttu-id="c6931-613">可取值为：`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways`。</span><span class="sxs-lookup"><span data-stu-id="c6931-613">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="c6931-614">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="c6931-614">safariManagedDomains</span></span>|<span data-ttu-id="c6931-615">String collection</span><span class="sxs-lookup"><span data-stu-id="c6931-615">String collection</span></span>|<span data-ttu-id="c6931-616">与此处列出的模式匹配的 URL 将被视为托管。</span><span class="sxs-lookup"><span data-stu-id="c6931-616">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="c6931-617">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="c6931-617">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="c6931-618">String 集合</span><span class="sxs-lookup"><span data-stu-id="c6931-618">String collection</span></span>|<span data-ttu-id="c6931-619">用户只能通过匹配此处列出的模式的 URL 将密码保存在 Safari 中。</span><span class="sxs-lookup"><span data-stu-id="c6931-619">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="c6931-620">适用于处于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-620">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="c6931-621">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="c6931-621">safariRequireFraudWarning</span></span>|<span data-ttu-id="c6931-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-622">Boolean</span></span>|<span data-ttu-id="c6931-623">指示在 Safari 中是否需要诈骗警告。</span><span class="sxs-lookup"><span data-stu-id="c6931-623">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="c6931-624">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-624">screenCaptureBlocked</span></span>|<span data-ttu-id="c6931-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-625">Boolean</span></span>|<span data-ttu-id="c6931-626">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="c6931-626">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="c6931-627">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-627">siriBlocked</span></span>|<span data-ttu-id="c6931-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-628">Boolean</span></span>|<span data-ttu-id="c6931-629">指示是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="c6931-629">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="c6931-630">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="c6931-630">siriBlockedWhenLocked</span></span>|<span data-ttu-id="c6931-631">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-631">Boolean</span></span>|<span data-ttu-id="c6931-632">指示锁定时是否阻止用户使用 Siri。</span><span class="sxs-lookup"><span data-stu-id="c6931-632">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="c6931-633">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="c6931-633">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="c6931-634">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-634">Boolean</span></span>|<span data-ttu-id="c6931-635">指示在受监督的设备上使用时是否阻止 Siri 查询用户生成的内容。</span><span class="sxs-lookup"><span data-stu-id="c6931-635">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="c6931-636">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="c6931-636">siriRequireProfanityFilter</span></span>|<span data-ttu-id="c6931-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-637">Boolean</span></span>|<span data-ttu-id="c6931-638">指示是否阻止 Siri 在受监督的设备上口述或说出亵渎语言。</span><span class="sxs-lookup"><span data-stu-id="c6931-638">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="c6931-639">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="c6931-639">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="c6931-640">Int32</span><span class="sxs-lookup"><span data-stu-id="c6931-640">Int32</span></span>|<span data-ttu-id="c6931-641">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="c6931-641">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="c6931-642">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="c6931-642">Valid values 0 to 90</span></span>|
|<span data-ttu-id="c6931-643">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="c6931-643">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="c6931-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-644">Boolean</span></span>|<span data-ttu-id="c6931-645">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="c6931-645">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-646">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="c6931-646">spotlightBlockInternetResults</span></span>|<span data-ttu-id="c6931-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-647">Boolean</span></span>|<span data-ttu-id="c6931-648">指示是否阻止 Spotlight 搜索在受监督的设备上返回 Internet 搜索结果。</span><span class="sxs-lookup"><span data-stu-id="c6931-648">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="c6931-649">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-649">voiceDialingBlocked</span></span>|<span data-ttu-id="c6931-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-650">Boolean</span></span>|<span data-ttu-id="c6931-651">指示是否阻止语音拨号。</span><span class="sxs-lookup"><span data-stu-id="c6931-651">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="c6931-652">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="c6931-652">wallpaperBlockModification</span></span>|<span data-ttu-id="c6931-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-653">Boolean</span></span>|<span data-ttu-id="c6931-654">指示是否允许在受监督的设备上修改墙纸（iOS 9.0 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c6931-654">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="c6931-655">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="c6931-655">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="c6931-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-656">Boolean</span></span>|<span data-ttu-id="c6931-657">指示设备处于监督模式时是否强制设备仅使用配置文件中的 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="c6931-657">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c6931-658">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="c6931-658">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="c6931-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-659">Boolean</span></span>|<span data-ttu-id="c6931-660">指示在非托管课程中通过教室注册的学生是否会在尝试离开该课程 (iOS 11.3 及更高版本) 时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="c6931-660">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="c6931-661">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="c6931-661">keychainBlockCloudSync</span></span>|<span data-ttu-id="c6931-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-662">Boolean</span></span>|<span data-ttu-id="c6931-663">指示是否阻止 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="c6931-663">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="c6931-664">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-664">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="c6931-665">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="c6931-665">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="c6931-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-666">Boolean</span></span>|<span data-ttu-id="c6931-667">指示是否阻止无线 PKI 更新。</span><span class="sxs-lookup"><span data-stu-id="c6931-667">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="c6931-668">将此限制设置为 false 不会禁用 CRL 和 OCSP 检查 (iOS 7.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-668">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="c6931-669">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="c6931-669">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="c6931-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-670">Boolean</span></span>|<span data-ttu-id="c6931-671">指示广告跟踪是否受限制。(iOS 7.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-671">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="c6931-672">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="c6931-672">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="c6931-673">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-673">Boolean</span></span>|<span data-ttu-id="c6931-674">指示是否阻止企业书籍备份。</span><span class="sxs-lookup"><span data-stu-id="c6931-674">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="c6931-675">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="c6931-675">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="c6931-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-676">Boolean</span></span>|<span data-ttu-id="c6931-677">指示是否阻止企业书籍笔记和突出显示同步。</span><span class="sxs-lookup"><span data-stu-id="c6931-677">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="c6931-678">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-678">airPrintBlocked</span></span>|<span data-ttu-id="c6931-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-679">Boolean</span></span>|<span data-ttu-id="c6931-680">指示是否阻止 AirPrint (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-680">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="c6931-681">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="c6931-681">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="c6931-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-682">Boolean</span></span>|<span data-ttu-id="c6931-683">指示是否阻止 Airprint 的用户名和密码的密钥链存储 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-683">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="c6931-684">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="c6931-684">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="c6931-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-685">Boolean</span></span>|<span data-ttu-id="c6931-686">指示 TLS 打印通信是否需要受信任的证书 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-686">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="c6931-687">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="c6931-687">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="c6931-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-688">Boolean</span></span>|<span data-ttu-id="c6931-689">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="c6931-689">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="c6931-690">这样可以防止虚假的 AirPrint 蓝牙信号免受网络流量 (iOS 11.0 及更高版本) 的欺骗。</span><span class="sxs-lookup"><span data-stu-id="c6931-690">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="c6931-691">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="c6931-691">blockSystemAppRemoval</span></span>|<span data-ttu-id="c6931-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-692">Boolean</span></span>|<span data-ttu-id="c6931-693">指示是否在受监督的设备 (iOS 11.0 及更高版本) 上阻止从设备中删除系统应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6931-693">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="c6931-694">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="c6931-694">vpnBlockCreation</span></span>|<span data-ttu-id="c6931-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-695">Boolean</span></span>|<span data-ttu-id="c6931-696">指示是否阻止创建 VPN 配置 (iOS 11.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-696">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="c6931-697">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-697">appRemovalBlocked</span></span>|<span data-ttu-id="c6931-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-698">Boolean</span></span>|<span data-ttu-id="c6931-699">指示是否允许删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6931-699">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="c6931-700">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-700">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="c6931-701">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-701">Boolean</span></span>|<span data-ttu-id="c6931-702">指示是否允许在锁定设备时连接到 USB 附件 (iOS 11.4.1 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-702">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="c6931-703">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="c6931-703">passwordBlockAutoFill</span></span>|<span data-ttu-id="c6931-704">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-704">Boolean</span></span>|<span data-ttu-id="c6931-705">指示是否允许自动填充密码功能 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-705">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="c6931-706">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="c6931-706">passwordBlockProximityRequests</span></span>|<span data-ttu-id="c6931-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-707">Boolean</span></span>|<span data-ttu-id="c6931-708">指示是否阻止来自附近设备 (iOS 12.0 及更高版本) 发出请求的密码。</span><span class="sxs-lookup"><span data-stu-id="c6931-708">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="c6931-709">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="c6931-709">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="c6931-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-710">Boolean</span></span>|<span data-ttu-id="c6931-711">指示是否阻止使用 AirDrop 密码的共享密码功能 iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-711">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="c6931-712">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="c6931-712">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="c6931-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-713">Boolean</span></span>|<span data-ttu-id="c6931-714">指示是否启用日期和时间 "设置自动设置" 功能, 以及用户是否无法关闭该功能 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-714">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="c6931-715">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="c6931-715">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="c6931-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-716">Boolean</span></span>|<span data-ttu-id="c6931-717">指示托管应用程序是否可以将联系人写入非托管联系人帐户 (iOS 12.0 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-717">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="c6931-718">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="c6931-718">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="c6931-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-719">Boolean</span></span>|<span data-ttu-id="c6931-720">指示非托管应用是否可以从托管联系人帐户读取 (iOS 12.0 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-720">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="c6931-721">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="c6931-721">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="c6931-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-722">Boolean</span></span>|<span data-ttu-id="c6931-723">指示是否阻止用户修改个人热点设置 (iOS 12.2 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-723">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="c6931-724">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="c6931-724">siriDisableServerLogging</span></span>|<span data-ttu-id="c6931-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-725">Boolean</span></span>|<span data-ttu-id="c6931-726">指示是否禁用服务器端 Siri 日志记录 (iOS 12.2 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-726">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="c6931-727">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-727">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="c6931-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-728">Boolean</span></span>|<span data-ttu-id="c6931-729">指示设备受到监督时是否阻止连续路径键盘 (iOS 13 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-729">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="c6931-730">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-730">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="c6931-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-731">Boolean</span></span>|<span data-ttu-id="c6931-732">指示设备受到监督时是否阻止查找我的设备 (iOS 13 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-732">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="c6931-733">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-733">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="c6931-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-734">Boolean</span></span>|<span data-ttu-id="c6931-735">指示设备受到监督时是否阻止查找我的好友 (iOS 13 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-735">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="c6931-736">wiFiBlockPowerModification</span><span class="sxs-lookup"><span data-stu-id="c6931-736">wiFiBlockPowerModification</span></span>|<span data-ttu-id="c6931-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-737">Boolean</span></span>|<span data-ttu-id="c6931-738">指示设备受到监督时是否阻止 WiFi 电源修改 (iOS 13 或更高版本)。</span><span class="sxs-lookup"><span data-stu-id="c6931-738">Indicates whether or not to block WiFi power modification when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="c6931-739">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="c6931-739">iTunesBlocked</span></span>|<span data-ttu-id="c6931-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6931-740">Boolean</span></span>|<span data-ttu-id="c6931-741">指示是否阻止 iTunes 应用。</span><span class="sxs-lookup"><span data-stu-id="c6931-741">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="c6931-742">需要受监督设备的 iOS 13 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c6931-742">Requires a supervised device for iOS 13 and later.</span></span>|



## <a name="response"></a><span data-ttu-id="c6931-743">响应</span><span class="sxs-lookup"><span data-stu-id="c6931-743">Response</span></span>
<span data-ttu-id="c6931-744">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6931-744">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6931-745">示例</span><span class="sxs-lookup"><span data-stu-id="c6931-745">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6931-746">请求</span><span class="sxs-lookup"><span data-stu-id="c6931-746">Request</span></span>
<span data-ttu-id="c6931-747">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6931-747">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10353

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
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "wiFiBlockPowerModification": true,
  "iTunesBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="c6931-748">响应</span><span class="sxs-lookup"><span data-stu-id="c6931-748">Response</span></span>
<span data-ttu-id="c6931-p153">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6931-p153">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10525

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
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "wiFiBlockPowerModification": true,
  "iTunesBlocked": true
}
```






