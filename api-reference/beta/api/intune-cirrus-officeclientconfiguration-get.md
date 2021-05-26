---
title: 获取 officeClientConfiguration
description: 获取特定策略。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3b4a2f582d093798145d971936ac3510813ccb0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665713"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="a136a-103">获取 officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="a136a-103">Get officeClientConfiguration</span></span>

<span data-ttu-id="a136a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a136a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a136a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a136a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a136a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a136a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a136a-107">获取特定策略。</span><span class="sxs-lookup"><span data-stu-id="a136a-107">Get a specific policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a136a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a136a-108">Prerequisites</span></span>
<span data-ttu-id="a136a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a136a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a136a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a136a-111">Permission type</span></span>|<span data-ttu-id="a136a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a136a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a136a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a136a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a136a-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a136a-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a136a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a136a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a136a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a136a-116">Not supported.</span></span>|
|<span data-ttu-id="a136a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a136a-117">Application</span></span>|<span data-ttu-id="a136a-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a136a-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a136a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a136a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a136a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a136a-120">Optional query parameters</span></span>
<span data-ttu-id="a136a-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a136a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a136a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a136a-122">Request headers</span></span>
|<span data-ttu-id="a136a-123">标头</span><span class="sxs-lookup"><span data-stu-id="a136a-123">Header</span></span>|<span data-ttu-id="a136a-124">值</span><span class="sxs-lookup"><span data-stu-id="a136a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a136a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a136a-125">Authorization</span></span>|<span data-ttu-id="a136a-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a136a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a136a-127">接受</span><span class="sxs-lookup"><span data-stu-id="a136a-127">Accept</span></span>|<span data-ttu-id="a136a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a136a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a136a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a136a-129">Request body</span></span>
<span data-ttu-id="a136a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a136a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a136a-131">响应</span><span class="sxs-lookup"><span data-stu-id="a136a-131">Response</span></span>
<span data-ttu-id="a136a-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a136a-132">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a136a-133">示例</span><span class="sxs-lookup"><span data-stu-id="a136a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a136a-134">请求</span><span class="sxs-lookup"><span data-stu-id="a136a-134">Request</span></span>
<span data-ttu-id="a136a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a136a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="a136a-136">响应</span><span class="sxs-lookup"><span data-stu-id="a136a-136">Response</span></span>
<span data-ttu-id="a136a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a136a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfiguration",
    "id": "362ce0f0-e0f0-362c-f0e0-2c36f0e02c36",
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




