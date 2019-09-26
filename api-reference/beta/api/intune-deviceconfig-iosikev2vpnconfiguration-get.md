---
title: 获取 iosikEv2VpnConfiguration
description: 读取 iosikEv2VpnConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8002213185bed9d0391c5d8805c2541496bd4f83
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174373"
---
# <a name="get-iosikev2vpnconfiguration"></a><span data-ttu-id="1ddd7-103">获取 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ddd7-103">Get iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="1ddd7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ddd7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ddd7-106">读取[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-106">Read properties and relationships of the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ddd7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ddd7-107">Prerequisites</span></span>
<span data-ttu-id="1ddd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ddd7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ddd7-110">Permission type</span></span>|<span data-ttu-id="1ddd7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ddd7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ddd7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ddd7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ddd7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ddd7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ddd7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ddd7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ddd7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-115">Not supported.</span></span>|
|<span data-ttu-id="1ddd7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ddd7-116">Application</span></span>|<span data-ttu-id="1ddd7-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ddd7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ddd7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ddd7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ddd7-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ddd7-119">Optional query parameters</span></span>
<span data-ttu-id="1ddd7-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ddd7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ddd7-121">Request headers</span></span>
|<span data-ttu-id="1ddd7-122">标头</span><span class="sxs-lookup"><span data-stu-id="1ddd7-122">Header</span></span>|<span data-ttu-id="1ddd7-123">值</span><span class="sxs-lookup"><span data-stu-id="1ddd7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ddd7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ddd7-124">Authorization</span></span>|<span data-ttu-id="1ddd7-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ddd7-126">接受</span><span class="sxs-lookup"><span data-stu-id="1ddd7-126">Accept</span></span>|<span data-ttu-id="1ddd7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1ddd7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ddd7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ddd7-128">Request body</span></span>
<span data-ttu-id="1ddd7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ddd7-130">响应</span><span class="sxs-lookup"><span data-stu-id="1ddd7-130">Response</span></span>
<span data-ttu-id="1ddd7-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-131">If successful, this method returns a `200 OK` response code and [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ddd7-132">示例</span><span class="sxs-lookup"><span data-stu-id="1ddd7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ddd7-133">请求</span><span class="sxs-lookup"><span data-stu-id="1ddd7-133">Request</span></span>
<span data-ttu-id="1ddd7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1ddd7-135">响应</span><span class="sxs-lookup"><span data-stu-id="1ddd7-135">Response</span></span>
<span data-ttu-id="1ddd7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ddd7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4679

{
  "value": {
    "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
    "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
    "connectionName": "Connection Name value",
    "connectionType": "pulseSecure",
    "loginGroupOrDomain": "Login Group Or Domain value",
    "role": "Role value",
    "realm": "Realm value",
    "server": {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    },
    "identifier": "Identifier value",
    "customData": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ],
    "customKeyValueData": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "enableSplitTunneling": true,
    "authenticationMethod": "usernameAndPassword",
    "enablePerApp": true,
    "safariDomains": [
      "Safari Domains value"
    ],
    "onDemandRules": [
      {
        "@odata.type": "microsoft.graph.vpnOnDemandRule",
        "ssids": [
          "Ssids value"
        ],
        "dnsSearchDomains": [
          "Dns Search Domains value"
        ],
        "probeUrl": "https://example.com/probeUrl/",
        "action": "evaluateConnection",
        "domainAction": "neverConnect",
        "domains": [
          "Domains value"
        ],
        "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
      }
    ],
    "proxyServer": {
      "@odata.type": "microsoft.graph.vpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4
    },
    "optInToDeviceIdSharing": true,
    "providerType": "appProxy",
    "userDomain": "User Domain value",
    "strictEnforcement": true,
    "cloudName": "Cloud Name value",
    "excludeList": [
      "Exclude List value"
    ],
    "childSecurityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "des",
      "securityIntegrityAlgorithm": "sha1_96",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "clientAuthenticationType": "deviceAuthentication",
    "deadPeerDetectionRate": "none",
    "disableMobilityAndMultihoming": true,
    "disableRedirect": true,
    "enableCertificateRevocationCheck": true,
    "enableEAP": true,
    "enablePerfectForwardSecrecy": true,
    "enableUseInternalSubnetAttributes": true,
    "localIdentifier": "empty",
    "remoteIdentifier": "Remote Identifier value",
    "securityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "des",
      "securityIntegrityAlgorithm": "sha1_96",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "serverCertificateCommonName": "Server Certificate Common Name value",
    "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
    "serverCertificateType": "ecdsa256",
    "sharedSecret": "Shared Secret value",
    "tlsMaximumVersion": "Tls Maximum Version value",
    "tlsMinimumVersion": "Tls Minimum Version value",
    "allowDefaultSecurityAssociationParameters": true,
    "allowDefaultChildSecurityAssociationParameters": true
  }
}
```




