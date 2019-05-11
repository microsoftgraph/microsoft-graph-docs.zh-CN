---
title: 列出 officeClientConfigurations
description: 获取所有策略。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 093364b093606153fd82c18791a86ff441291d56
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934066"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="2f543-103">列出 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="2f543-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="2f543-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f543-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f543-106">获取所有策略。</span><span class="sxs-lookup"><span data-stu-id="2f543-106">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f543-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f543-107">Prerequisites</span></span>
<span data-ttu-id="2f543-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f543-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f543-110">Permission type</span></span>|<span data-ttu-id="2f543-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f543-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f543-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f543-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f543-113">Devicemanagementconfiguration.readwrite.all 的所有 Devicemanagementconfiguration.readwrite.all</span><span class="sxs-lookup"><span data-stu-id="2f543-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2f543-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f543-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f543-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f543-115">Not supported.</span></span>|
|<span data-ttu-id="2f543-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f543-116">Application</span></span>|<span data-ttu-id="2f543-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f543-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f543-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f543-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f543-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f543-119">Request headers</span></span>
|<span data-ttu-id="2f543-120">标头</span><span class="sxs-lookup"><span data-stu-id="2f543-120">Header</span></span>|<span data-ttu-id="2f543-121">值</span><span class="sxs-lookup"><span data-stu-id="2f543-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f543-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f543-122">Authorization</span></span>|<span data-ttu-id="2f543-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f543-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f543-124">接受</span><span class="sxs-lookup"><span data-stu-id="2f543-124">Accept</span></span>|<span data-ttu-id="2f543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f543-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f543-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f543-126">Request body</span></span>
<span data-ttu-id="2f543-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f543-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f543-128">响应</span><span class="sxs-lookup"><span data-stu-id="2f543-128">Response</span></span>
<span data-ttu-id="2f543-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2f543-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f543-130">示例</span><span class="sxs-lookup"><span data-stu-id="2f543-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f543-131">请求</span><span class="sxs-lookup"><span data-stu-id="2f543-131">Request</span></span>
<span data-ttu-id="2f543-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f543-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="2f543-133">响应</span><span class="sxs-lookup"><span data-stu-id="2f543-133">Response</span></span>
<span data-ttu-id="2f543-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f543-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1207

{
  "value": [
    {
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
  ]
}
```



