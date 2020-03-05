---
title: 创建 androidWorkProfileEnterpriseWiFiConfiguration
description: 创建新的 androidWorkProfileEnterpriseWiFiConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4667a184a04e7a7d98c8579800b03476e6ff14ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449563"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="6fa01-103">创建 androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fa01-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="6fa01-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6fa01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fa01-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6fa01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fa01-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fa01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fa01-107">创建新的[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fa01-107">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fa01-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6fa01-108">Prerequisites</span></span>
<span data-ttu-id="6fa01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fa01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa01-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fa01-111">Permission type</span></span>|<span data-ttu-id="6fa01-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6fa01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fa01-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fa01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fa01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fa01-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fa01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fa01-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fa01-116">Not supported.</span></span>|
|<span data-ttu-id="6fa01-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fa01-117">Application</span></span>|<span data-ttu-id="6fa01-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa01-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fa01-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fa01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6fa01-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fa01-120">Request headers</span></span>
|<span data-ttu-id="6fa01-121">标头</span><span class="sxs-lookup"><span data-stu-id="6fa01-121">Header</span></span>|<span data-ttu-id="6fa01-122">值</span><span class="sxs-lookup"><span data-stu-id="6fa01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fa01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa01-123">Authorization</span></span>|<span data-ttu-id="6fa01-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6fa01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fa01-125">接受</span><span class="sxs-lookup"><span data-stu-id="6fa01-125">Accept</span></span>|<span data-ttu-id="6fa01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fa01-127">Request body</span></span>
<span data-ttu-id="6fa01-128">在请求正文中，提供 androidWorkProfileEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fa01-128">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="6fa01-129">下表显示创建 androidWorkProfileEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6fa01-129">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="6fa01-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fa01-130">Property</span></span>|<span data-ttu-id="6fa01-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fa01-131">Type</span></span>|<span data-ttu-id="6fa01-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fa01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa01-133">id</span><span class="sxs-lookup"><span data-stu-id="6fa01-133">id</span></span>|<span data-ttu-id="6fa01-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6fa01-134">String</span></span>|<span data-ttu-id="6fa01-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6fa01-135">Key of the entity.</span></span> <span data-ttu-id="6fa01-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa01-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6fa01-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa01-138">DateTimeOffset</span></span>|<span data-ttu-id="6fa01-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6fa01-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6fa01-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fa01-141">roleScopeTagIds</span></span>|<span data-ttu-id="6fa01-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6fa01-142">String collection</span></span>|<span data-ttu-id="6fa01-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6fa01-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6fa01-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6fa01-145">supportsScopeTags</span></span>|<span data-ttu-id="6fa01-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6fa01-146">Boolean</span></span>|<span data-ttu-id="6fa01-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6fa01-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6fa01-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6fa01-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6fa01-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6fa01-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6fa01-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6fa01-150">This property is read-only.</span></span> <span data-ttu-id="6fa01-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6fa01-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6fa01-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6fa01-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6fa01-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6fa01-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6fa01-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6fa01-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6fa01-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6fa01-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6fa01-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6fa01-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6fa01-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6fa01-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6fa01-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6fa01-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6fa01-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6fa01-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6fa01-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fa01-164">createdDateTime</span></span>|<span data-ttu-id="6fa01-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fa01-165">DateTimeOffset</span></span>|<span data-ttu-id="6fa01-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6fa01-166">DateTime the object was created.</span></span> <span data-ttu-id="6fa01-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-168">说明</span><span class="sxs-lookup"><span data-stu-id="6fa01-168">description</span></span>|<span data-ttu-id="6fa01-169">String</span><span class="sxs-lookup"><span data-stu-id="6fa01-169">String</span></span>|<span data-ttu-id="6fa01-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6fa01-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6fa01-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6fa01-172">displayName</span></span>|<span data-ttu-id="6fa01-173">String</span><span class="sxs-lookup"><span data-stu-id="6fa01-173">String</span></span>|<span data-ttu-id="6fa01-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6fa01-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6fa01-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-176">version</span><span class="sxs-lookup"><span data-stu-id="6fa01-176">version</span></span>|<span data-ttu-id="6fa01-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6fa01-177">Int32</span></span>|<span data-ttu-id="6fa01-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6fa01-178">Version of the device configuration.</span></span> <span data-ttu-id="6fa01-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-180">networkName</span><span class="sxs-lookup"><span data-stu-id="6fa01-180">networkName</span></span>|<span data-ttu-id="6fa01-181">String</span><span class="sxs-lookup"><span data-stu-id="6fa01-181">String</span></span>|<span data-ttu-id="6fa01-182">从[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="6fa01-182">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-183">ssid</span><span class="sxs-lookup"><span data-stu-id="6fa01-183">ssid</span></span>|<span data-ttu-id="6fa01-184">String</span><span class="sxs-lookup"><span data-stu-id="6fa01-184">String</span></span>|<span data-ttu-id="6fa01-185">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="6fa01-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6fa01-186">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6fa01-187">connectAutomatically</span></span>|<span data-ttu-id="6fa01-188">布尔</span><span class="sxs-lookup"><span data-stu-id="6fa01-188">Boolean</span></span>|<span data-ttu-id="6fa01-189">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="6fa01-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6fa01-190">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="6fa01-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6fa01-191">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-191">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6fa01-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6fa01-193">布尔</span><span class="sxs-lookup"><span data-stu-id="6fa01-193">Boolean</span></span>|<span data-ttu-id="6fa01-194">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="6fa01-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6fa01-195">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fa01-195">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6fa01-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6fa01-196">wiFiSecurityType</span></span>|[<span data-ttu-id="6fa01-197">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6fa01-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="6fa01-198">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="6fa01-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6fa01-199">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6fa01-199">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="6fa01-200">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="6fa01-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="6fa01-201">eapType</span><span class="sxs-lookup"><span data-stu-id="6fa01-201">eapType</span></span>|[<span data-ttu-id="6fa01-202">androidEapType</span><span class="sxs-lookup"><span data-stu-id="6fa01-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="6fa01-203">指示 Wi-fi 终结点（路由器）上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="6fa01-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6fa01-204">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="6fa01-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="6fa01-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fa01-205">authenticationMethod</span></span>|[<span data-ttu-id="6fa01-206">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fa01-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6fa01-207">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时，客户端（设备）需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6fa01-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6fa01-208">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="6fa01-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6fa01-209">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="6fa01-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6fa01-210">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="6fa01-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6fa01-211">EAP 类型为 EAP 时，用于身份验证的非 EAP 方法（内部标识）-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="6fa01-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6fa01-212">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="6fa01-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6fa01-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="6fa01-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="6fa01-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="6fa01-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="6fa01-215">当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，用于身份验证的非 EAP 方法（内部标识）。</span><span class="sxs-lookup"><span data-stu-id="6fa01-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6fa01-216">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="6fa01-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6fa01-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6fa01-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6fa01-218">String</span><span class="sxs-lookup"><span data-stu-id="6fa01-218">String</span></span>|<span data-ttu-id="6fa01-219">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时启用标识隐私（外部标识）。</span><span class="sxs-lookup"><span data-stu-id="6fa01-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="6fa01-220">此处提供的字符串用于在用户尝试连接到 Wlan 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="6fa01-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="6fa01-221">proxySettings</span><span class="sxs-lookup"><span data-stu-id="6fa01-221">proxySettings</span></span>|[<span data-ttu-id="6fa01-222">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="6fa01-222">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="6fa01-223">此 Wlan 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="6fa01-223">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="6fa01-224">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="6fa01-224">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="6fa01-225">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="6fa01-225">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="6fa01-226">String</span><span class="sxs-lookup"><span data-stu-id="6fa01-226">String</span></span>|<span data-ttu-id="6fa01-227">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="6fa01-227">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="6fa01-228">此 URL 通常是 PAC （代理自动配置）文件的位置。</span><span class="sxs-lookup"><span data-stu-id="6fa01-228">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="6fa01-229">响应</span><span class="sxs-lookup"><span data-stu-id="6fa01-229">Response</span></span>
<span data-ttu-id="6fa01-230">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fa01-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fa01-231">示例</span><span class="sxs-lookup"><span data-stu-id="6fa01-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fa01-232">请求</span><span class="sxs-lookup"><span data-stu-id="6fa01-232">Request</span></span>
<span data-ttu-id="6fa01-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fa01-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6fa01-234">响应</span><span class="sxs-lookup"><span data-stu-id="6fa01-234">Response</span></span>
<span data-ttu-id="6fa01-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fa01-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





