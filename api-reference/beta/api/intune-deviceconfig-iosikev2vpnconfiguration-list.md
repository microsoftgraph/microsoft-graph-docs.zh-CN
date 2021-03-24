---
title: 列出 iosikEv2VpnConfigurations
description: 列出 iosikEv2VpnConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d834bb45dc5cf7ada80e21c28e1208a22acb4a3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131545"
---
# <a name="list-iosikev2vpnconfigurations"></a><span data-ttu-id="3f65f-103">列出 iosikEv2VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="3f65f-103">List iosikEv2VpnConfigurations</span></span>

<span data-ttu-id="3f65f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f65f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f65f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f65f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f65f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f65f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f65f-107">列出 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f65f-107">List properties and relationships of the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f65f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f65f-108">Prerequisites</span></span>
<span data-ttu-id="3f65f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f65f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f65f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f65f-111">Permission type</span></span>|<span data-ttu-id="3f65f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f65f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f65f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f65f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f65f-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f65f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f65f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f65f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f65f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f65f-116">Not supported.</span></span>|
|<span data-ttu-id="3f65f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f65f-117">Application</span></span>|<span data-ttu-id="3f65f-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f65f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f65f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f65f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f65f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f65f-120">Request headers</span></span>
|<span data-ttu-id="3f65f-121">标头</span><span class="sxs-lookup"><span data-stu-id="3f65f-121">Header</span></span>|<span data-ttu-id="3f65f-122">值</span><span class="sxs-lookup"><span data-stu-id="3f65f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f65f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f65f-123">Authorization</span></span>|<span data-ttu-id="3f65f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f65f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f65f-125">接受</span><span class="sxs-lookup"><span data-stu-id="3f65f-125">Accept</span></span>|<span data-ttu-id="3f65f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f65f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f65f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f65f-127">Request body</span></span>
<span data-ttu-id="3f65f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f65f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f65f-129">响应</span><span class="sxs-lookup"><span data-stu-id="3f65f-129">Response</span></span>
<span data-ttu-id="3f65f-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3f65f-130">If successful, this method returns a `200 OK` response code and a collection of [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f65f-131">示例</span><span class="sxs-lookup"><span data-stu-id="3f65f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f65f-132">请求</span><span class="sxs-lookup"><span data-stu-id="3f65f-132">Request</span></span>
<span data-ttu-id="3f65f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f65f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3f65f-134">响应</span><span class="sxs-lookup"><span data-stu-id="3f65f-134">Response</span></span>
<span data-ttu-id="3f65f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f65f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6357

{
  "value": [
    {
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
      "providerType": "appProxy",
      "associatedDomains": [
        "Associated Domains value"
      ],
      "excludedDomains": [
        "Excluded Domains value"
      ],
      "disableOnDemandUserOverride": true,
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "optInToDeviceIdSharing": true,
      "userDomain": "User Domain value",
      "strictEnforcement": true,
      "cloudName": "Cloud Name value",
      "excludeList": [
        "Exclude List value"
      ],
      "targetedMobileApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
      "allowDefaultChildSecurityAssociationParameters": true,
      "alwaysOnConfiguration": {
        "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
        "tunnelConfiguration": "cellular",
        "userToggleEnabled": true,
        "voicemailExceptionAction": "allowTrafficOutside",
        "airPrintExceptionAction": "allowTrafficOutside",
        "cellularExceptionAction": "allowTrafficOutside",
        "allowAllCaptiveNetworkPlugins": true,
        "allowedCaptiveNetworkPlugins": {
          "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
          "allowedBundleIdentifiers": [
            "Allowed Bundle Identifiers value"
          ]
        },
        "allowCaptiveWebSheet": true,
        "natKeepAliveIntervalInSeconds": 13,
        "natKeepAliveOffloadEnable": true
      },
      "enableAlwaysOnConfiguration": true,
      "mtuSizeInBytes": 14
    }
  ]
}
```




