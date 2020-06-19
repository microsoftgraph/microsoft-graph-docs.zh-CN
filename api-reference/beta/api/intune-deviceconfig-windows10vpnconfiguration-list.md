---
title: 列出 windows10VpnConfigurations
description: 列出 windows10VpnConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bdf7dc2c4dd3c26fd21df40567d4c59b09e73176
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792595"
---
# <a name="list-windows10vpnconfigurations"></a><span data-ttu-id="2bbf0-103">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="2bbf0-103">List windows10VpnConfigurations</span></span>

<span data-ttu-id="2bbf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bbf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bbf0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bbf0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bbf0-107">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-107">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bbf0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2bbf0-108">Prerequisites</span></span>
<span data-ttu-id="2bbf0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2bbf0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2bbf0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bbf0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bbf0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bbf0-111">Permission type</span></span>|<span data-ttu-id="2bbf0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2bbf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bbf0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bbf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bbf0-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bbf0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2bbf0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bbf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bbf0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-116">Not supported.</span></span>|
|<span data-ttu-id="2bbf0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bbf0-117">Application</span></span>|<span data-ttu-id="2bbf0-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bbf0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bbf0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bbf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2bbf0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bbf0-120">Request headers</span></span>
|<span data-ttu-id="2bbf0-121">标头</span><span class="sxs-lookup"><span data-stu-id="2bbf0-121">Header</span></span>|<span data-ttu-id="2bbf0-122">值</span><span class="sxs-lookup"><span data-stu-id="2bbf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bbf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bbf0-123">Authorization</span></span>|<span data-ttu-id="2bbf0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bbf0-125">接受</span><span class="sxs-lookup"><span data-stu-id="2bbf0-125">Accept</span></span>|<span data-ttu-id="2bbf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bbf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bbf0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bbf0-127">Request body</span></span>
<span data-ttu-id="2bbf0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bbf0-129">响应</span><span class="sxs-lookup"><span data-stu-id="2bbf0-129">Response</span></span>
<span data-ttu-id="2bbf0-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-130">If successful, this method returns a `200 OK` response code and a collection of [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bbf0-131">示例</span><span class="sxs-lookup"><span data-stu-id="2bbf0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bbf0-132">请求</span><span class="sxs-lookup"><span data-stu-id="2bbf0-132">Request</span></span>
<span data-ttu-id="2bbf0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bbf0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2bbf0-134">响应</span><span class="sxs-lookup"><span data-stu-id="2bbf0-134">Response</span></span>
<span data-ttu-id="2bbf0-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="2bbf0-135">Here is an example of the response.</span></span> <span data-ttu-id="2bbf0-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="2bbf0-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2bbf0-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2bbf0-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5260

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
      "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "customXml": "Y3VzdG9tWG1s",
      "profileTarget": "device",
      "connectionType": "f5EdgeClient",
      "enableSplitTunneling": true,
      "enableAlwaysOn": true,
      "enableDeviceTunnel": true,
      "enableDnsRegistration": true,
      "dnsSuffixes": [
        "Dns Suffixes value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "rememberUserCredentials": true,
      "enableConditionalAccess": true,
      "enableSingleSignOnWithAlternateCertificate": true,
      "singleSignOnEku": {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      },
      "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
      "eapXml": "ZWFwWG1s",
      "proxyServer": {
        "@odata.type": "microsoft.graph.windows10VpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4,
        "bypassProxyServerForLocalAddress": true
      },
      "associatedApps": [
        {
          "@odata.type": "microsoft.graph.windows10AssociatedApps",
          "appType": "universal",
          "identifier": "Identifier value"
        }
      ],
      "onlyAssociatedAppsCanUseConnection": true,
      "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
      "trafficRules": [
        {
          "@odata.type": "microsoft.graph.vpnTrafficRule",
          "name": "Name value",
          "protocols": 9,
          "localPortRanges": [
            {
              "@odata.type": "microsoft.graph.numberRange",
              "lowerNumber": 11,
              "upperNumber": 11
            }
          ],
          "remotePortRanges": [
            {
              "@odata.type": "microsoft.graph.numberRange",
              "lowerNumber": 11,
              "upperNumber": 11
            }
          ],
          "localAddressRanges": [
            {
              "@odata.type": "microsoft.graph.iPv4Range",
              "lowerAddress": "Lower Address value",
              "upperAddress": "Upper Address value"
            }
          ],
          "remoteAddressRanges": [
            {
              "@odata.type": "microsoft.graph.iPv4Range",
              "lowerAddress": "Lower Address value",
              "upperAddress": "Upper Address value"
            }
          ],
          "appId": "App Id value",
          "appType": "desktop",
          "routingPolicyType": "splitTunnel",
          "claims": "Claims value"
        }
      ],
      "routes": [
        {
          "@odata.type": "microsoft.graph.vpnRoute",
          "destinationPrefix": "Destination Prefix value",
          "prefixSize": 10
        }
      ],
      "dnsRules": [
        {
          "@odata.type": "microsoft.graph.vpnDnsRule",
          "name": "Name value",
          "servers": [
            "Servers value"
          ],
          "proxyServerUri": "Proxy Server Uri value",
          "autoTrigger": true,
          "persistent": true
        }
      ],
      "trustedNetworkDomains": [
        "Trusted Network Domains value"
      ],
      "cryptographySuite": {
        "@odata.type": "microsoft.graph.cryptographySuite",
        "encryptionMethod": "des",
        "integrityCheckMethod": "sha1_96",
        "dhGroup": "group2",
        "cipherTransformConstants": "des",
        "authenticationTransformConstants": "sha1_96",
        "pfsGroup": "pfs2"
      }
    }
  ]
}
```



