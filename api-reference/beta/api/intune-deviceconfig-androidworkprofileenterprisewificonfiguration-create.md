---
title: 创建 androidWorkProfileEnterpriseWiFiConfiguration
description: 创建新的 androidWorkProfileEnterpriseWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab1c27d72ea671900f177a099806b2e991f2a957
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126575"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="594e3-103">创建 androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="594e3-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="594e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="594e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="594e3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="594e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="594e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="594e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="594e3-107">创建新的 [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="594e3-107">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="594e3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="594e3-108">Prerequisites</span></span>
<span data-ttu-id="594e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="594e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="594e3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="594e3-111">Permission type</span></span>|<span data-ttu-id="594e3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="594e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="594e3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="594e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="594e3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="594e3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="594e3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="594e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="594e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="594e3-116">Not supported.</span></span>|
|<span data-ttu-id="594e3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="594e3-117">Application</span></span>|<span data-ttu-id="594e3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="594e3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="594e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="594e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="594e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="594e3-120">Request headers</span></span>
|<span data-ttu-id="594e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="594e3-121">Header</span></span>|<span data-ttu-id="594e3-122">值</span><span class="sxs-lookup"><span data-stu-id="594e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="594e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="594e3-123">Authorization</span></span>|<span data-ttu-id="594e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="594e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="594e3-125">接受</span><span class="sxs-lookup"><span data-stu-id="594e3-125">Accept</span></span>|<span data-ttu-id="594e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="594e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="594e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="594e3-127">Request body</span></span>
<span data-ttu-id="594e3-128">在请求正文中，提供 androidWorkProfileEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="594e3-128">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="594e3-129">下表显示创建 androidWorkProfileEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="594e3-129">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="594e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="594e3-130">Property</span></span>|<span data-ttu-id="594e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="594e3-131">Type</span></span>|<span data-ttu-id="594e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="594e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="594e3-133">id</span><span class="sxs-lookup"><span data-stu-id="594e3-133">id</span></span>|<span data-ttu-id="594e3-134">String</span><span class="sxs-lookup"><span data-stu-id="594e3-134">String</span></span>|<span data-ttu-id="594e3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="594e3-135">Key of the entity.</span></span> <span data-ttu-id="594e3-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="594e3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="594e3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="594e3-138">DateTimeOffset</span></span>|<span data-ttu-id="594e3-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="594e3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="594e3-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="594e3-141">roleScopeTagIds</span></span>|<span data-ttu-id="594e3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="594e3-142">String collection</span></span>|<span data-ttu-id="594e3-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="594e3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="594e3-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="594e3-145">supportsScopeTags</span></span>|<span data-ttu-id="594e3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="594e3-146">Boolean</span></span>|<span data-ttu-id="594e3-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="594e3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="594e3-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="594e3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="594e3-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="594e3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="594e3-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="594e3-150">This property is read-only.</span></span> <span data-ttu-id="594e3-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="594e3-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="594e3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="594e3-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="594e3-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="594e3-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="594e3-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="594e3-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="594e3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="594e3-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="594e3-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="594e3-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="594e3-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="594e3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="594e3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="594e3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="594e3-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="594e3-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="594e3-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="594e3-164">createdDateTime</span></span>|<span data-ttu-id="594e3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="594e3-165">DateTimeOffset</span></span>|<span data-ttu-id="594e3-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="594e3-166">DateTime the object was created.</span></span> <span data-ttu-id="594e3-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-168">说明</span><span class="sxs-lookup"><span data-stu-id="594e3-168">description</span></span>|<span data-ttu-id="594e3-169">String</span><span class="sxs-lookup"><span data-stu-id="594e3-169">String</span></span>|<span data-ttu-id="594e3-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="594e3-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="594e3-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-172">displayName</span><span class="sxs-lookup"><span data-stu-id="594e3-172">displayName</span></span>|<span data-ttu-id="594e3-173">String</span><span class="sxs-lookup"><span data-stu-id="594e3-173">String</span></span>|<span data-ttu-id="594e3-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="594e3-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="594e3-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-176">version</span><span class="sxs-lookup"><span data-stu-id="594e3-176">version</span></span>|<span data-ttu-id="594e3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="594e3-177">Int32</span></span>|<span data-ttu-id="594e3-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="594e3-178">Version of the device configuration.</span></span> <span data-ttu-id="594e3-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="594e3-180">networkName</span><span class="sxs-lookup"><span data-stu-id="594e3-180">networkName</span></span>|<span data-ttu-id="594e3-181">String</span><span class="sxs-lookup"><span data-stu-id="594e3-181">String</span></span>|<span data-ttu-id="594e3-182">网络名称 继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-182">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="594e3-183">ssid</span><span class="sxs-lookup"><span data-stu-id="594e3-183">ssid</span></span>|<span data-ttu-id="594e3-184">String</span><span class="sxs-lookup"><span data-stu-id="594e3-184">String</span></span>|<span data-ttu-id="594e3-185">这是广播到所有Wi-Fi网络的名称。</span><span class="sxs-lookup"><span data-stu-id="594e3-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="594e3-186">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="594e3-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="594e3-187">connectAutomatically</span></span>|<span data-ttu-id="594e3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="594e3-188">Boolean</span></span>|<span data-ttu-id="594e3-189">此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="594e3-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="594e3-190">如果设置为 true，将跳过用户提示，并自动将设备Wi-Fi网络。</span><span class="sxs-lookup"><span data-stu-id="594e3-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="594e3-191">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-191">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="594e3-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="594e3-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="594e3-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="594e3-193">Boolean</span></span>|<span data-ttu-id="594e3-194">设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="594e3-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="594e3-195">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="594e3-195">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="594e3-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="594e3-196">wiFiSecurityType</span></span>|[<span data-ttu-id="594e3-197">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="594e3-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="594e3-198">指示Wi-Fi是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="594e3-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="594e3-199">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="594e3-199">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="594e3-200">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="594e3-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="594e3-201">eapType</span><span class="sxs-lookup"><span data-stu-id="594e3-201">eapType</span></span>|[<span data-ttu-id="594e3-202">androidEapType</span><span class="sxs-lookup"><span data-stu-id="594e3-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="594e3-203">指示在 Wi-Fi 路由器 (上设置的 EAP) 。</span><span class="sxs-lookup"><span data-stu-id="594e3-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="594e3-204">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="594e3-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="594e3-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="594e3-205">authenticationMethod</span></span>|[<span data-ttu-id="594e3-206">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="594e3-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="594e3-207">指示当 EAP 类型 (EAP 类型) EAP-TTLS 时，需要使用的客户端身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="594e3-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="594e3-208">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="594e3-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="594e3-209">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="594e3-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="594e3-210">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="594e3-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="594e3-211">当 EAP 类型为 EAP-TTLS) Authentication 方法为 Username 和 Password 时，用于身份验证的非 EAP (内部标识方法。</span><span class="sxs-lookup"><span data-stu-id="594e3-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="594e3-212">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="594e3-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="594e3-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="594e3-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="594e3-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="594e3-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="594e3-215">当 EAP 类型为 PEAP (Authentication 方法为 Username 和 Password 时) 非 EAP 身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="594e3-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="594e3-216">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="594e3-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="594e3-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="594e3-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="594e3-218">String</span><span class="sxs-lookup"><span data-stu-id="594e3-218">String</span></span>|<span data-ttu-id="594e3-219">将 EAP (EAP 类型) EAP-TTLS 或 PEAP 时，启用标识隐私和外部标识。</span><span class="sxs-lookup"><span data-stu-id="594e3-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="594e3-220">此处提供的字符串用于在用户尝试连接到网络时屏蔽Wi-Fi用户名。</span><span class="sxs-lookup"><span data-stu-id="594e3-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="594e3-221">proxySettings</span><span class="sxs-lookup"><span data-stu-id="594e3-221">proxySettings</span></span>|[<span data-ttu-id="594e3-222">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="594e3-222">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="594e3-223">此连接代理Wi-Fi类型。</span><span class="sxs-lookup"><span data-stu-id="594e3-223">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="594e3-224">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="594e3-224">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="594e3-225">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="594e3-225">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="594e3-226">String</span><span class="sxs-lookup"><span data-stu-id="594e3-226">String</span></span>|<span data-ttu-id="594e3-227">选择自动配置时代理服务器自动配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="594e3-227">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="594e3-228">此 URL 通常是 PAC 代理自动配置 (文件) 位置。</span><span class="sxs-lookup"><span data-stu-id="594e3-228">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="594e3-229">响应</span><span class="sxs-lookup"><span data-stu-id="594e3-229">Response</span></span>
<span data-ttu-id="594e3-230">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="594e3-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="594e3-231">示例</span><span class="sxs-lookup"><span data-stu-id="594e3-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="594e3-232">请求</span><span class="sxs-lookup"><span data-stu-id="594e3-232">Request</span></span>
<span data-ttu-id="594e3-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="594e3-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="594e3-234">响应</span><span class="sxs-lookup"><span data-stu-id="594e3-234">Response</span></span>
<span data-ttu-id="594e3-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="594e3-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




