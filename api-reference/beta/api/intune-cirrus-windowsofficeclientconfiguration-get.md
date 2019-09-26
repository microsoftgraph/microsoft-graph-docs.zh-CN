---
title: 获取 windowsOfficeClientConfiguration
description: 获取特定的非安全策略 windowsOfficeClientConfiguration 对象。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ad1578810511e951a07343e3df35d2ff6db0b10
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170747"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="90de2-103">获取 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="90de2-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="90de2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90de2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90de2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90de2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90de2-106">获取特定的非安全策略[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90de2-106">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90de2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="90de2-107">Prerequisites</span></span>
<span data-ttu-id="90de2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90de2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90de2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90de2-110">Permission type</span></span>|<span data-ttu-id="90de2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90de2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90de2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90de2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90de2-113">Devicemanagementconfiguration.readwrite.all 的所有 Devicemanagementconfiguration.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="90de2-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90de2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90de2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90de2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90de2-115">Not supported.</span></span>|
|<span data-ttu-id="90de2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="90de2-116">Application</span></span>|<span data-ttu-id="90de2-117">Devicemanagementconfiguration.readwrite.all 的所有 Devicemanagementconfiguration.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="90de2-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90de2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90de2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90de2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90de2-119">Optional query parameters</span></span>
<span data-ttu-id="90de2-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="90de2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90de2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="90de2-121">Request headers</span></span>
|<span data-ttu-id="90de2-122">标头</span><span class="sxs-lookup"><span data-stu-id="90de2-122">Header</span></span>|<span data-ttu-id="90de2-123">值</span><span class="sxs-lookup"><span data-stu-id="90de2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90de2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="90de2-124">Authorization</span></span>|<span data-ttu-id="90de2-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90de2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90de2-126">接受</span><span class="sxs-lookup"><span data-stu-id="90de2-126">Accept</span></span>|<span data-ttu-id="90de2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="90de2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90de2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="90de2-128">Request body</span></span>
<span data-ttu-id="90de2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90de2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90de2-130">响应</span><span class="sxs-lookup"><span data-stu-id="90de2-130">Response</span></span>
<span data-ttu-id="90de2-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90de2-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90de2-132">示例</span><span class="sxs-lookup"><span data-stu-id="90de2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="90de2-133">请求</span><span class="sxs-lookup"><span data-stu-id="90de2-133">Request</span></span>
<span data-ttu-id="90de2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90de2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="90de2-135">响应</span><span class="sxs-lookup"><span data-stu-id="90de2-135">Response</span></span>
<span data-ttu-id="90de2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90de2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
    "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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




