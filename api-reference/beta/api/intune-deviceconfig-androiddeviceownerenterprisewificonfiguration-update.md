---
title: 更新 androidDeviceOwnerEnterpriseWiFiConfiguration
description: 更新 androidDeviceOwnerEnterpriseWiFiConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 443ef78b5dbc786399cbc1b92e0e18c8d7c9f0e4
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955061"
---
# <a name="update-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="b5087-103">更新 androidDeviceOwnerEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5087-103">Update androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="b5087-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5087-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5087-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5087-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5087-106">更新[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5087-106">Update the properties of a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5087-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5087-107">Prerequisites</span></span>
<span data-ttu-id="b5087-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5087-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5087-110">Permission type</span></span>|<span data-ttu-id="b5087-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5087-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5087-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5087-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5087-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5087-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5087-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5087-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5087-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5087-115">Not supported.</span></span>|
|<span data-ttu-id="b5087-116">Application</span><span class="sxs-lookup"><span data-stu-id="b5087-116">Application</span></span>|<span data-ttu-id="b5087-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5087-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5087-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5087-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5087-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5087-119">Request headers</span></span>
|<span data-ttu-id="b5087-120">标头</span><span class="sxs-lookup"><span data-stu-id="b5087-120">Header</span></span>|<span data-ttu-id="b5087-121">值</span><span class="sxs-lookup"><span data-stu-id="b5087-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5087-122">授权</span><span class="sxs-lookup"><span data-stu-id="b5087-122">Authorization</span></span>|<span data-ttu-id="b5087-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5087-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5087-124">接受</span><span class="sxs-lookup"><span data-stu-id="b5087-124">Accept</span></span>|<span data-ttu-id="b5087-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5087-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5087-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5087-126">Request body</span></span>
<span data-ttu-id="b5087-127">在请求正文中，提供[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5087-127">In the request body, supply a JSON representation for the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="b5087-128">下表显示创建[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5087-128">The following table shows the properties that are required when you create the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="b5087-129">属性</span><span class="sxs-lookup"><span data-stu-id="b5087-129">Property</span></span>|<span data-ttu-id="b5087-130">类型</span><span class="sxs-lookup"><span data-stu-id="b5087-130">Type</span></span>|<span data-ttu-id="b5087-131">说明</span><span class="sxs-lookup"><span data-stu-id="b5087-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5087-132">id</span><span class="sxs-lookup"><span data-stu-id="b5087-132">id</span></span>|<span data-ttu-id="b5087-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b5087-133">String</span></span>|<span data-ttu-id="b5087-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5087-134">Key of the entity.</span></span> <span data-ttu-id="b5087-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5087-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b5087-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5087-137">DateTimeOffset</span></span>|<span data-ttu-id="b5087-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b5087-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b5087-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5087-140">roleScopeTagIds</span></span>|<span data-ttu-id="b5087-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b5087-141">String collection</span></span>|<span data-ttu-id="b5087-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b5087-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5087-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b5087-144">supportsScopeTags</span></span>|<span data-ttu-id="b5087-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5087-145">Boolean</span></span>|<span data-ttu-id="b5087-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b5087-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5087-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b5087-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5087-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b5087-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5087-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b5087-149">This property is read-only.</span></span> <span data-ttu-id="b5087-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5087-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5087-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5087-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5087-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b5087-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5087-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5087-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5087-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5087-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5087-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b5087-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5087-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5087-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5087-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5087-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5087-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b5087-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5087-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5087-163">createdDateTime</span></span>|<span data-ttu-id="b5087-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5087-164">DateTimeOffset</span></span>|<span data-ttu-id="b5087-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b5087-165">DateTime the object was created.</span></span> <span data-ttu-id="b5087-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-167">说明</span><span class="sxs-lookup"><span data-stu-id="b5087-167">description</span></span>|<span data-ttu-id="b5087-168">String</span><span class="sxs-lookup"><span data-stu-id="b5087-168">String</span></span>|<span data-ttu-id="b5087-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b5087-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5087-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b5087-171">displayName</span></span>|<span data-ttu-id="b5087-172">String</span><span class="sxs-lookup"><span data-stu-id="b5087-172">String</span></span>|<span data-ttu-id="b5087-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b5087-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5087-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-175">version</span><span class="sxs-lookup"><span data-stu-id="b5087-175">version</span></span>|<span data-ttu-id="b5087-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b5087-176">Int32</span></span>|<span data-ttu-id="b5087-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b5087-177">Version of the device configuration.</span></span> <span data-ttu-id="b5087-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5087-179">networkName</span><span class="sxs-lookup"><span data-stu-id="b5087-179">networkName</span></span>|<span data-ttu-id="b5087-180">字符串</span><span class="sxs-lookup"><span data-stu-id="b5087-180">String</span></span>|<span data-ttu-id="b5087-181">从[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="b5087-181">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="b5087-182">ssid</span><span class="sxs-lookup"><span data-stu-id="b5087-182">ssid</span></span>|<span data-ttu-id="b5087-183">字符串</span><span class="sxs-lookup"><span data-stu-id="b5087-183">String</span></span>|<span data-ttu-id="b5087-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="b5087-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="b5087-185">继承自[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-185">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="b5087-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b5087-186">connectAutomatically</span></span>|<span data-ttu-id="b5087-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5087-187">Boolean</span></span>|<span data-ttu-id="b5087-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="b5087-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b5087-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="b5087-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="b5087-190">继承自[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-190">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="b5087-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b5087-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b5087-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5087-192">Boolean</span></span>|<span data-ttu-id="b5087-193">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="b5087-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="b5087-194">继承自[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-194">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="b5087-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b5087-195">wiFiSecurityType</span></span>|[<span data-ttu-id="b5087-196">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b5087-196">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="b5087-197">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="b5087-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b5087-198">继承自[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b5087-198">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="b5087-199">可取值为：`open`、`wep`、`wpaPersonal`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="b5087-199">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="b5087-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b5087-200">preSharedKey</span></span>|<span data-ttu-id="b5087-201">字符串</span><span class="sxs-lookup"><span data-stu-id="b5087-201">String</span></span>|<span data-ttu-id="b5087-202">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="b5087-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="b5087-203">继承自[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-203">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="b5087-204">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="b5087-204">preSharedKeyIsSet</span></span>|<span data-ttu-id="b5087-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5087-205">Boolean</span></span>|<span data-ttu-id="b5087-206">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="b5087-206">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="b5087-207">继承自[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5087-207">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="b5087-208">eapType</span><span class="sxs-lookup"><span data-stu-id="b5087-208">eapType</span></span>|[<span data-ttu-id="b5087-209">androidEapType</span><span class="sxs-lookup"><span data-stu-id="b5087-209">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="b5087-210">指示 Wi-fi 终结点（路由器）上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="b5087-210">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="b5087-211">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="b5087-211">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="b5087-212">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b5087-212">authenticationMethod</span></span>|[<span data-ttu-id="b5087-213">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b5087-213">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="b5087-214">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时，客户端（设备）需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b5087-214">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="b5087-215">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="b5087-215">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b5087-216">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="b5087-216">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="b5087-217">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="b5087-217">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="b5087-218">EAP 类型为 EAP 时，用于身份验证的非 EAP 方法（内部标识）-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="b5087-218">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="b5087-219">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="b5087-219">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b5087-220">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="b5087-220">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="b5087-221">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="b5087-221">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="b5087-222">当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法（内部标识）。</span><span class="sxs-lookup"><span data-stu-id="b5087-222">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="b5087-223">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="b5087-223">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b5087-224">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="b5087-224">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="b5087-225">字符串</span><span class="sxs-lookup"><span data-stu-id="b5087-225">String</span></span>|<span data-ttu-id="b5087-226">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时启用标识隐私（外部标识）。</span><span class="sxs-lookup"><span data-stu-id="b5087-226">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="b5087-227">此处提供的字符串用于在用户尝试连接到 Wlan 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="b5087-227">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="b5087-228">响应</span><span class="sxs-lookup"><span data-stu-id="b5087-228">Response</span></span>
<span data-ttu-id="b5087-229">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5087-229">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5087-230">示例</span><span class="sxs-lookup"><span data-stu-id="b5087-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5087-231">请求</span><span class="sxs-lookup"><span data-stu-id="b5087-231">Request</span></span>
<span data-ttu-id="b5087-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5087-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1612

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="b5087-233">响应</span><span class="sxs-lookup"><span data-stu-id="b5087-233">Response</span></span>
<span data-ttu-id="b5087-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5087-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1784

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
  "id": "7ef0d9c3-d9c3-7ef0-c3d9-f07ec3d9f07e",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





