---
title: 创建 androidForWorkEnterpriseWiFiConfiguration
description: 创建新的 androidForWorkEnterpriseWiFiConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcef78f6fef3e331cfe6f27f1178191fe4be3857
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534650"
---
# <a name="create-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="4d323-103">创建 androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="4d323-103">Create androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="4d323-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d323-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d323-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d323-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d323-106">创建新的[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4d323-106">Create a new [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d323-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d323-107">Prerequisites</span></span>
<span data-ttu-id="4d323-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d323-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d323-110">Permission type</span></span>|<span data-ttu-id="4d323-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d323-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d323-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d323-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d323-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d323-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d323-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d323-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d323-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d323-115">Not supported.</span></span>|
|<span data-ttu-id="4d323-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d323-116">Application</span></span>|<span data-ttu-id="4d323-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d323-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d323-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d323-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4d323-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d323-119">Request headers</span></span>
|<span data-ttu-id="4d323-120">标头</span><span class="sxs-lookup"><span data-stu-id="4d323-120">Header</span></span>|<span data-ttu-id="4d323-121">值</span><span class="sxs-lookup"><span data-stu-id="4d323-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d323-122">授权</span><span class="sxs-lookup"><span data-stu-id="4d323-122">Authorization</span></span>|<span data-ttu-id="4d323-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d323-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d323-124">接受</span><span class="sxs-lookup"><span data-stu-id="4d323-124">Accept</span></span>|<span data-ttu-id="4d323-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d323-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d323-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d323-126">Request body</span></span>
<span data-ttu-id="4d323-127">在请求正文中，提供 androidForWorkEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d323-127">In the request body, supply a JSON representation for the androidForWorkEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="4d323-128">下表显示创建 androidForWorkEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d323-128">The following table shows the properties that are required when you create the androidForWorkEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="4d323-129">属性</span><span class="sxs-lookup"><span data-stu-id="4d323-129">Property</span></span>|<span data-ttu-id="4d323-130">类型</span><span class="sxs-lookup"><span data-stu-id="4d323-130">Type</span></span>|<span data-ttu-id="4d323-131">说明</span><span class="sxs-lookup"><span data-stu-id="4d323-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d323-132">id</span><span class="sxs-lookup"><span data-stu-id="4d323-132">id</span></span>|<span data-ttu-id="4d323-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4d323-133">String</span></span>|<span data-ttu-id="4d323-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d323-134">Key of the entity.</span></span> <span data-ttu-id="4d323-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d323-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4d323-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d323-137">DateTimeOffset</span></span>|<span data-ttu-id="4d323-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4d323-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4d323-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d323-140">roleScopeTagIds</span></span>|<span data-ttu-id="4d323-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="4d323-141">String collection</span></span>|<span data-ttu-id="4d323-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4d323-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4d323-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4d323-144">supportsScopeTags</span></span>|<span data-ttu-id="4d323-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d323-145">Boolean</span></span>|<span data-ttu-id="4d323-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4d323-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4d323-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4d323-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4d323-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4d323-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4d323-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4d323-149">This property is read-only.</span></span> <span data-ttu-id="4d323-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4d323-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4d323-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4d323-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4d323-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4d323-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4d323-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4d323-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4d323-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4d323-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4d323-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4d323-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4d323-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4d323-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4d323-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4d323-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4d323-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4d323-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4d323-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d323-163">createdDateTime</span></span>|<span data-ttu-id="4d323-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d323-164">DateTimeOffset</span></span>|<span data-ttu-id="4d323-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4d323-165">DateTime the object was created.</span></span> <span data-ttu-id="4d323-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-167">说明</span><span class="sxs-lookup"><span data-stu-id="4d323-167">description</span></span>|<span data-ttu-id="4d323-168">String</span><span class="sxs-lookup"><span data-stu-id="4d323-168">String</span></span>|<span data-ttu-id="4d323-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4d323-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d323-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4d323-171">displayName</span></span>|<span data-ttu-id="4d323-172">String</span><span class="sxs-lookup"><span data-stu-id="4d323-172">String</span></span>|<span data-ttu-id="4d323-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4d323-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d323-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-175">version</span><span class="sxs-lookup"><span data-stu-id="4d323-175">version</span></span>|<span data-ttu-id="4d323-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4d323-176">Int32</span></span>|<span data-ttu-id="4d323-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4d323-177">Version of the device configuration.</span></span> <span data-ttu-id="4d323-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d323-179">networkName</span><span class="sxs-lookup"><span data-stu-id="4d323-179">networkName</span></span>|<span data-ttu-id="4d323-180">字符串</span><span class="sxs-lookup"><span data-stu-id="4d323-180">String</span></span>|<span data-ttu-id="4d323-181">从[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="4d323-181">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="4d323-182">ssid</span><span class="sxs-lookup"><span data-stu-id="4d323-182">ssid</span></span>|<span data-ttu-id="4d323-183">字符串</span><span class="sxs-lookup"><span data-stu-id="4d323-183">String</span></span>|<span data-ttu-id="4d323-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="4d323-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="4d323-185">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-185">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="4d323-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="4d323-186">connectAutomatically</span></span>|<span data-ttu-id="4d323-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d323-187">Boolean</span></span>|<span data-ttu-id="4d323-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="4d323-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="4d323-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="4d323-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="4d323-190">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-190">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="4d323-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="4d323-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="4d323-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d323-192">Boolean</span></span>|<span data-ttu-id="4d323-193">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="4d323-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="4d323-194">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d323-194">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="4d323-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="4d323-195">wiFiSecurityType</span></span>|[<span data-ttu-id="4d323-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="4d323-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="4d323-197">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="4d323-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="4d323-198">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="4d323-198">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="4d323-199">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="4d323-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="4d323-200">eapType</span><span class="sxs-lookup"><span data-stu-id="4d323-200">eapType</span></span>|[<span data-ttu-id="4d323-201">androidEapType</span><span class="sxs-lookup"><span data-stu-id="4d323-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="4d323-202">指示 Wi-fi 终结点（路由器）上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="4d323-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="4d323-203">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="4d323-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="4d323-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4d323-204">authenticationMethod</span></span>|[<span data-ttu-id="4d323-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4d323-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="4d323-206">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时，客户端（设备）需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="4d323-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="4d323-207">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="4d323-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4d323-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="4d323-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="4d323-209">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="4d323-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="4d323-210">EAP 类型为 EAP 时，用于身份验证的非 EAP 方法（内部标识）-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="4d323-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="4d323-211">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="4d323-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="4d323-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="4d323-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="4d323-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="4d323-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="4d323-214">当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法（内部标识）。</span><span class="sxs-lookup"><span data-stu-id="4d323-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="4d323-215">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="4d323-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="4d323-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="4d323-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="4d323-217">字符串</span><span class="sxs-lookup"><span data-stu-id="4d323-217">String</span></span>|<span data-ttu-id="4d323-218">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时启用标识隐私（外部标识）。</span><span class="sxs-lookup"><span data-stu-id="4d323-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="4d323-219">此处提供的字符串用于在用户尝试连接到 Wlan 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="4d323-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="4d323-220">响应</span><span class="sxs-lookup"><span data-stu-id="4d323-220">Response</span></span>
<span data-ttu-id="4d323-221">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4d323-221">If successful, this method returns a `201 Created` response code and a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d323-222">示例</span><span class="sxs-lookup"><span data-stu-id="4d323-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d323-223">请求</span><span class="sxs-lookup"><span data-stu-id="4d323-223">Request</span></span>
<span data-ttu-id="4d323-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d323-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="4d323-225">响应</span><span class="sxs-lookup"><span data-stu-id="4d323-225">Response</span></span>
<span data-ttu-id="4d323-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d323-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1717

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```






