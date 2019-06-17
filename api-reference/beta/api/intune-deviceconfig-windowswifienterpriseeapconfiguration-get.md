---
title: 获取 windowsWifiEnterpriseEAPConfiguration
description: 读取 windowsWifiEnterpriseEAPConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b37beed3576f011288751e73ce25d3cdf7bf2297
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961138"
---
# <a name="get-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="f7989-103">获取 windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7989-103">Get windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="f7989-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7989-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7989-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7989-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7989-106">读取[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7989-106">Read properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7989-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7989-107">Prerequisites</span></span>
<span data-ttu-id="f7989-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7989-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7989-110">Permission type</span></span>|<span data-ttu-id="f7989-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7989-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7989-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7989-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7989-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7989-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f7989-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7989-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7989-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7989-115">Not supported.</span></span>|
|<span data-ttu-id="f7989-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7989-116">Application</span></span>|<span data-ttu-id="f7989-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7989-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7989-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7989-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7989-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7989-119">Optional query parameters</span></span>
<span data-ttu-id="f7989-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7989-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7989-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7989-121">Request headers</span></span>
|<span data-ttu-id="f7989-122">标头</span><span class="sxs-lookup"><span data-stu-id="f7989-122">Header</span></span>|<span data-ttu-id="f7989-123">值</span><span class="sxs-lookup"><span data-stu-id="f7989-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7989-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7989-124">Authorization</span></span>|<span data-ttu-id="f7989-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7989-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7989-126">接受</span><span class="sxs-lookup"><span data-stu-id="f7989-126">Accept</span></span>|<span data-ttu-id="f7989-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f7989-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7989-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7989-128">Request body</span></span>
<span data-ttu-id="f7989-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7989-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7989-130">响应</span><span class="sxs-lookup"><span data-stu-id="f7989-130">Response</span></span>
<span data-ttu-id="f7989-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7989-131">If successful, this method returns a `200 OK` response code and [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7989-132">示例</span><span class="sxs-lookup"><span data-stu-id="f7989-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7989-133">请求</span><span class="sxs-lookup"><span data-stu-id="f7989-133">Request</span></span>
<span data-ttu-id="f7989-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7989-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f7989-135">响应</span><span class="sxs-lookup"><span data-stu-id="f7989-135">Response</span></span>
<span data-ttu-id="f7989-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7989-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2588

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
    "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
    "preSharedKey": "Pre Shared Key value",
    "wifiSecurityType": "wpaPersonal",
    "meteredConnectionLimit": "fixed",
    "ssid": "Ssid value",
    "networkName": "Network Name value",
    "connectAutomatically": true,
    "connectToPreferredNetwork": true,
    "connectWhenNetworkNameIsHidden": true,
    "proxySetting": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "forceFIPSCompliance": true,
    "networkSingleSignOn": "prelogon",
    "maximumAuthenticationTimeoutInSeconds": 5,
    "promptForAdditionalAuthenticationCredentials": true,
    "enablePairwiseMasterKeyCaching": true,
    "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
    "maximumNumberOfPairwiseMasterKeysInCache": 8,
    "enablePreAuthentication": true,
    "maximumPreAuthenticationAttempts": 0,
    "eapType": "leap",
    "trustedServerCertificateNames": [
      "Trusted Server Certificate Names value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
  }
}
```





