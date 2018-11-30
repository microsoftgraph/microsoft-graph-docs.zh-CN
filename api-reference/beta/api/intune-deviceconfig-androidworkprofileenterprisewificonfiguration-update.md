---
title: 更新 androidWorkProfileEnterpriseWiFiConfiguration
description: 更新 androidWorkProfileEnterpriseWiFiConfiguration 对象的属性。
ms.openlocfilehash: 00b0a4b2a2140f9d6aedcacdc1eb0c8a0a68e6c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048567"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="71ba5-103">更新 androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="71ba5-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="71ba5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="71ba5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71ba5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="71ba5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71ba5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="71ba5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71ba5-107">更新[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71ba5-107">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71ba5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="71ba5-108">Prerequisites</span></span>
<span data-ttu-id="71ba5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="71ba5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ba5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71ba5-111">Permission type</span></span>|<span data-ttu-id="71ba5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71ba5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ba5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71ba5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71ba5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ba5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71ba5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71ba5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71ba5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71ba5-116">Not supported.</span></span>|
|<span data-ttu-id="71ba5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71ba5-117">Application</span></span>|<span data-ttu-id="71ba5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="71ba5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71ba5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71ba5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71ba5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71ba5-120">Request headers</span></span>
|<span data-ttu-id="71ba5-121">标头</span><span class="sxs-lookup"><span data-stu-id="71ba5-121">Header</span></span>|<span data-ttu-id="71ba5-122">值</span><span class="sxs-lookup"><span data-stu-id="71ba5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71ba5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71ba5-123">Authorization</span></span>|<span data-ttu-id="71ba5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71ba5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71ba5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71ba5-125">Accept</span></span>|<span data-ttu-id="71ba5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71ba5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ba5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="71ba5-127">Request body</span></span>
<span data-ttu-id="71ba5-128">在请求正文中，提供[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71ba5-128">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="71ba5-129">下表显示时创建[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="71ba5-129">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="71ba5-130">属性</span><span class="sxs-lookup"><span data-stu-id="71ba5-130">Property</span></span>|<span data-ttu-id="71ba5-131">类型</span><span class="sxs-lookup"><span data-stu-id="71ba5-131">Type</span></span>|<span data-ttu-id="71ba5-132">说明</span><span class="sxs-lookup"><span data-stu-id="71ba5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ba5-133">id</span><span class="sxs-lookup"><span data-stu-id="71ba5-133">id</span></span>|<span data-ttu-id="71ba5-134">String</span><span class="sxs-lookup"><span data-stu-id="71ba5-134">String</span></span>|<span data-ttu-id="71ba5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71ba5-135">Key of the entity.</span></span> <span data-ttu-id="71ba5-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71ba5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="71ba5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ba5-138">DateTimeOffset</span></span>|<span data-ttu-id="71ba5-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71ba5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="71ba5-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71ba5-141">roleScopeTagIds</span></span>|<span data-ttu-id="71ba5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="71ba5-142">String collection</span></span>|<span data-ttu-id="71ba5-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="71ba5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71ba5-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71ba5-145">supportsScopeTags</span></span>|<span data-ttu-id="71ba5-146">布尔</span><span class="sxs-lookup"><span data-stu-id="71ba5-146">Boolean</span></span>|<span data-ttu-id="71ba5-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="71ba5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71ba5-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="71ba5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71ba5-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="71ba5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71ba5-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="71ba5-150">This property is read-only.</span></span> <span data-ttu-id="71ba5-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71ba5-152">createdDateTime</span></span>|<span data-ttu-id="71ba5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ba5-153">DateTimeOffset</span></span>|<span data-ttu-id="71ba5-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71ba5-154">DateTime the object was created.</span></span> <span data-ttu-id="71ba5-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-156">description</span><span class="sxs-lookup"><span data-stu-id="71ba5-156">description</span></span>|<span data-ttu-id="71ba5-157">String</span><span class="sxs-lookup"><span data-stu-id="71ba5-157">String</span></span>|<span data-ttu-id="71ba5-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="71ba5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71ba5-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="71ba5-160">displayName</span></span>|<span data-ttu-id="71ba5-161">String</span><span class="sxs-lookup"><span data-stu-id="71ba5-161">String</span></span>|<span data-ttu-id="71ba5-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="71ba5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71ba5-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-164">version</span><span class="sxs-lookup"><span data-stu-id="71ba5-164">version</span></span>|<span data-ttu-id="71ba5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="71ba5-165">Int32</span></span>|<span data-ttu-id="71ba5-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="71ba5-166">Version of the device configuration.</span></span> <span data-ttu-id="71ba5-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-168">networkName</span><span class="sxs-lookup"><span data-stu-id="71ba5-168">networkName</span></span>|<span data-ttu-id="71ba5-169">字符串</span><span class="sxs-lookup"><span data-stu-id="71ba5-169">String</span></span>|<span data-ttu-id="71ba5-170">网络名称继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-170">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-171">ssid</span><span class="sxs-lookup"><span data-stu-id="71ba5-171">ssid</span></span>|<span data-ttu-id="71ba5-172">字符串</span><span class="sxs-lookup"><span data-stu-id="71ba5-172">String</span></span>|<span data-ttu-id="71ba5-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="71ba5-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="71ba5-174">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-174">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="71ba5-175">connectAutomatically</span></span>|<span data-ttu-id="71ba5-176">布尔</span><span class="sxs-lookup"><span data-stu-id="71ba5-176">Boolean</span></span>|<span data-ttu-id="71ba5-177">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="71ba5-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="71ba5-178">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="71ba5-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="71ba5-179">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-179">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="71ba5-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="71ba5-181">布尔</span><span class="sxs-lookup"><span data-stu-id="71ba5-181">Boolean</span></span>|<span data-ttu-id="71ba5-182">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="71ba5-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="71ba5-183">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ba5-183">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="71ba5-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="71ba5-184">wiFiSecurityType</span></span>|[<span data-ttu-id="71ba5-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="71ba5-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="71ba5-186">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="71ba5-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="71ba5-187">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="71ba5-187">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="71ba5-188">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="71ba5-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="71ba5-189">eapType</span><span class="sxs-lookup"><span data-stu-id="71ba5-189">eapType</span></span>|[<span data-ttu-id="71ba5-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="71ba5-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="71ba5-191">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="71ba5-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="71ba5-192">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="71ba5-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="71ba5-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="71ba5-193">authenticationMethod</span></span>|[<span data-ttu-id="71ba5-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="71ba5-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="71ba5-195">指示客户端 （设备） 所需 EAP 类型配置为 PEAP 或 EAP TTL 时要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="71ba5-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="71ba5-196">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="71ba5-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="71ba5-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="71ba5-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="71ba5-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="71ba5-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="71ba5-199">身份验证 （内部标识） EAP 类型时 EAP TTL 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="71ba5-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="71ba5-200">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="71ba5-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="71ba5-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="71ba5-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="71ba5-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="71ba5-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="71ba5-203">身份验证 （内部标识） EAP 类型时 PEAP 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="71ba5-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="71ba5-204">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="71ba5-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="71ba5-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="71ba5-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="71ba5-206">字符串</span><span class="sxs-lookup"><span data-stu-id="71ba5-206">String</span></span>|<span data-ttu-id="71ba5-207">当 EAP 类型配置为 EAP TTL 或 PEAP 启用标识隐私 （外部标识）。</span><span class="sxs-lookup"><span data-stu-id="71ba5-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="71ba5-208">此处提供的字符串用于在尝试连接到 Wi-fi 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="71ba5-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="71ba5-209">响应</span><span class="sxs-lookup"><span data-stu-id="71ba5-209">Response</span></span>
<span data-ttu-id="71ba5-210">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="71ba5-210">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ba5-211">示例</span><span class="sxs-lookup"><span data-stu-id="71ba5-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="71ba5-212">请求</span><span class="sxs-lookup"><span data-stu-id="71ba5-212">Request</span></span>
<span data-ttu-id="71ba5-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71ba5-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 756

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="71ba5-214">响应</span><span class="sxs-lookup"><span data-stu-id="71ba5-214">Response</span></span>
<span data-ttu-id="71ba5-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71ba5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 948

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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





