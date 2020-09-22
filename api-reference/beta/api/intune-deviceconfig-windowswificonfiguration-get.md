---
title: 获取 windowsWifiConfiguration
description: 读取 windowsWifiConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76a9bce9f3b04785146eb415fd3f5e20627eaa8e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011352"
---
# <a name="get-windowswificonfiguration"></a><span data-ttu-id="e72df-103">获取 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e72df-103">Get windowsWifiConfiguration</span></span>

<span data-ttu-id="e72df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e72df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e72df-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e72df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e72df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e72df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e72df-107">读取 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e72df-107">Read properties and relationships of the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e72df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e72df-108">Prerequisites</span></span>
<span data-ttu-id="e72df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e72df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e72df-111">Permission type</span></span>|<span data-ttu-id="e72df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e72df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e72df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e72df-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e72df-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e72df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e72df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e72df-116">Not supported.</span></span>|
|<span data-ttu-id="e72df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e72df-117">Application</span></span>|<span data-ttu-id="e72df-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e72df-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e72df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e72df-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e72df-120">Optional query parameters</span></span>
<span data-ttu-id="e72df-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e72df-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e72df-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e72df-122">Request headers</span></span>
|<span data-ttu-id="e72df-123">标头</span><span class="sxs-lookup"><span data-stu-id="e72df-123">Header</span></span>|<span data-ttu-id="e72df-124">值</span><span class="sxs-lookup"><span data-stu-id="e72df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72df-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72df-125">Authorization</span></span>|<span data-ttu-id="e72df-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e72df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72df-127">接受</span><span class="sxs-lookup"><span data-stu-id="e72df-127">Accept</span></span>|<span data-ttu-id="e72df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e72df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72df-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e72df-129">Request body</span></span>
<span data-ttu-id="e72df-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e72df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e72df-131">响应</span><span class="sxs-lookup"><span data-stu-id="e72df-131">Response</span></span>
<span data-ttu-id="e72df-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e72df-132">If successful, this method returns a `200 OK` response code and [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72df-133">示例</span><span class="sxs-lookup"><span data-stu-id="e72df-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e72df-134">请求</span><span class="sxs-lookup"><span data-stu-id="e72df-134">Request</span></span>
<span data-ttu-id="e72df-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e72df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e72df-136">响应</span><span class="sxs-lookup"><span data-stu-id="e72df-136">Response</span></span>
<span data-ttu-id="e72df-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e72df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
    "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
    "forceFIPSCompliance": true
  }
}
```






