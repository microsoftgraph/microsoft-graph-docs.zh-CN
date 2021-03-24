---
title: 创建 macOSWiredNetworkConfiguration
description: 创建新的 macOSWiredNetworkConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91003cdb7b48da0271dcf83651628b4a3b5dde47
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131202"
---
# <a name="create-macoswirednetworkconfiguration"></a><span data-ttu-id="380b0-103">创建 macOSWiredNetworkConfiguration</span><span class="sxs-lookup"><span data-stu-id="380b0-103">Create macOSWiredNetworkConfiguration</span></span>

<span data-ttu-id="380b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="380b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="380b0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="380b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="380b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="380b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="380b0-107">创建新的 [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="380b0-107">Create a new [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="380b0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="380b0-108">Prerequisites</span></span>
<span data-ttu-id="380b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="380b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="380b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="380b0-111">Permission type</span></span>|<span data-ttu-id="380b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="380b0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="380b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="380b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="380b0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="380b0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="380b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="380b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="380b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="380b0-116">Not supported.</span></span>|
|<span data-ttu-id="380b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="380b0-117">Application</span></span>|<span data-ttu-id="380b0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="380b0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="380b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="380b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="380b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="380b0-120">Request headers</span></span>
|<span data-ttu-id="380b0-121">标头</span><span class="sxs-lookup"><span data-stu-id="380b0-121">Header</span></span>|<span data-ttu-id="380b0-122">值</span><span class="sxs-lookup"><span data-stu-id="380b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="380b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="380b0-123">Authorization</span></span>|<span data-ttu-id="380b0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="380b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="380b0-125">接受</span><span class="sxs-lookup"><span data-stu-id="380b0-125">Accept</span></span>|<span data-ttu-id="380b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="380b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="380b0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="380b0-127">Request body</span></span>
<span data-ttu-id="380b0-128">在请求正文中，提供 macOSWiredNetworkConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="380b0-128">In the request body, supply a JSON representation for the macOSWiredNetworkConfiguration object.</span></span>

<span data-ttu-id="380b0-129">下表显示创建 macOSWiredNetworkConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="380b0-129">The following table shows the properties that are required when you create the macOSWiredNetworkConfiguration.</span></span>

|<span data-ttu-id="380b0-130">属性</span><span class="sxs-lookup"><span data-stu-id="380b0-130">Property</span></span>|<span data-ttu-id="380b0-131">类型</span><span class="sxs-lookup"><span data-stu-id="380b0-131">Type</span></span>|<span data-ttu-id="380b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="380b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="380b0-133">id</span><span class="sxs-lookup"><span data-stu-id="380b0-133">id</span></span>|<span data-ttu-id="380b0-134">String</span><span class="sxs-lookup"><span data-stu-id="380b0-134">String</span></span>|<span data-ttu-id="380b0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="380b0-135">Key of the entity.</span></span> <span data-ttu-id="380b0-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="380b0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="380b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="380b0-138">DateTimeOffset</span></span>|<span data-ttu-id="380b0-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="380b0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="380b0-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="380b0-141">roleScopeTagIds</span></span>|<span data-ttu-id="380b0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="380b0-142">String collection</span></span>|<span data-ttu-id="380b0-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="380b0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="380b0-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="380b0-145">supportsScopeTags</span></span>|<span data-ttu-id="380b0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="380b0-146">Boolean</span></span>|<span data-ttu-id="380b0-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="380b0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="380b0-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="380b0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="380b0-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="380b0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="380b0-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="380b0-150">This property is read-only.</span></span> <span data-ttu-id="380b0-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="380b0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="380b0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="380b0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="380b0-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="380b0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="380b0-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="380b0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="380b0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="380b0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="380b0-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="380b0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="380b0-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="380b0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="380b0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="380b0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="380b0-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="380b0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="380b0-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="380b0-164">createdDateTime</span></span>|<span data-ttu-id="380b0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="380b0-165">DateTimeOffset</span></span>|<span data-ttu-id="380b0-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="380b0-166">DateTime the object was created.</span></span> <span data-ttu-id="380b0-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-168">说明</span><span class="sxs-lookup"><span data-stu-id="380b0-168">description</span></span>|<span data-ttu-id="380b0-169">String</span><span class="sxs-lookup"><span data-stu-id="380b0-169">String</span></span>|<span data-ttu-id="380b0-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="380b0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="380b0-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="380b0-172">displayName</span></span>|<span data-ttu-id="380b0-173">String</span><span class="sxs-lookup"><span data-stu-id="380b0-173">String</span></span>|<span data-ttu-id="380b0-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="380b0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="380b0-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-176">version</span><span class="sxs-lookup"><span data-stu-id="380b0-176">version</span></span>|<span data-ttu-id="380b0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="380b0-177">Int32</span></span>|<span data-ttu-id="380b0-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="380b0-178">Version of the device configuration.</span></span> <span data-ttu-id="380b0-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="380b0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="380b0-180">networkName</span><span class="sxs-lookup"><span data-stu-id="380b0-180">networkName</span></span>|<span data-ttu-id="380b0-181">String</span><span class="sxs-lookup"><span data-stu-id="380b0-181">String</span></span>|<span data-ttu-id="380b0-182">网络名称</span><span class="sxs-lookup"><span data-stu-id="380b0-182">Network Name</span></span>|
|<span data-ttu-id="380b0-183">networkInterface</span><span class="sxs-lookup"><span data-stu-id="380b0-183">networkInterface</span></span>|[<span data-ttu-id="380b0-184">wiredNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="380b0-184">wiredNetworkInterface</span></span>](../resources/intune-deviceconfig-wirednetworkinterface.md)|<span data-ttu-id="380b0-185">网络接口。</span><span class="sxs-lookup"><span data-stu-id="380b0-185">Network interface.</span></span> <span data-ttu-id="380b0-186">可取值为：`anyEthernet`、`firstActiveEthernet`、`secondActiveEthernet`、`thirdActiveEthernet`、`firstEthernet`、`secondEthernet` 或 `thirdEthernet`。</span><span class="sxs-lookup"><span data-stu-id="380b0-186">Possible values are: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.</span></span>|
|<span data-ttu-id="380b0-187">eapType</span><span class="sxs-lookup"><span data-stu-id="380b0-187">eapType</span></span>|[<span data-ttu-id="380b0-188">eapType</span><span class="sxs-lookup"><span data-stu-id="380b0-188">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="380b0-189">可扩展身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="380b0-189">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="380b0-190">指示在有线网络上设置的 EAP 协议类型。</span><span class="sxs-lookup"><span data-stu-id="380b0-190">Indicates the type of EAP protocol set on the wired network.</span></span> <span data-ttu-id="380b0-191">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="380b0-191">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="380b0-192">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="380b0-192">eapFastConfiguration</span></span>|[<span data-ttu-id="380b0-193">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="380b0-193">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="380b0-194">当 EAP-FAST 为所选的 EAP 类型时，EAP-FAST 配置选项。</span><span class="sxs-lookup"><span data-stu-id="380b0-194">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="380b0-195">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="380b0-195">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="380b0-196">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="380b0-196">trustedServerCertificateNames</span></span>|<span data-ttu-id="380b0-197">String collection</span><span class="sxs-lookup"><span data-stu-id="380b0-197">String collection</span></span>|<span data-ttu-id="380b0-198">将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="380b0-198">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="380b0-199">这是由受信任证书颁发机构颁发给 CA 证书颁发机构颁发的 (名) 。</span><span class="sxs-lookup"><span data-stu-id="380b0-199">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="380b0-200">如果提供此信息，可以在最终用户连接到此有线网络时绕过显示在最终用户设备上的动态信任对话框。</span><span class="sxs-lookup"><span data-stu-id="380b0-200">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this wired network.</span></span>|
|<span data-ttu-id="380b0-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="380b0-201">authenticationMethod</span></span>|[<span data-ttu-id="380b0-202">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="380b0-202">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="380b0-203">当 EAP 类型配置为 PEAP 或 EAP-TTLS 时身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="380b0-203">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="380b0-204">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="380b0-204">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="380b0-205">nonEapAuthenticationMethodForEapTtls</span><span class="sxs-lookup"><span data-stu-id="380b0-205">nonEapAuthenticationMethodForEapTtls</span></span>|[<span data-ttu-id="380b0-206">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="380b0-206">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="380b0-207">当 EAP 类型为 EAP-TTLS) Authentication 方法为 Username 和 Password 时，用于身份验证的非 EAP (内部标识方法。</span><span class="sxs-lookup"><span data-stu-id="380b0-207">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="380b0-208">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="380b0-208">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="380b0-209">enableOuterIdentityPrivacy</span><span class="sxs-lookup"><span data-stu-id="380b0-209">enableOuterIdentityPrivacy</span></span>|<span data-ttu-id="380b0-210">String</span><span class="sxs-lookup"><span data-stu-id="380b0-210">String</span></span>|<span data-ttu-id="380b0-211">将 EAP (EAP 类型) EAP-TTLS、EAP-FAST 或 PEAP 时，启用标识隐私和外部标识。</span><span class="sxs-lookup"><span data-stu-id="380b0-211">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="380b0-212">此属性会屏蔽输入文本的用户名。</span><span class="sxs-lookup"><span data-stu-id="380b0-212">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="380b0-213">例如，如果使用"匿名"，则使用真实用户名对此有线网络进行身份验证的每个用户将显示为"匿名"。</span><span class="sxs-lookup"><span data-stu-id="380b0-213">For example, if you use 'anonymous', each user that authenticates with this wired network using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="380b0-214">响应</span><span class="sxs-lookup"><span data-stu-id="380b0-214">Response</span></span>
<span data-ttu-id="380b0-215">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="380b0-215">If successful, this method returns a `201 Created` response code and a [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="380b0-216">示例</span><span class="sxs-lookup"><span data-stu-id="380b0-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="380b0-217">请求</span><span class="sxs-lookup"><span data-stu-id="380b0-217">Request</span></span>
<span data-ttu-id="380b0-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="380b0-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
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
  "networkInterface": "firstActiveEthernet",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
}
```

### <a name="response"></a><span data-ttu-id="380b0-219">响应</span><span class="sxs-lookup"><span data-stu-id="380b0-219">Response</span></span>
<span data-ttu-id="380b0-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="380b0-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
  "id": "e5a57519-7519-e5a5-1975-a5e51975a5e5",
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
  "networkInterface": "firstActiveEthernet",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "nonEapAuthenticationMethodForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "enableOuterIdentityPrivacy": "Enable Outer Identity Privacy value"
}
```




