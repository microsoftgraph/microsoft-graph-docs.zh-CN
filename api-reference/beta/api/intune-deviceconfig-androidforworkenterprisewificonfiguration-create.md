---
title: 创建 androidForWorkEnterpriseWiFiConfiguration
description: 创建新的 androidForWorkEnterpriseWiFiConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94cf6ad12a74964d461c6a245513d27188f1f96e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933695"
---
# <a name="create-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="d64ba-103">创建 androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="d64ba-103">Create androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="d64ba-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d64ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d64ba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d64ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d64ba-106">创建新的[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d64ba-106">Create a new [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d64ba-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d64ba-107">Prerequisites</span></span>
<span data-ttu-id="d64ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d64ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d64ba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d64ba-110">Permission type</span></span>|<span data-ttu-id="d64ba-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d64ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d64ba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d64ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d64ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d64ba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d64ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d64ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d64ba-115">Not supported.</span></span>|
|<span data-ttu-id="d64ba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d64ba-116">Application</span></span>|<span data-ttu-id="d64ba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d64ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d64ba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d64ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d64ba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d64ba-119">Request headers</span></span>
|<span data-ttu-id="d64ba-120">标头</span><span class="sxs-lookup"><span data-stu-id="d64ba-120">Header</span></span>|<span data-ttu-id="d64ba-121">值</span><span class="sxs-lookup"><span data-stu-id="d64ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d64ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d64ba-122">Authorization</span></span>|<span data-ttu-id="d64ba-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d64ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d64ba-124">接受</span><span class="sxs-lookup"><span data-stu-id="d64ba-124">Accept</span></span>|<span data-ttu-id="d64ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d64ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d64ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d64ba-126">Request body</span></span>
<span data-ttu-id="d64ba-127">在请求正文中, 提供 androidForWorkEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d64ba-127">In the request body, supply a JSON representation for the androidForWorkEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="d64ba-128">下表显示创建 androidForWorkEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d64ba-128">The following table shows the properties that are required when you create the androidForWorkEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="d64ba-129">属性</span><span class="sxs-lookup"><span data-stu-id="d64ba-129">Property</span></span>|<span data-ttu-id="d64ba-130">类型</span><span class="sxs-lookup"><span data-stu-id="d64ba-130">Type</span></span>|<span data-ttu-id="d64ba-131">说明</span><span class="sxs-lookup"><span data-stu-id="d64ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d64ba-132">id</span><span class="sxs-lookup"><span data-stu-id="d64ba-132">id</span></span>|<span data-ttu-id="d64ba-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d64ba-133">String</span></span>|<span data-ttu-id="d64ba-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d64ba-134">Key of the entity.</span></span> <span data-ttu-id="d64ba-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d64ba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d64ba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d64ba-137">DateTimeOffset</span></span>|<span data-ttu-id="d64ba-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d64ba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d64ba-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d64ba-140">roleScopeTagIds</span></span>|<span data-ttu-id="d64ba-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d64ba-141">String collection</span></span>|<span data-ttu-id="d64ba-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d64ba-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d64ba-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d64ba-144">supportsScopeTags</span></span>|<span data-ttu-id="d64ba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64ba-145">Boolean</span></span>|<span data-ttu-id="d64ba-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d64ba-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d64ba-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d64ba-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d64ba-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d64ba-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d64ba-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d64ba-149">This property is read-only.</span></span> <span data-ttu-id="d64ba-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d64ba-151">createdDateTime</span></span>|<span data-ttu-id="d64ba-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d64ba-152">DateTimeOffset</span></span>|<span data-ttu-id="d64ba-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d64ba-153">DateTime the object was created.</span></span> <span data-ttu-id="d64ba-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-155">说明</span><span class="sxs-lookup"><span data-stu-id="d64ba-155">description</span></span>|<span data-ttu-id="d64ba-156">String</span><span class="sxs-lookup"><span data-stu-id="d64ba-156">String</span></span>|<span data-ttu-id="d64ba-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d64ba-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d64ba-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d64ba-159">displayName</span></span>|<span data-ttu-id="d64ba-160">String</span><span class="sxs-lookup"><span data-stu-id="d64ba-160">String</span></span>|<span data-ttu-id="d64ba-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d64ba-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d64ba-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-163">version</span><span class="sxs-lookup"><span data-stu-id="d64ba-163">version</span></span>|<span data-ttu-id="d64ba-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ba-164">Int32</span></span>|<span data-ttu-id="d64ba-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d64ba-165">Version of the device configuration.</span></span> <span data-ttu-id="d64ba-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-167">networkName</span><span class="sxs-lookup"><span data-stu-id="d64ba-167">networkName</span></span>|<span data-ttu-id="d64ba-168">String</span><span class="sxs-lookup"><span data-stu-id="d64ba-168">String</span></span>|<span data-ttu-id="d64ba-169">从[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="d64ba-169">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-170">ssid</span><span class="sxs-lookup"><span data-stu-id="d64ba-170">ssid</span></span>|<span data-ttu-id="d64ba-171">String</span><span class="sxs-lookup"><span data-stu-id="d64ba-171">String</span></span>|<span data-ttu-id="d64ba-172">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="d64ba-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="d64ba-173">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-173">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="d64ba-174">connectAutomatically</span></span>|<span data-ttu-id="d64ba-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64ba-175">Boolean</span></span>|<span data-ttu-id="d64ba-176">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="d64ba-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="d64ba-177">将此设置为 true 将跳过用户提示, 并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="d64ba-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="d64ba-178">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-178">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d64ba-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d64ba-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64ba-180">Boolean</span></span>|<span data-ttu-id="d64ba-181">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="d64ba-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="d64ba-182">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d64ba-182">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d64ba-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d64ba-183">wiFiSecurityType</span></span>|[<span data-ttu-id="d64ba-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d64ba-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="d64ba-185">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="d64ba-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="d64ba-186">继承自[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d64ba-186">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="d64ba-187">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="d64ba-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="d64ba-188">eapType</span><span class="sxs-lookup"><span data-stu-id="d64ba-188">eapType</span></span>|[<span data-ttu-id="d64ba-189">androidEapType</span><span class="sxs-lookup"><span data-stu-id="d64ba-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="d64ba-190">指示在 Wlan 终结点 (路由器) 上设置的 EAP 协议的类型。</span><span class="sxs-lookup"><span data-stu-id="d64ba-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="d64ba-191">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="d64ba-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="d64ba-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d64ba-192">authenticationMethod</span></span>|[<span data-ttu-id="d64ba-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d64ba-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="d64ba-194">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时, 客户端 (设备) 需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d64ba-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="d64ba-195">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="d64ba-195">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d64ba-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="d64ba-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="d64ba-197">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="d64ba-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="d64ba-198">EAP 类型为 EAP 时, 用于身份验证的非 EAP 方法 (内部标识)-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="d64ba-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="d64ba-199">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="d64ba-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="d64ba-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="d64ba-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="d64ba-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="d64ba-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="d64ba-202">当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时, 用于身份验证的非 EAP 方法 (内部标识)。</span><span class="sxs-lookup"><span data-stu-id="d64ba-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="d64ba-203">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="d64ba-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="d64ba-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="d64ba-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="d64ba-205">String</span><span class="sxs-lookup"><span data-stu-id="d64ba-205">String</span></span>|<span data-ttu-id="d64ba-206">将 EAP 类型配置为 EAP-TTLS 或 PEAP 时启用标识隐私 (外部标识)。</span><span class="sxs-lookup"><span data-stu-id="d64ba-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="d64ba-207">此处提供的字符串用于在用户尝试连接到 Wlan 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="d64ba-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="d64ba-208">响应</span><span class="sxs-lookup"><span data-stu-id="d64ba-208">Response</span></span>
<span data-ttu-id="d64ba-209">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d64ba-209">If successful, this method returns a `201 Created` response code and a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d64ba-210">示例</span><span class="sxs-lookup"><span data-stu-id="d64ba-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="d64ba-211">请求</span><span class="sxs-lookup"><span data-stu-id="d64ba-211">Request</span></span>
<span data-ttu-id="d64ba-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d64ba-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 772

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="d64ba-213">响应</span><span class="sxs-lookup"><span data-stu-id="d64ba-213">Response</span></span>
<span data-ttu-id="d64ba-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d64ba-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 944

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




