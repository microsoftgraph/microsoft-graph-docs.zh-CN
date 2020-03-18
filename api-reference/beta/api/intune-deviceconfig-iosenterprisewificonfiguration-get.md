---
title: 获取 iosEnterpriseWiFiConfiguration
description: 读取 iosEnterpriseWiFiConfiguration 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0098fd23510d8925175f41070119aff9ed159d66
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42750899"
---
# <a name="get-iosenterprisewificonfiguration"></a><span data-ttu-id="bf668-103">获取 iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="bf668-103">Get iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="bf668-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf668-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf668-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf668-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf668-106">读取[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf668-106">Read properties and relationships of the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf668-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf668-107">Prerequisites</span></span>
<span data-ttu-id="bf668-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf668-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf668-110">Permission type</span></span>|<span data-ttu-id="bf668-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf668-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf668-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf668-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf668-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf668-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bf668-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf668-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf668-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf668-115">Not supported.</span></span>|
|<span data-ttu-id="bf668-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf668-116">Application</span></span>|<span data-ttu-id="bf668-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf668-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf668-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf668-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf668-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bf668-119">Optional query parameters</span></span>
<span data-ttu-id="bf668-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bf668-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf668-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf668-121">Request headers</span></span>
|<span data-ttu-id="bf668-122">标头</span><span class="sxs-lookup"><span data-stu-id="bf668-122">Header</span></span>|<span data-ttu-id="bf668-123">值</span><span class="sxs-lookup"><span data-stu-id="bf668-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf668-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf668-124">Authorization</span></span>|<span data-ttu-id="bf668-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf668-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf668-126">接受</span><span class="sxs-lookup"><span data-stu-id="bf668-126">Accept</span></span>|<span data-ttu-id="bf668-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bf668-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf668-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf668-128">Request body</span></span>
<span data-ttu-id="bf668-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf668-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf668-130">响应</span><span class="sxs-lookup"><span data-stu-id="bf668-130">Response</span></span>
<span data-ttu-id="bf668-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf668-131">If successful, this method returns a `200 OK` response code and [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf668-132">示例</span><span class="sxs-lookup"><span data-stu-id="bf668-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf668-133">请求</span><span class="sxs-lookup"><span data-stu-id="bf668-133">Request</span></span>
<span data-ttu-id="bf668-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf668-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bf668-135">响应</span><span class="sxs-lookup"><span data-stu-id="bf668-135">Response</span></span>
<span data-ttu-id="bf668-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf668-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2269

{
  "value": {
    "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
    "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaPersonal",
    "proxySettings": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "preSharedKey": "Pre Shared Key value",
    "eapType": "leap",
    "eapFastConfiguration": "useProtectedAccessCredential",
    "trustedServerCertificateNames": [
      "Trusted Server Certificate Names value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
    "usernameFormatString": "Username Format String value",
    "passwordFormatString": "Password Format String value"
  }
}
```




