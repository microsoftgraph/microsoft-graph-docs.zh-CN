---
title: 创建 androidWorkProfileEnterpriseWiFiConfiguration
description: 创建新的 androidWorkProfileEnterpriseWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27e0ac00b3e3f56b6d70b5cb9d9482de74c9d409
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49237364"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="65a14-103">创建 androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="65a14-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="65a14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65a14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65a14-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65a14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65a14-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65a14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65a14-107">创建新的 [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65a14-107">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65a14-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="65a14-108">Prerequisites</span></span>
<span data-ttu-id="65a14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65a14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65a14-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65a14-111">Permission type</span></span>|<span data-ttu-id="65a14-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65a14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65a14-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65a14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65a14-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a14-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65a14-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65a14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65a14-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65a14-116">Not supported.</span></span>|
|<span data-ttu-id="65a14-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65a14-117">Application</span></span>|<span data-ttu-id="65a14-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a14-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65a14-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65a14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65a14-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65a14-120">Request headers</span></span>
|<span data-ttu-id="65a14-121">标头</span><span class="sxs-lookup"><span data-stu-id="65a14-121">Header</span></span>|<span data-ttu-id="65a14-122">值</span><span class="sxs-lookup"><span data-stu-id="65a14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65a14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65a14-123">Authorization</span></span>|<span data-ttu-id="65a14-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65a14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65a14-125">接受</span><span class="sxs-lookup"><span data-stu-id="65a14-125">Accept</span></span>|<span data-ttu-id="65a14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65a14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65a14-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65a14-127">Request body</span></span>
<span data-ttu-id="65a14-128">在请求正文中，提供 androidWorkProfileEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65a14-128">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="65a14-129">下表显示创建 androidWorkProfileEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65a14-129">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="65a14-130">属性</span><span class="sxs-lookup"><span data-stu-id="65a14-130">Property</span></span>|<span data-ttu-id="65a14-131">类型</span><span class="sxs-lookup"><span data-stu-id="65a14-131">Type</span></span>|<span data-ttu-id="65a14-132">说明</span><span class="sxs-lookup"><span data-stu-id="65a14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a14-133">id</span><span class="sxs-lookup"><span data-stu-id="65a14-133">id</span></span>|<span data-ttu-id="65a14-134">String</span><span class="sxs-lookup"><span data-stu-id="65a14-134">String</span></span>|<span data-ttu-id="65a14-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65a14-135">Key of the entity.</span></span> <span data-ttu-id="65a14-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65a14-137">lastModifiedDateTime</span></span>|<span data-ttu-id="65a14-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65a14-138">DateTimeOffset</span></span>|<span data-ttu-id="65a14-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="65a14-139">DateTime the object was last modified.</span></span> <span data-ttu-id="65a14-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65a14-141">roleScopeTagIds</span></span>|<span data-ttu-id="65a14-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="65a14-142">String collection</span></span>|<span data-ttu-id="65a14-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="65a14-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65a14-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="65a14-145">supportsScopeTags</span></span>|<span data-ttu-id="65a14-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="65a14-146">Boolean</span></span>|<span data-ttu-id="65a14-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="65a14-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65a14-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="65a14-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65a14-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="65a14-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65a14-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="65a14-150">This property is read-only.</span></span> <span data-ttu-id="65a14-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65a14-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="65a14-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65a14-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="65a14-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="65a14-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="65a14-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65a14-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="65a14-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65a14-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="65a14-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="65a14-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="65a14-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65a14-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="65a14-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65a14-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="65a14-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="65a14-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="65a14-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65a14-164">createdDateTime</span></span>|<span data-ttu-id="65a14-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65a14-165">DateTimeOffset</span></span>|<span data-ttu-id="65a14-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="65a14-166">DateTime the object was created.</span></span> <span data-ttu-id="65a14-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-168">description</span><span class="sxs-lookup"><span data-stu-id="65a14-168">description</span></span>|<span data-ttu-id="65a14-169">String</span><span class="sxs-lookup"><span data-stu-id="65a14-169">String</span></span>|<span data-ttu-id="65a14-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="65a14-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65a14-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-172">displayName</span><span class="sxs-lookup"><span data-stu-id="65a14-172">displayName</span></span>|<span data-ttu-id="65a14-173">String</span><span class="sxs-lookup"><span data-stu-id="65a14-173">String</span></span>|<span data-ttu-id="65a14-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="65a14-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65a14-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-176">version</span><span class="sxs-lookup"><span data-stu-id="65a14-176">version</span></span>|<span data-ttu-id="65a14-177">Int32</span><span class="sxs-lookup"><span data-stu-id="65a14-177">Int32</span></span>|<span data-ttu-id="65a14-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="65a14-178">Version of the device configuration.</span></span> <span data-ttu-id="65a14-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65a14-180">networkName</span><span class="sxs-lookup"><span data-stu-id="65a14-180">networkName</span></span>|<span data-ttu-id="65a14-181">String</span><span class="sxs-lookup"><span data-stu-id="65a14-181">String</span></span>|<span data-ttu-id="65a14-182">从[AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="65a14-182">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="65a14-183">ssid</span><span class="sxs-lookup"><span data-stu-id="65a14-183">ssid</span></span>|<span data-ttu-id="65a14-184">String</span><span class="sxs-lookup"><span data-stu-id="65a14-184">String</span></span>|<span data-ttu-id="65a14-185">这是广播到所有设备的 Wi-Fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="65a14-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="65a14-186">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="65a14-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="65a14-187">connectAutomatically</span></span>|<span data-ttu-id="65a14-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="65a14-188">Boolean</span></span>|<span data-ttu-id="65a14-189">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="65a14-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="65a14-190">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="65a14-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="65a14-191">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-191">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="65a14-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="65a14-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="65a14-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="65a14-193">Boolean</span></span>|<span data-ttu-id="65a14-194">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="65a14-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="65a14-195">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65a14-195">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="65a14-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="65a14-196">wiFiSecurityType</span></span>|[<span data-ttu-id="65a14-197">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="65a14-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="65a14-198">指示 Wi-Fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="65a14-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="65a14-199">继承自 [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="65a14-199">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="65a14-200">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="65a14-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="65a14-201">eapType</span><span class="sxs-lookup"><span data-stu-id="65a14-201">eapType</span></span>|[<span data-ttu-id="65a14-202">androidEapType</span><span class="sxs-lookup"><span data-stu-id="65a14-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="65a14-203">指示 Wi-Fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="65a14-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="65a14-204">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="65a14-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="65a14-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="65a14-205">authenticationMethod</span></span>|[<span data-ttu-id="65a14-206">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="65a14-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="65a14-207">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时，客户端 (设备) 需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="65a14-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="65a14-208">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="65a14-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="65a14-209">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="65a14-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="65a14-210">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="65a14-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="65a14-211">在 EAP 类型为 EAP 时，用于身份验证的非 EAP 方法 (内部标识) （eap 类型为 EAP-TTLS，Authenticationmethod 为用户名和密码）。</span><span class="sxs-lookup"><span data-stu-id="65a14-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="65a14-212">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="65a14-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="65a14-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="65a14-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="65a14-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="65a14-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="65a14-215">在 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时，身份验证 (内部标识) 的非 EAP 方法。</span><span class="sxs-lookup"><span data-stu-id="65a14-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="65a14-216">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="65a14-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="65a14-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="65a14-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="65a14-218">String</span><span class="sxs-lookup"><span data-stu-id="65a14-218">String</span></span>|<span data-ttu-id="65a14-219">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时，请启用标识隐私 (外部标识) 。</span><span class="sxs-lookup"><span data-stu-id="65a14-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="65a14-220">此处提供的字符串用于在用户尝试连接到 Wi-Fi 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="65a14-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="65a14-221">proxySettings</span><span class="sxs-lookup"><span data-stu-id="65a14-221">proxySettings</span></span>|[<span data-ttu-id="65a14-222">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="65a14-222">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="65a14-223">此 Wi-Fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="65a14-223">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="65a14-224">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="65a14-224">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="65a14-225">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="65a14-225">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="65a14-226">String</span><span class="sxs-lookup"><span data-stu-id="65a14-226">String</span></span>|<span data-ttu-id="65a14-227">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="65a14-227">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="65a14-228">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="65a14-228">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="65a14-229">响应</span><span class="sxs-lookup"><span data-stu-id="65a14-229">Response</span></span>
<span data-ttu-id="65a14-230">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65a14-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a14-231">示例</span><span class="sxs-lookup"><span data-stu-id="65a14-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="65a14-232">请求</span><span class="sxs-lookup"><span data-stu-id="65a14-232">Request</span></span>
<span data-ttu-id="65a14-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65a14-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65a14-234">响应</span><span class="sxs-lookup"><span data-stu-id="65a14-234">Response</span></span>
<span data-ttu-id="65a14-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65a14-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




