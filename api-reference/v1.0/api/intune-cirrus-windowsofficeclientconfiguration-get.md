---
title: 获取 windowsOfficeClientConfiguration
description: 获取特定的非安全策略 windowsOfficeClientConfiguration 对象。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53238bdb656967ccc3e230532270057d1cb5f07c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751763"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="02e02-103">获取 windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="02e02-103">Get windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="02e02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02e02-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02e02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02e02-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02e02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e02-107">获取特定的非安全策略 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02e02-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02e02-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="02e02-108">Prerequisites</span></span>
<span data-ttu-id="02e02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e02-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02e02-111">Permission type</span></span>|<span data-ttu-id="02e02-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02e02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e02-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02e02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02e02-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e02-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="02e02-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02e02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e02-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02e02-116">Not supported.</span></span>|
|<span data-ttu-id="02e02-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02e02-117">Application</span></span>|<span data-ttu-id="02e02-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e02-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e02-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02e02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02e02-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="02e02-120">Optional query parameters</span></span>
<span data-ttu-id="02e02-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="02e02-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02e02-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="02e02-122">Request headers</span></span>
|<span data-ttu-id="02e02-123">标头</span><span class="sxs-lookup"><span data-stu-id="02e02-123">Header</span></span>|<span data-ttu-id="02e02-124">值</span><span class="sxs-lookup"><span data-stu-id="02e02-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e02-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="02e02-125">Authorization</span></span>|<span data-ttu-id="02e02-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02e02-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e02-127">接受</span><span class="sxs-lookup"><span data-stu-id="02e02-127">Accept</span></span>|<span data-ttu-id="02e02-128">application/json</span><span class="sxs-lookup"><span data-stu-id="02e02-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e02-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="02e02-129">Request body</span></span>
<span data-ttu-id="02e02-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02e02-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02e02-131">响应</span><span class="sxs-lookup"><span data-stu-id="02e02-131">Response</span></span>
<span data-ttu-id="02e02-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02e02-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e02-133">示例</span><span class="sxs-lookup"><span data-stu-id="02e02-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e02-134">请求</span><span class="sxs-lookup"><span data-stu-id="02e02-134">Request</span></span>
<span data-ttu-id="02e02-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02e02-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="02e02-136">响应</span><span class="sxs-lookup"><span data-stu-id="02e02-136">Response</span></span>
<span data-ttu-id="02e02-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02e02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




