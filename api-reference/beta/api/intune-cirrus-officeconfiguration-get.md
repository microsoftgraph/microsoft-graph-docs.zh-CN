---
title: 获取 officeConfiguration
description: 读取 officeConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f215b5d369b42e72efb0847c2e2c9360b4f98cb1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725885"
---
# <a name="get-officeconfiguration"></a><span data-ttu-id="d03ad-103">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d03ad-103">Get officeConfiguration</span></span>

> <span data-ttu-id="d03ad-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d03ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d03ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d03ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d03ad-106">读取[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d03ad-106">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d03ad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d03ad-107">Prerequisites</span></span>
<span data-ttu-id="d03ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d03ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d03ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d03ad-110">Permission type</span></span>|<span data-ttu-id="d03ad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d03ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d03ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d03ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d03ad-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d03ad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d03ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d03ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d03ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d03ad-115">Not supported.</span></span>|
|<span data-ttu-id="d03ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d03ad-116">Application</span></span>|<span data-ttu-id="d03ad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d03ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d03ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d03ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d03ad-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d03ad-119">Optional query parameters</span></span>
<span data-ttu-id="d03ad-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d03ad-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d03ad-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d03ad-121">Request headers</span></span>
|<span data-ttu-id="d03ad-122">标头</span><span class="sxs-lookup"><span data-stu-id="d03ad-122">Header</span></span>|<span data-ttu-id="d03ad-123">值</span><span class="sxs-lookup"><span data-stu-id="d03ad-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d03ad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d03ad-124">Authorization</span></span>|<span data-ttu-id="d03ad-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d03ad-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d03ad-126">接受</span><span class="sxs-lookup"><span data-stu-id="d03ad-126">Accept</span></span>|<span data-ttu-id="d03ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d03ad-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d03ad-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d03ad-128">Request body</span></span>
<span data-ttu-id="d03ad-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d03ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d03ad-130">响应</span><span class="sxs-lookup"><span data-stu-id="d03ad-130">Response</span></span>
<span data-ttu-id="d03ad-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d03ad-131">If successful, this method returns a `200 OK` response code and [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d03ad-132">示例</span><span class="sxs-lookup"><span data-stu-id="d03ad-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d03ad-133">请求</span><span class="sxs-lookup"><span data-stu-id="d03ad-133">Request</span></span>
<span data-ttu-id="d03ad-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d03ad-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration
```

### <a name="response"></a><span data-ttu-id="d03ad-135">响应</span><span class="sxs-lookup"><span data-stu-id="d03ad-135">Response</span></span>
<span data-ttu-id="d03ad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d03ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 959

{
  "value": {
    "@odata.type": "#microsoft.graph.officeConfiguration",
    "id": "4b5f7085-7085-4b5f-8570-5f4b85705f4b",
    "tenantCheckinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userId": "User Id value",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ],
        "lastTaskName": "Last Task Name value"
      }
    ],
    "tenantUserCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    }
  }
}
```





