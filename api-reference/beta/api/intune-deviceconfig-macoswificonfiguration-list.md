---
title: 列出 macOSWiFiConfigurations
description: 列出 macOSWiFiConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dbd52a086f02fad8783b9d167f4ff879da14efe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127884"
---
# <a name="list-macoswificonfigurations"></a><span data-ttu-id="77cf5-103">列出 macOSWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="77cf5-103">List macOSWiFiConfigurations</span></span>

<span data-ttu-id="77cf5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77cf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77cf5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77cf5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77cf5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77cf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77cf5-107">列出 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77cf5-107">List properties and relationships of the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77cf5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77cf5-108">Prerequisites</span></span>
<span data-ttu-id="77cf5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77cf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77cf5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77cf5-111">Permission type</span></span>|<span data-ttu-id="77cf5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77cf5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77cf5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77cf5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77cf5-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77cf5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77cf5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77cf5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77cf5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77cf5-116">Not supported.</span></span>|
|<span data-ttu-id="77cf5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77cf5-117">Application</span></span>|<span data-ttu-id="77cf5-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77cf5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77cf5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77cf5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77cf5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="77cf5-120">Request headers</span></span>
|<span data-ttu-id="77cf5-121">标头</span><span class="sxs-lookup"><span data-stu-id="77cf5-121">Header</span></span>|<span data-ttu-id="77cf5-122">值</span><span class="sxs-lookup"><span data-stu-id="77cf5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77cf5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77cf5-123">Authorization</span></span>|<span data-ttu-id="77cf5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77cf5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77cf5-125">接受</span><span class="sxs-lookup"><span data-stu-id="77cf5-125">Accept</span></span>|<span data-ttu-id="77cf5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77cf5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77cf5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77cf5-127">Request body</span></span>
<span data-ttu-id="77cf5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77cf5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77cf5-129">响应</span><span class="sxs-lookup"><span data-stu-id="77cf5-129">Response</span></span>
<span data-ttu-id="77cf5-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77cf5-130">If successful, this method returns a `200 OK` response code and a collection of [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77cf5-131">示例</span><span class="sxs-lookup"><span data-stu-id="77cf5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77cf5-132">请求</span><span class="sxs-lookup"><span data-stu-id="77cf5-132">Request</span></span>
<span data-ttu-id="77cf5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77cf5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="77cf5-134">响应</span><span class="sxs-lookup"><span data-stu-id="77cf5-134">Response</span></span>
<span data-ttu-id="77cf5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77cf5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1823

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
      "id": "471203fb-03fb-4712-fb03-1247fb031247",
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
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```




