---
title: 列出 officeClientConfigurations
description: 获取所有策略。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50f9554377cd6e0b887f6fb6a1e9d5ea6aede3e5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665712"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="767a5-103">列出 officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="767a5-103">List officeClientConfigurations</span></span>

<span data-ttu-id="767a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="767a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="767a5-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="767a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="767a5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="767a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767a5-107">获取所有策略。</span><span class="sxs-lookup"><span data-stu-id="767a5-107">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="767a5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="767a5-108">Prerequisites</span></span>
<span data-ttu-id="767a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="767a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767a5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="767a5-111">Permission type</span></span>|<span data-ttu-id="767a5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="767a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="767a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="767a5-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="767a5-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="767a5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="767a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="767a5-116">Not supported.</span></span>|
|<span data-ttu-id="767a5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="767a5-117">Application</span></span>|<span data-ttu-id="767a5-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="767a5-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="767a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="767a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="767a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="767a5-120">Request headers</span></span>
|<span data-ttu-id="767a5-121">标头</span><span class="sxs-lookup"><span data-stu-id="767a5-121">Header</span></span>|<span data-ttu-id="767a5-122">值</span><span class="sxs-lookup"><span data-stu-id="767a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="767a5-123">Authorization</span></span>|<span data-ttu-id="767a5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="767a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767a5-125">接受</span><span class="sxs-lookup"><span data-stu-id="767a5-125">Accept</span></span>|<span data-ttu-id="767a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="767a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="767a5-127">Request body</span></span>
<span data-ttu-id="767a5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="767a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="767a5-129">响应</span><span class="sxs-lookup"><span data-stu-id="767a5-129">Response</span></span>
<span data-ttu-id="767a5-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="767a5-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767a5-131">示例</span><span class="sxs-lookup"><span data-stu-id="767a5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="767a5-132">请求</span><span class="sxs-lookup"><span data-stu-id="767a5-132">Request</span></span>
<span data-ttu-id="767a5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="767a5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="767a5-134">响应</span><span class="sxs-lookup"><span data-stu-id="767a5-134">Response</span></span>
<span data-ttu-id="767a5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="767a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




