---
title: 更新 androidWorkProfileEnterpriseWiFiConfiguration
description: 更新 androidWorkProfileEnterpriseWiFiConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6402afbf5899337536db8a6239c1ed3e730ebc1a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758493"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="8f947-103">更新 androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f947-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="8f947-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f947-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f947-106">更新[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8f947-106">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f947-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f947-107">Prerequisites</span></span>
<span data-ttu-id="8f947-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f947-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f947-110">Permission type</span></span>|<span data-ttu-id="8f947-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f947-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f947-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f947-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f947-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f947-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f947-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f947-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f947-115">Not supported.</span></span>|
|<span data-ttu-id="8f947-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f947-116">Application</span></span>|<span data-ttu-id="8f947-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f947-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f947-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f947-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8f947-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f947-119">Request headers</span></span>
|<span data-ttu-id="8f947-120">标头</span><span class="sxs-lookup"><span data-stu-id="8f947-120">Header</span></span>|<span data-ttu-id="8f947-121">值</span><span class="sxs-lookup"><span data-stu-id="8f947-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f947-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f947-122">Authorization</span></span>|<span data-ttu-id="8f947-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f947-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f947-124">接受</span><span class="sxs-lookup"><span data-stu-id="8f947-124">Accept</span></span>|<span data-ttu-id="8f947-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f947-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f947-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f947-126">Request body</span></span>
<span data-ttu-id="8f947-127">在请求正文中，提供[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f947-127">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="8f947-128">下表显示创建[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8f947-128">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="8f947-129">属性</span><span class="sxs-lookup"><span data-stu-id="8f947-129">Property</span></span>|<span data-ttu-id="8f947-130">类型</span><span class="sxs-lookup"><span data-stu-id="8f947-130">Type</span></span>|<span data-ttu-id="8f947-131">说明</span><span class="sxs-lookup"><span data-stu-id="8f947-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f947-132">id</span><span class="sxs-lookup"><span data-stu-id="8f947-132">id</span></span>|<span data-ttu-id="8f947-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8f947-133">String</span></span>|<span data-ttu-id="8f947-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8f947-134">Key of the entity.</span></span> <span data-ttu-id="8f947-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f947-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8f947-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f947-137">DateTimeOffset</span></span>|<span data-ttu-id="8f947-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8f947-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8f947-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f947-140">roleScopeTagIds</span></span>|<span data-ttu-id="8f947-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8f947-141">String collection</span></span>|<span data-ttu-id="8f947-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8f947-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8f947-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8f947-144">supportsScopeTags</span></span>|<span data-ttu-id="8f947-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f947-145">Boolean</span></span>|<span data-ttu-id="8f947-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8f947-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8f947-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8f947-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8f947-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8f947-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8f947-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8f947-149">This property is read-only.</span></span> <span data-ttu-id="8f947-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8f947-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8f947-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8f947-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8f947-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8f947-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8f947-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8f947-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8f947-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8f947-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8f947-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8f947-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8f947-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8f947-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8f947-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8f947-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8f947-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8f947-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8f947-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f947-163">createdDateTime</span></span>|<span data-ttu-id="8f947-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f947-164">DateTimeOffset</span></span>|<span data-ttu-id="8f947-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8f947-165">DateTime the object was created.</span></span> <span data-ttu-id="8f947-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-167">说明</span><span class="sxs-lookup"><span data-stu-id="8f947-167">description</span></span>|<span data-ttu-id="8f947-168">String</span><span class="sxs-lookup"><span data-stu-id="8f947-168">String</span></span>|<span data-ttu-id="8f947-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8f947-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f947-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8f947-171">displayName</span></span>|<span data-ttu-id="8f947-172">String</span><span class="sxs-lookup"><span data-stu-id="8f947-172">String</span></span>|<span data-ttu-id="8f947-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8f947-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f947-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-175">version</span><span class="sxs-lookup"><span data-stu-id="8f947-175">version</span></span>|<span data-ttu-id="8f947-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8f947-176">Int32</span></span>|<span data-ttu-id="8f947-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8f947-177">Version of the device configuration.</span></span> <span data-ttu-id="8f947-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f947-179">networkName</span><span class="sxs-lookup"><span data-stu-id="8f947-179">networkName</span></span>|<span data-ttu-id="8f947-180">String</span><span class="sxs-lookup"><span data-stu-id="8f947-180">String</span></span>|<span data-ttu-id="8f947-181">从[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="8f947-181">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="8f947-182">ssid</span><span class="sxs-lookup"><span data-stu-id="8f947-182">ssid</span></span>|<span data-ttu-id="8f947-183">String</span><span class="sxs-lookup"><span data-stu-id="8f947-183">String</span></span>|<span data-ttu-id="8f947-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="8f947-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="8f947-185">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-185">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="8f947-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="8f947-186">connectAutomatically</span></span>|<span data-ttu-id="8f947-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f947-187">Boolean</span></span>|<span data-ttu-id="8f947-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="8f947-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8f947-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="8f947-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="8f947-190">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-190">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="8f947-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="8f947-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8f947-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="8f947-192">Boolean</span></span>|<span data-ttu-id="8f947-193">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="8f947-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="8f947-194">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f947-194">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="8f947-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8f947-195">wiFiSecurityType</span></span>|[<span data-ttu-id="8f947-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8f947-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="8f947-197">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="8f947-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8f947-198">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8f947-198">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="8f947-199">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="8f947-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="8f947-200">eapType</span><span class="sxs-lookup"><span data-stu-id="8f947-200">eapType</span></span>|[<span data-ttu-id="8f947-201">androidEapType</span><span class="sxs-lookup"><span data-stu-id="8f947-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="8f947-202">指示 Wi-fi 终结点（路由器）上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="8f947-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="8f947-203">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="8f947-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="8f947-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8f947-204">authenticationMethod</span></span>|[<span data-ttu-id="8f947-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8f947-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="8f947-206">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时，客户端（设备）需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8f947-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="8f947-207">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="8f947-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="8f947-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="8f947-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="8f947-209">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="8f947-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="8f947-210">EAP 类型为 EAP 时，用于身份验证的非 EAP 方法（内部标识）-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="8f947-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="8f947-211">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="8f947-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="8f947-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="8f947-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="8f947-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="8f947-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="8f947-214">当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法（内部标识）。</span><span class="sxs-lookup"><span data-stu-id="8f947-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="8f947-215">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="8f947-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="8f947-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="8f947-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="8f947-217">String</span><span class="sxs-lookup"><span data-stu-id="8f947-217">String</span></span>|<span data-ttu-id="8f947-218">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时启用标识隐私（外部标识）。</span><span class="sxs-lookup"><span data-stu-id="8f947-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="8f947-219">此处提供的字符串用于在用户尝试连接到 Wlan 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="8f947-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="8f947-220">proxySettings</span><span class="sxs-lookup"><span data-stu-id="8f947-220">proxySettings</span></span>|[<span data-ttu-id="8f947-221">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="8f947-221">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="8f947-222">此 Wlan 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="8f947-222">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="8f947-223">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="8f947-223">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="8f947-224">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="8f947-224">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="8f947-225">String</span><span class="sxs-lookup"><span data-stu-id="8f947-225">String</span></span>|<span data-ttu-id="8f947-226">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f947-226">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="8f947-227">此 URL 通常是 PAC （代理自动配置）文件的位置。</span><span class="sxs-lookup"><span data-stu-id="8f947-227">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="8f947-228">响应</span><span class="sxs-lookup"><span data-stu-id="8f947-228">Response</span></span>
<span data-ttu-id="8f947-229">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8f947-229">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f947-230">示例</span><span class="sxs-lookup"><span data-stu-id="8f947-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f947-231">请求</span><span class="sxs-lookup"><span data-stu-id="8f947-231">Request</span></span>
<span data-ttu-id="8f947-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f947-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1671

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```

### <a name="response"></a><span data-ttu-id="8f947-233">响应</span><span class="sxs-lookup"><span data-stu-id="8f947-233">Response</span></span>
<span data-ttu-id="8f947-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f947-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1843

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```




