---
title: 列出 iosVpnConfigurations
description: 列出 iosVpnConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 070bd7fe31d7bd0e7eb6eea74415728b13836ff5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155788"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="12f6c-103">列出 iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="12f6c-103">List iosVpnConfigurations</span></span>

<span data-ttu-id="12f6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12f6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12f6c-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12f6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12f6c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12f6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12f6c-107">列出 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12f6c-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12f6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12f6c-108">Prerequisites</span></span>
<span data-ttu-id="12f6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12f6c-111">Permission type</span></span>|<span data-ttu-id="12f6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12f6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12f6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12f6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12f6c-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12f6c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="12f6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12f6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12f6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12f6c-116">Not supported.</span></span>|
|<span data-ttu-id="12f6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12f6c-117">Application</span></span>|<span data-ttu-id="12f6c-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12f6c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12f6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12f6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12f6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12f6c-120">Request headers</span></span>
|<span data-ttu-id="12f6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="12f6c-121">Header</span></span>|<span data-ttu-id="12f6c-122">值</span><span class="sxs-lookup"><span data-stu-id="12f6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12f6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f6c-123">Authorization</span></span>|<span data-ttu-id="12f6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12f6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12f6c-125">接受</span><span class="sxs-lookup"><span data-stu-id="12f6c-125">Accept</span></span>|<span data-ttu-id="12f6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12f6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12f6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12f6c-127">Request body</span></span>
<span data-ttu-id="12f6c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12f6c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12f6c-129">响应</span><span class="sxs-lookup"><span data-stu-id="12f6c-129">Response</span></span>
<span data-ttu-id="12f6c-130">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="12f6c-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f6c-131">示例</span><span class="sxs-lookup"><span data-stu-id="12f6c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="12f6c-132">请求</span><span class="sxs-lookup"><span data-stu-id="12f6c-132">Request</span></span>
<span data-ttu-id="12f6c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12f6c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="12f6c-134">响应</span><span class="sxs-lookup"><span data-stu-id="12f6c-134">Response</span></span>
<span data-ttu-id="12f6c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12f6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3955

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVpnConfiguration",
      "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
      "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
    }
  ]
}
```




