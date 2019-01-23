---
title: 获取 windows10NetworkBoundaryConfiguration
description: 读取属性和 windows10NetworkBoundaryConfiguration 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 96cd710e496d04446cbb7e85d592b857f3081c71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401339"
---
# <a name="get-windows10networkboundaryconfiguration"></a><span data-ttu-id="2ef20-103">获取 windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ef20-103">Get windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="2ef20-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2ef20-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ef20-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2ef20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ef20-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ef20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ef20-107">读取属性和[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2ef20-107">Read properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ef20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ef20-108">Prerequisites</span></span>
<span data-ttu-id="2ef20-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2ef20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ef20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ef20-111">Permission type</span></span>|<span data-ttu-id="2ef20-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ef20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ef20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ef20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ef20-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ef20-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2ef20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ef20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ef20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ef20-116">Not supported.</span></span>|
|<span data-ttu-id="2ef20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ef20-117">Application</span></span>|<span data-ttu-id="2ef20-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ef20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ef20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ef20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ef20-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ef20-120">Optional query parameters</span></span>
<span data-ttu-id="2ef20-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ef20-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ef20-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ef20-122">Request headers</span></span>
|<span data-ttu-id="2ef20-123">标头</span><span class="sxs-lookup"><span data-stu-id="2ef20-123">Header</span></span>|<span data-ttu-id="2ef20-124">值</span><span class="sxs-lookup"><span data-stu-id="2ef20-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ef20-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ef20-125">Authorization</span></span>|<span data-ttu-id="2ef20-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ef20-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ef20-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2ef20-127">Accept</span></span>|<span data-ttu-id="2ef20-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef20-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef20-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ef20-129">Request body</span></span>
<span data-ttu-id="2ef20-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ef20-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ef20-131">响应</span><span class="sxs-lookup"><span data-stu-id="2ef20-131">Response</span></span>
<span data-ttu-id="2ef20-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ef20-132">If successful, this method returns a `200 OK` response code and [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef20-133">示例</span><span class="sxs-lookup"><span data-stu-id="2ef20-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ef20-134">请求</span><span class="sxs-lookup"><span data-stu-id="2ef20-134">Request</span></span>
<span data-ttu-id="2ef20-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ef20-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2ef20-136">响应</span><span class="sxs-lookup"><span data-stu-id="2ef20-136">Response</span></span>
<span data-ttu-id="2ef20-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ef20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1519

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
    "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "windowsNetworkIsolationPolicy": {
      "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
      "enterpriseNetworkDomainNames": [
        "Enterprise Network Domain Names value"
      ],
      "enterpriseCloudResources": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ],
      "enterpriseIPRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "enterpriseInternalProxyServers": [
        "Enterprise Internal Proxy Servers value"
      ],
      "enterpriseIPRangesAreAuthoritative": true,
      "enterpriseProxyServers": [
        "Enterprise Proxy Servers value"
      ],
      "enterpriseProxyServersAreAuthoritative": true,
      "neutralDomainResources": [
        "Neutral Domain Resources value"
      ]
    }
  }
}
```




