---
title: 更新 androidWorkProfileEnterpriseWiFiConfiguration
description: 更新 androidWorkProfileEnterpriseWiFiConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05dd752507a402fb54d27dad40a4264617395b50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406757"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="eefee-103">更新 androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="eefee-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="eefee-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="eefee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eefee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eefee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eefee-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eefee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eefee-107">更新[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eefee-107">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eefee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eefee-108">Prerequisites</span></span>
<span data-ttu-id="eefee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="eefee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eefee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eefee-111">Permission type</span></span>|<span data-ttu-id="eefee-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eefee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eefee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eefee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eefee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eefee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eefee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eefee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eefee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eefee-116">Not supported.</span></span>|
|<span data-ttu-id="eefee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eefee-117">Application</span></span>|<span data-ttu-id="eefee-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eefee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eefee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eefee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eefee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eefee-120">Request headers</span></span>
|<span data-ttu-id="eefee-121">标头</span><span class="sxs-lookup"><span data-stu-id="eefee-121">Header</span></span>|<span data-ttu-id="eefee-122">值</span><span class="sxs-lookup"><span data-stu-id="eefee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eefee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eefee-123">Authorization</span></span>|<span data-ttu-id="eefee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eefee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eefee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eefee-125">Accept</span></span>|<span data-ttu-id="eefee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eefee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eefee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eefee-127">Request body</span></span>
<span data-ttu-id="eefee-128">在请求正文中，提供[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eefee-128">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="eefee-129">下表显示时创建[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eefee-129">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="eefee-130">属性</span><span class="sxs-lookup"><span data-stu-id="eefee-130">Property</span></span>|<span data-ttu-id="eefee-131">类型</span><span class="sxs-lookup"><span data-stu-id="eefee-131">Type</span></span>|<span data-ttu-id="eefee-132">说明</span><span class="sxs-lookup"><span data-stu-id="eefee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eefee-133">id</span><span class="sxs-lookup"><span data-stu-id="eefee-133">id</span></span>|<span data-ttu-id="eefee-134">String</span><span class="sxs-lookup"><span data-stu-id="eefee-134">String</span></span>|<span data-ttu-id="eefee-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eefee-135">Key of the entity.</span></span> <span data-ttu-id="eefee-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eefee-137">lastModifiedDateTime</span></span>|<span data-ttu-id="eefee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eefee-138">DateTimeOffset</span></span>|<span data-ttu-id="eefee-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eefee-139">DateTime the object was last modified.</span></span> <span data-ttu-id="eefee-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eefee-141">roleScopeTagIds</span></span>|<span data-ttu-id="eefee-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="eefee-142">String collection</span></span>|<span data-ttu-id="eefee-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="eefee-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eefee-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eefee-145">supportsScopeTags</span></span>|<span data-ttu-id="eefee-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="eefee-146">Boolean</span></span>|<span data-ttu-id="eefee-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="eefee-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eefee-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="eefee-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eefee-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="eefee-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eefee-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="eefee-150">This property is read-only.</span></span> <span data-ttu-id="eefee-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eefee-152">createdDateTime</span></span>|<span data-ttu-id="eefee-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eefee-153">DateTimeOffset</span></span>|<span data-ttu-id="eefee-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eefee-154">DateTime the object was created.</span></span> <span data-ttu-id="eefee-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-156">description</span><span class="sxs-lookup"><span data-stu-id="eefee-156">description</span></span>|<span data-ttu-id="eefee-157">String</span><span class="sxs-lookup"><span data-stu-id="eefee-157">String</span></span>|<span data-ttu-id="eefee-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="eefee-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eefee-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-160">displayName</span><span class="sxs-lookup"><span data-stu-id="eefee-160">displayName</span></span>|<span data-ttu-id="eefee-161">String</span><span class="sxs-lookup"><span data-stu-id="eefee-161">String</span></span>|<span data-ttu-id="eefee-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="eefee-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eefee-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-164">version</span><span class="sxs-lookup"><span data-stu-id="eefee-164">version</span></span>|<span data-ttu-id="eefee-165">Int32</span><span class="sxs-lookup"><span data-stu-id="eefee-165">Int32</span></span>|<span data-ttu-id="eefee-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="eefee-166">Version of the device configuration.</span></span> <span data-ttu-id="eefee-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eefee-168">networkName</span><span class="sxs-lookup"><span data-stu-id="eefee-168">networkName</span></span>|<span data-ttu-id="eefee-169">String</span><span class="sxs-lookup"><span data-stu-id="eefee-169">String</span></span>|<span data-ttu-id="eefee-170">网络名称继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-170">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="eefee-171">ssid</span><span class="sxs-lookup"><span data-stu-id="eefee-171">ssid</span></span>|<span data-ttu-id="eefee-172">String</span><span class="sxs-lookup"><span data-stu-id="eefee-172">String</span></span>|<span data-ttu-id="eefee-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="eefee-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="eefee-174">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-174">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="eefee-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="eefee-175">connectAutomatically</span></span>|<span data-ttu-id="eefee-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="eefee-176">Boolean</span></span>|<span data-ttu-id="eefee-177">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="eefee-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="eefee-178">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="eefee-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="eefee-179">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-179">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="eefee-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="eefee-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="eefee-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="eefee-181">Boolean</span></span>|<span data-ttu-id="eefee-182">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="eefee-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="eefee-183">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eefee-183">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="eefee-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="eefee-184">wiFiSecurityType</span></span>|[<span data-ttu-id="eefee-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="eefee-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="eefee-186">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="eefee-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="eefee-187">继承自[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="eefee-187">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="eefee-188">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="eefee-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="eefee-189">eapType</span><span class="sxs-lookup"><span data-stu-id="eefee-189">eapType</span></span>|[<span data-ttu-id="eefee-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="eefee-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="eefee-191">指示 EAP 协议设置类型 Wi-fi 终结点 （路由器）。</span><span class="sxs-lookup"><span data-stu-id="eefee-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="eefee-192">可取值为：`eapTls`、`eapTtls`、`peap`。</span><span class="sxs-lookup"><span data-stu-id="eefee-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="eefee-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="eefee-193">authenticationMethod</span></span>|[<span data-ttu-id="eefee-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="eefee-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="eefee-195">指示客户端 （设备） 所需 EAP 类型配置为 PEAP 或 EAP TTL 时要使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="eefee-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="eefee-196">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="eefee-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="eefee-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="eefee-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="eefee-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="eefee-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="eefee-199">身份验证 （内部标识） EAP 类型时 EAP TTL 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="eefee-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="eefee-200">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="eefee-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="eefee-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="eefee-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="eefee-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="eefee-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="eefee-203">身份验证 （内部标识） EAP 类型时 PEAP 和 Authenticationmethod 非 EAP 方法是用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="eefee-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="eefee-204">可取值为：`none`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="eefee-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="eefee-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="eefee-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="eefee-206">String</span><span class="sxs-lookup"><span data-stu-id="eefee-206">String</span></span>|<span data-ttu-id="eefee-207">当 EAP 类型配置为 EAP TTL 或 PEAP 启用标识隐私 （外部标识）。</span><span class="sxs-lookup"><span data-stu-id="eefee-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="eefee-208">此处提供的字符串用于在尝试连接到 Wi-fi 网络时屏蔽各个用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="eefee-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="eefee-209">响应</span><span class="sxs-lookup"><span data-stu-id="eefee-209">Response</span></span>
<span data-ttu-id="eefee-210">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eefee-210">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eefee-211">示例</span><span class="sxs-lookup"><span data-stu-id="eefee-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="eefee-212">请求</span><span class="sxs-lookup"><span data-stu-id="eefee-212">Request</span></span>
<span data-ttu-id="eefee-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eefee-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 776

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="eefee-214">响应</span><span class="sxs-lookup"><span data-stu-id="eefee-214">Response</span></span>
<span data-ttu-id="eefee-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eefee-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




