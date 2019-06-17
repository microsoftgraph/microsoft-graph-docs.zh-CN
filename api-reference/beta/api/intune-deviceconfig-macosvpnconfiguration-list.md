---
title: 列出 macOSVpnConfigurations
description: 列出 macOSVpnConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2e17e557edb3f585727f99c3088fe139127332a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963070"
---
# <a name="list-macosvpnconfigurations"></a><span data-ttu-id="41146-103">列出 macOSVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="41146-103">List macOSVpnConfigurations</span></span>

> <span data-ttu-id="41146-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41146-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41146-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41146-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41146-106">列出[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41146-106">List properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41146-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="41146-107">Prerequisites</span></span>
<span data-ttu-id="41146-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41146-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41146-110">Permission type</span></span>|<span data-ttu-id="41146-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41146-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41146-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41146-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41146-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41146-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41146-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41146-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41146-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41146-115">Not supported.</span></span>|
|<span data-ttu-id="41146-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41146-116">Application</span></span>|<span data-ttu-id="41146-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41146-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41146-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41146-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41146-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41146-119">Request headers</span></span>
|<span data-ttu-id="41146-120">标头</span><span class="sxs-lookup"><span data-stu-id="41146-120">Header</span></span>|<span data-ttu-id="41146-121">值</span><span class="sxs-lookup"><span data-stu-id="41146-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41146-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41146-122">Authorization</span></span>|<span data-ttu-id="41146-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41146-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41146-124">接受</span><span class="sxs-lookup"><span data-stu-id="41146-124">Accept</span></span>|<span data-ttu-id="41146-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41146-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41146-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41146-126">Request body</span></span>
<span data-ttu-id="41146-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41146-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41146-128">响应</span><span class="sxs-lookup"><span data-stu-id="41146-128">Response</span></span>
<span data-ttu-id="41146-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="41146-129">If successful, this method returns a `200 OK` response code and a collection of [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41146-130">示例</span><span class="sxs-lookup"><span data-stu-id="41146-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="41146-131">请求</span><span class="sxs-lookup"><span data-stu-id="41146-131">Request</span></span>
<span data-ttu-id="41146-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41146-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="41146-133">响应</span><span class="sxs-lookup"><span data-stu-id="41146-133">Response</span></span>
<span data-ttu-id="41146-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41146-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3191

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
      "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
      "optInToDeviceIdSharing": true
    }
  ]
}
```





