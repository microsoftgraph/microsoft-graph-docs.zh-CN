---
title: 创建 androidEnterpriseWiFiConfiguration
description: 创建新的 androidEnterpriseWiFiConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e0f841444d2c91ad644cde481afbe0c804ce0b00
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393695"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="a52af-103">创建 androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a52af-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="a52af-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a52af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a52af-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a52af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a52af-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a52af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a52af-107">创建新的[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a52af-107">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a52af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a52af-108">Prerequisites</span></span>
<span data-ttu-id="a52af-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a52af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a52af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a52af-111">Permission type</span></span>|<span data-ttu-id="a52af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a52af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a52af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a52af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a52af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a52af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a52af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a52af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a52af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a52af-116">Not supported.</span></span>|
|<span data-ttu-id="a52af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a52af-117">Application</span></span>|<span data-ttu-id="a52af-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a52af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a52af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a52af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a52af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a52af-120">Request headers</span></span>
|<span data-ttu-id="a52af-121">标头</span><span class="sxs-lookup"><span data-stu-id="a52af-121">Header</span></span>|<span data-ttu-id="a52af-122">值</span><span class="sxs-lookup"><span data-stu-id="a52af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a52af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a52af-123">Authorization</span></span>|<span data-ttu-id="a52af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a52af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a52af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a52af-125">Accept</span></span>|<span data-ttu-id="a52af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a52af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a52af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a52af-127">Request body</span></span>
<span data-ttu-id="a52af-128">在请求正文中，提供 androidEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a52af-128">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="a52af-129">下表显示时创建 androidEnterpriseWiFiConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a52af-129">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="a52af-130">属性</span><span class="sxs-lookup"><span data-stu-id="a52af-130">Property</span></span>|<span data-ttu-id="a52af-131">类型</span><span class="sxs-lookup"><span data-stu-id="a52af-131">Type</span></span>|<span data-ttu-id="a52af-132">说明</span><span class="sxs-lookup"><span data-stu-id="a52af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a52af-133">id</span><span class="sxs-lookup"><span data-stu-id="a52af-133">id</span></span>|<span data-ttu-id="a52af-134">String</span><span class="sxs-lookup"><span data-stu-id="a52af-134">String</span></span>|<span data-ttu-id="a52af-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a52af-135">Key of the entity.</span></span> <span data-ttu-id="a52af-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a52af-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a52af-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a52af-138">DateTimeOffset</span></span>|<span data-ttu-id="a52af-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a52af-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a52af-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a52af-141">roleScopeTagIds</span></span>|<span data-ttu-id="a52af-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="a52af-142">String collection</span></span>|<span data-ttu-id="a52af-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a52af-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a52af-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a52af-145">supportsScopeTags</span></span>|<span data-ttu-id="a52af-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a52af-146">Boolean</span></span>|<span data-ttu-id="a52af-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a52af-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a52af-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a52af-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a52af-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="a52af-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a52af-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a52af-150">This property is read-only.</span></span> <span data-ttu-id="a52af-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a52af-152">createdDateTime</span></span>|<span data-ttu-id="a52af-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a52af-153">DateTimeOffset</span></span>|<span data-ttu-id="a52af-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a52af-154">DateTime the object was created.</span></span> <span data-ttu-id="a52af-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-156">description</span><span class="sxs-lookup"><span data-stu-id="a52af-156">description</span></span>|<span data-ttu-id="a52af-157">String</span><span class="sxs-lookup"><span data-stu-id="a52af-157">String</span></span>|<span data-ttu-id="a52af-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a52af-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a52af-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a52af-160">displayName</span></span>|<span data-ttu-id="a52af-161">String</span><span class="sxs-lookup"><span data-stu-id="a52af-161">String</span></span>|<span data-ttu-id="a52af-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a52af-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a52af-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-164">version</span><span class="sxs-lookup"><span data-stu-id="a52af-164">version</span></span>|<span data-ttu-id="a52af-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a52af-165">Int32</span></span>|<span data-ttu-id="a52af-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a52af-166">Version of the device configuration.</span></span> <span data-ttu-id="a52af-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a52af-168">networkName</span><span class="sxs-lookup"><span data-stu-id="a52af-168">networkName</span></span>|<span data-ttu-id="a52af-169">String</span><span class="sxs-lookup"><span data-stu-id="a52af-169">String</span></span>|<span data-ttu-id="a52af-170">网络名称继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-170">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="a52af-171">ssid</span><span class="sxs-lookup"><span data-stu-id="a52af-171">ssid</span></span>|<span data-ttu-id="a52af-172">String</span><span class="sxs-lookup"><span data-stu-id="a52af-172">String</span></span>|<span data-ttu-id="a52af-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="a52af-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="a52af-174">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-174">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="a52af-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a52af-175">connectAutomatically</span></span>|<span data-ttu-id="a52af-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="a52af-176">Boolean</span></span>|<span data-ttu-id="a52af-177">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="a52af-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a52af-178">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="a52af-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="a52af-179">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-179">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="a52af-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a52af-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a52af-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a52af-181">Boolean</span></span>|<span data-ttu-id="a52af-182">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="a52af-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="a52af-183">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a52af-183">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="a52af-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a52af-184">wiFiSecurityType</span></span>|[<span data-ttu-id="a52af-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a52af-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="a52af-186">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="a52af-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a52af-187">继承自[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a52af-187">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="a52af-188">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="a52af-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="a52af-189">eapType</span><span class="sxs-lookup"><span data-stu-id="a52af-189">eapType</span></span>|[<span data-ttu-id="a52af-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="a52af-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="a52af-191">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="a52af-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="a52af-192">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="a52af-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="a52af-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a52af-193">authenticationMethod</span></span>|[<span data-ttu-id="a52af-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a52af-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="a52af-195">指示客户端 （设备） 所需 EAP 类型配置为 PEAP 或 EAP TTL 时要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a52af-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="a52af-196">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="a52af-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="a52af-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="a52af-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="a52af-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="a52af-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="a52af-199">身份验证 （内部标识） EAP 类型时 EAP TTL 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="a52af-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="a52af-200">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="a52af-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="a52af-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="a52af-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="a52af-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="a52af-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="a52af-203">身份验证 （内部标识） EAP 类型时 PEAP 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="a52af-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="a52af-204">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="a52af-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="a52af-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="a52af-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="a52af-206">String</span><span class="sxs-lookup"><span data-stu-id="a52af-206">String</span></span>|<span data-ttu-id="a52af-207">当 EAP 类型配置为 EAP TTL 或 PEAP 启用标识隐私 （外部标识）。</span><span class="sxs-lookup"><span data-stu-id="a52af-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="a52af-208">此处提供的字符串用于在尝试连接到 Wi-fi 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="a52af-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="a52af-209">响应</span><span class="sxs-lookup"><span data-stu-id="a52af-209">Response</span></span>
<span data-ttu-id="a52af-210">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a52af-210">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a52af-211">示例</span><span class="sxs-lookup"><span data-stu-id="a52af-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="a52af-212">请求</span><span class="sxs-lookup"><span data-stu-id="a52af-212">Request</span></span>
<span data-ttu-id="a52af-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a52af-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a52af-214">响应</span><span class="sxs-lookup"><span data-stu-id="a52af-214">Response</span></span>
<span data-ttu-id="a52af-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a52af-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




