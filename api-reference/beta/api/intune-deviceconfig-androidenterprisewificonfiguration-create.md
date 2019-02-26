---
title: 创建 androidEnterpriseWiFiConfiguration
description: 创建新的 androidEnterpriseWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 466d5526682ab11dd2e8da7e1fcf1f3c8fddcc72
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166680"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="3f22b-103">创建 androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="3f22b-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="3f22b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f22b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f22b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f22b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f22b-106">创建新的[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f22b-106">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f22b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f22b-107">Prerequisites</span></span>
<span data-ttu-id="3f22b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3f22b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f22b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f22b-110">Permission type</span></span>|<span data-ttu-id="3f22b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3f22b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f22b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f22b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f22b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f22b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f22b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f22b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f22b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f22b-115">Not supported.</span></span>|
|<span data-ttu-id="3f22b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f22b-116">Application</span></span>|<span data-ttu-id="3f22b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f22b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f22b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f22b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f22b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f22b-119">Request headers</span></span>
|<span data-ttu-id="3f22b-120">标头</span><span class="sxs-lookup"><span data-stu-id="3f22b-120">Header</span></span>|<span data-ttu-id="3f22b-121">值</span><span class="sxs-lookup"><span data-stu-id="3f22b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f22b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f22b-122">Authorization</span></span>|<span data-ttu-id="3f22b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f22b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f22b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3f22b-124">Accept</span></span>|<span data-ttu-id="3f22b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f22b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f22b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f22b-126">Request body</span></span>
<span data-ttu-id="3f22b-127">在请求正文中, 提供 androidEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f22b-127">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="3f22b-128">下表显示创建 androidEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3f22b-128">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="3f22b-129">属性</span><span class="sxs-lookup"><span data-stu-id="3f22b-129">Property</span></span>|<span data-ttu-id="3f22b-130">类型</span><span class="sxs-lookup"><span data-stu-id="3f22b-130">Type</span></span>|<span data-ttu-id="3f22b-131">说明</span><span class="sxs-lookup"><span data-stu-id="3f22b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f22b-132">id</span><span class="sxs-lookup"><span data-stu-id="3f22b-132">id</span></span>|<span data-ttu-id="3f22b-133">String</span><span class="sxs-lookup"><span data-stu-id="3f22b-133">String</span></span>|<span data-ttu-id="3f22b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3f22b-134">Key of the entity.</span></span> <span data-ttu-id="3f22b-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f22b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3f22b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f22b-137">DateTimeOffset</span></span>|<span data-ttu-id="3f22b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3f22b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3f22b-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f22b-140">roleScopeTagIds</span></span>|<span data-ttu-id="3f22b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3f22b-141">String collection</span></span>|<span data-ttu-id="3f22b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3f22b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f22b-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3f22b-144">supportsScopeTags</span></span>|<span data-ttu-id="3f22b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f22b-145">Boolean</span></span>|<span data-ttu-id="3f22b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3f22b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f22b-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3f22b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f22b-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3f22b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f22b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3f22b-149">This property is read-only.</span></span> <span data-ttu-id="3f22b-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f22b-151">createdDateTime</span></span>|<span data-ttu-id="3f22b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f22b-152">DateTimeOffset</span></span>|<span data-ttu-id="3f22b-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3f22b-153">DateTime the object was created.</span></span> <span data-ttu-id="3f22b-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-155">description</span><span class="sxs-lookup"><span data-stu-id="3f22b-155">description</span></span>|<span data-ttu-id="3f22b-156">String</span><span class="sxs-lookup"><span data-stu-id="3f22b-156">String</span></span>|<span data-ttu-id="3f22b-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3f22b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f22b-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3f22b-159">displayName</span></span>|<span data-ttu-id="3f22b-160">String</span><span class="sxs-lookup"><span data-stu-id="3f22b-160">String</span></span>|<span data-ttu-id="3f22b-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3f22b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f22b-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-163">version</span><span class="sxs-lookup"><span data-stu-id="3f22b-163">version</span></span>|<span data-ttu-id="3f22b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3f22b-164">Int32</span></span>|<span data-ttu-id="3f22b-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3f22b-165">Version of the device configuration.</span></span> <span data-ttu-id="3f22b-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-167">networkName</span><span class="sxs-lookup"><span data-stu-id="3f22b-167">networkName</span></span>|<span data-ttu-id="3f22b-168">String</span><span class="sxs-lookup"><span data-stu-id="3f22b-168">String</span></span>|<span data-ttu-id="3f22b-169">从[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="3f22b-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-170">ssid</span><span class="sxs-lookup"><span data-stu-id="3f22b-170">ssid</span></span>|<span data-ttu-id="3f22b-171">String</span><span class="sxs-lookup"><span data-stu-id="3f22b-171">String</span></span>|<span data-ttu-id="3f22b-172">这是广播到所有设备的 wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="3f22b-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="3f22b-173">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3f22b-174">connectAutomatically</span></span>|<span data-ttu-id="3f22b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f22b-175">Boolean</span></span>|<span data-ttu-id="3f22b-176">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="3f22b-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="3f22b-177">将此设置为 true 将跳过用户提示, 并自动将设备连接到 wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="3f22b-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="3f22b-178">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3f22b-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3f22b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f22b-180">Boolean</span></span>|<span data-ttu-id="3f22b-181">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="3f22b-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="3f22b-182">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f22b-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="3f22b-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3f22b-183">wiFiSecurityType</span></span>|[<span data-ttu-id="3f22b-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3f22b-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="3f22b-185">指示 wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="3f22b-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="3f22b-186">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="3f22b-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="3f22b-187">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="3f22b-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="3f22b-188">eapType</span><span class="sxs-lookup"><span data-stu-id="3f22b-188">eapType</span></span>|[<span data-ttu-id="3f22b-189">androidEapType</span><span class="sxs-lookup"><span data-stu-id="3f22b-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="3f22b-190">指示在 wlan 终结点 (路由器) 上设置的 EAP 协议的类型。</span><span class="sxs-lookup"><span data-stu-id="3f22b-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="3f22b-191">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="3f22b-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="3f22b-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3f22b-192">authenticationMethod</span></span>|[<span data-ttu-id="3f22b-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3f22b-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="3f22b-194">指示在将 EAP 类型配置为 PEAP 或 EAP-TTLS 时, 客户端 (设备) 需要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3f22b-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="3f22b-195">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="3f22b-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="3f22b-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="3f22b-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="3f22b-197">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="3f22b-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="3f22b-198">eap 类型为 eap 时, 用于身份验证的非 EAP 方法 (内部标识)-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="3f22b-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="3f22b-199">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="3f22b-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="3f22b-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="3f22b-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="3f22b-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="3f22b-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="3f22b-202">当 EAP 类型为 PEAP 且 Authenticationmethod 为用户名和密码时, 用于身份验证的非 EAP 方法 (内部标识)。</span><span class="sxs-lookup"><span data-stu-id="3f22b-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="3f22b-203">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="3f22b-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="3f22b-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="3f22b-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="3f22b-205">String</span><span class="sxs-lookup"><span data-stu-id="3f22b-205">String</span></span>|<span data-ttu-id="3f22b-206">将 eap 类型配置为 eap-TTLS 或 PEAP 时启用标识隐私 (外部标识)。</span><span class="sxs-lookup"><span data-stu-id="3f22b-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="3f22b-207">此处提供的字符串用于在用户尝试连接到 wlan 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="3f22b-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="3f22b-208">响应</span><span class="sxs-lookup"><span data-stu-id="3f22b-208">Response</span></span>
<span data-ttu-id="3f22b-209">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f22b-209">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f22b-210">示例</span><span class="sxs-lookup"><span data-stu-id="3f22b-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f22b-211">请求</span><span class="sxs-lookup"><span data-stu-id="3f22b-211">Request</span></span>
<span data-ttu-id="3f22b-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f22b-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 765

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="3f22b-213">响应</span><span class="sxs-lookup"><span data-stu-id="3f22b-213">Response</span></span>
<span data-ttu-id="3f22b-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f22b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 937

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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




