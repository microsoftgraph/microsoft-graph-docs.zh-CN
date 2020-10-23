---
title: 更新 androidDeviceOwnerEnterpriseWiFiConfiguration
description: 更新 androidDeviceOwnerEnterpriseWiFiConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a9ed0fa822def5f9edea00009e84b904f959be5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685280"
---
# <a name="update-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="27539-103">更新 androidDeviceOwnerEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="27539-103">Update androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="27539-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27539-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27539-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27539-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27539-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27539-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27539-107">更新 [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27539-107">Update the properties of a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27539-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27539-108">Prerequisites</span></span>
<span data-ttu-id="27539-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27539-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27539-111">Permission type</span></span>|<span data-ttu-id="27539-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27539-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27539-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27539-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27539-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27539-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27539-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27539-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27539-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27539-116">Not supported.</span></span>|
|<span data-ttu-id="27539-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="27539-117">Application</span></span>|<span data-ttu-id="27539-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27539-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27539-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27539-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="27539-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27539-120">Request headers</span></span>
|<span data-ttu-id="27539-121">标头</span><span class="sxs-lookup"><span data-stu-id="27539-121">Header</span></span>|<span data-ttu-id="27539-122">值</span><span class="sxs-lookup"><span data-stu-id="27539-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27539-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27539-123">Authorization</span></span>|<span data-ttu-id="27539-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27539-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27539-125">接受</span><span class="sxs-lookup"><span data-stu-id="27539-125">Accept</span></span>|<span data-ttu-id="27539-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27539-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27539-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27539-127">Request body</span></span>
<span data-ttu-id="27539-128">在请求正文中，提供 [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27539-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="27539-129">下表显示创建 [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27539-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="27539-130">属性</span><span class="sxs-lookup"><span data-stu-id="27539-130">Property</span></span>|<span data-ttu-id="27539-131">类型</span><span class="sxs-lookup"><span data-stu-id="27539-131">Type</span></span>|<span data-ttu-id="27539-132">说明</span><span class="sxs-lookup"><span data-stu-id="27539-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27539-133">id</span><span class="sxs-lookup"><span data-stu-id="27539-133">id</span></span>|<span data-ttu-id="27539-134">String</span><span class="sxs-lookup"><span data-stu-id="27539-134">String</span></span>|<span data-ttu-id="27539-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27539-135">Key of the entity.</span></span> <span data-ttu-id="27539-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27539-137">lastModifiedDateTime</span></span>|<span data-ttu-id="27539-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27539-138">DateTimeOffset</span></span>|<span data-ttu-id="27539-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27539-139">DateTime the object was last modified.</span></span> <span data-ttu-id="27539-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27539-141">roleScopeTagIds</span></span>|<span data-ttu-id="27539-142">String collection</span><span class="sxs-lookup"><span data-stu-id="27539-142">String collection</span></span>|<span data-ttu-id="27539-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="27539-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="27539-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="27539-145">supportsScopeTags</span></span>|<span data-ttu-id="27539-146">布尔</span><span class="sxs-lookup"><span data-stu-id="27539-146">Boolean</span></span>|<span data-ttu-id="27539-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="27539-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="27539-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="27539-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="27539-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="27539-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="27539-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="27539-150">This property is read-only.</span></span> <span data-ttu-id="27539-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="27539-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="27539-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="27539-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="27539-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="27539-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="27539-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="27539-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="27539-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="27539-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="27539-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="27539-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="27539-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="27539-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="27539-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="27539-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="27539-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="27539-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="27539-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27539-164">createdDateTime</span></span>|<span data-ttu-id="27539-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27539-165">DateTimeOffset</span></span>|<span data-ttu-id="27539-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27539-166">DateTime the object was created.</span></span> <span data-ttu-id="27539-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-168">说明</span><span class="sxs-lookup"><span data-stu-id="27539-168">description</span></span>|<span data-ttu-id="27539-169">String</span><span class="sxs-lookup"><span data-stu-id="27539-169">String</span></span>|<span data-ttu-id="27539-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="27539-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27539-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-172">displayName</span><span class="sxs-lookup"><span data-stu-id="27539-172">displayName</span></span>|<span data-ttu-id="27539-173">String</span><span class="sxs-lookup"><span data-stu-id="27539-173">String</span></span>|<span data-ttu-id="27539-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="27539-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27539-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-176">version</span><span class="sxs-lookup"><span data-stu-id="27539-176">version</span></span>|<span data-ttu-id="27539-177">Int32</span><span class="sxs-lookup"><span data-stu-id="27539-177">Int32</span></span>|<span data-ttu-id="27539-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="27539-178">Version of the device configuration.</span></span> <span data-ttu-id="27539-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27539-180">networkName</span><span class="sxs-lookup"><span data-stu-id="27539-180">networkName</span></span>|<span data-ttu-id="27539-181">String</span><span class="sxs-lookup"><span data-stu-id="27539-181">String</span></span>|<span data-ttu-id="27539-182">从[AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="27539-182">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="27539-183">ssid</span><span class="sxs-lookup"><span data-stu-id="27539-183">ssid</span></span>|<span data-ttu-id="27539-184">String</span><span class="sxs-lookup"><span data-stu-id="27539-184">String</span></span>|<span data-ttu-id="27539-185">这是广播到所有设备的 Wi-Fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="27539-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="27539-186">继承自 [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-186">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="27539-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="27539-187">connectAutomatically</span></span>|<span data-ttu-id="27539-188">布尔</span><span class="sxs-lookup"><span data-stu-id="27539-188">Boolean</span></span>|<span data-ttu-id="27539-189">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="27539-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="27539-190">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="27539-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="27539-191">继承自 [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-191">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="27539-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="27539-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="27539-193">布尔</span><span class="sxs-lookup"><span data-stu-id="27539-193">Boolean</span></span>|<span data-ttu-id="27539-194">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="27539-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="27539-195">继承自 [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-195">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="27539-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="27539-196">wiFiSecurityType</span></span>|[<span data-ttu-id="27539-197">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="27539-197">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="27539-198">指示 Wi-Fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="27539-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="27539-199">继承自 [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="27539-199">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="27539-200">可取值为：`open`、`wep`、`wpaPersonal`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="27539-200">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="27539-201">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="27539-201">preSharedKey</span></span>|<span data-ttu-id="27539-202">String</span><span class="sxs-lookup"><span data-stu-id="27539-202">String</span></span>|<span data-ttu-id="27539-203">这是 WPA 个人 Wi-Fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="27539-203">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="27539-204">继承自 [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-204">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="27539-205">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="27539-205">preSharedKeyIsSet</span></span>|<span data-ttu-id="27539-206">布尔</span><span class="sxs-lookup"><span data-stu-id="27539-206">Boolean</span></span>|<span data-ttu-id="27539-207">这是 WPA 个人 Wi-Fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="27539-207">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="27539-208">继承自 [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27539-208">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="27539-209">eapType</span><span class="sxs-lookup"><span data-stu-id="27539-209">eapType</span></span>|[<span data-ttu-id="27539-210">androidEapType</span><span class="sxs-lookup"><span data-stu-id="27539-210">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="27539-211">指示 Wi-Fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="27539-211">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="27539-212">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="27539-212">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="27539-213">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="27539-213">authenticationMethod</span></span>|[<span data-ttu-id="27539-214">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="27539-214">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="27539-215">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时，客户端 (设备) 需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="27539-215">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="27539-216">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="27539-216">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="27539-217">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="27539-217">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="27539-218">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="27539-218">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="27539-219">在 EAP 类型为 EAP 时，用于身份验证的非 EAP 方法 (内部标识) （eap 类型为 EAP-TTLS，Authenticationmethod 为用户名和密码）。</span><span class="sxs-lookup"><span data-stu-id="27539-219">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="27539-220">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="27539-220">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="27539-221">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="27539-221">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="27539-222">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="27539-222">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="27539-223">在 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，身份验证 (内部标识) 的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="27539-223">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="27539-224">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="27539-224">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="27539-225">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="27539-225">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="27539-226">String</span><span class="sxs-lookup"><span data-stu-id="27539-226">String</span></span>|<span data-ttu-id="27539-227">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时，请启用标识隐私 (外部标识) 。</span><span class="sxs-lookup"><span data-stu-id="27539-227">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="27539-228">此处提供的字符串用于在用户尝试连接到 Wi-Fi 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="27539-228">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="27539-229">响应</span><span class="sxs-lookup"><span data-stu-id="27539-229">Response</span></span>
<span data-ttu-id="27539-230">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27539-230">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27539-231">示例</span><span class="sxs-lookup"><span data-stu-id="27539-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="27539-232">请求</span><span class="sxs-lookup"><span data-stu-id="27539-232">Request</span></span>
<span data-ttu-id="27539-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27539-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27539-234">响应</span><span class="sxs-lookup"><span data-stu-id="27539-234">Response</span></span>
<span data-ttu-id="27539-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27539-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





