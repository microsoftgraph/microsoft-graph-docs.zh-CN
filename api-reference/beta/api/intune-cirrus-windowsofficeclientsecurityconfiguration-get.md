---
title: 获取 windowsOfficeClientSecurityConfiguration
description: 获取特定的安全策略 windowsOfficeClientSecurityConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a1619e7e1ed30afbc6b04f168f8e1fda2456e749
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409571"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="9dbca-103">获取 windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="9dbca-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="9dbca-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9dbca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9dbca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9dbca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dbca-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9dbca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dbca-107">获取特定的安全策略[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9dbca-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dbca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9dbca-108">Prerequisites</span></span>
<span data-ttu-id="9dbca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dbca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dbca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dbca-111">Permission type</span></span>|<span data-ttu-id="9dbca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9dbca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dbca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dbca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9dbca-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9dbca-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9dbca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dbca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dbca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dbca-116">Not supported.</span></span>|
|<span data-ttu-id="9dbca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dbca-117">Application</span></span>|<span data-ttu-id="9dbca-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dbca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dbca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dbca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9dbca-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9dbca-120">Optional query parameters</span></span>
<span data-ttu-id="9dbca-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9dbca-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9dbca-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dbca-122">Request headers</span></span>
|<span data-ttu-id="9dbca-123">标头</span><span class="sxs-lookup"><span data-stu-id="9dbca-123">Header</span></span>|<span data-ttu-id="9dbca-124">值</span><span class="sxs-lookup"><span data-stu-id="9dbca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dbca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dbca-125">Authorization</span></span>|<span data-ttu-id="9dbca-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9dbca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dbca-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9dbca-127">Accept</span></span>|<span data-ttu-id="9dbca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9dbca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dbca-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dbca-129">Request body</span></span>
<span data-ttu-id="9dbca-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9dbca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dbca-131">响应</span><span class="sxs-lookup"><span data-stu-id="9dbca-131">Response</span></span>
<span data-ttu-id="9dbca-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9dbca-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dbca-133">示例</span><span class="sxs-lookup"><span data-stu-id="9dbca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dbca-134">请求</span><span class="sxs-lookup"><span data-stu-id="9dbca-134">Request</span></span>
<span data-ttu-id="9dbca-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9dbca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="9dbca-136">响应</span><span class="sxs-lookup"><span data-stu-id="9dbca-136">Response</span></span>
<span data-ttu-id="9dbca-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9dbca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
    "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
    "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
    "policyPayload": "<Unknown Primitive Type Edm.Stream>",
    "description": "Description value",
    "displayName": "Display Name value",
    "priority": 8,
    "userCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    },
    "checkinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "userId": "User Id value",
        "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ]
      }
    ]
  }
}
```



