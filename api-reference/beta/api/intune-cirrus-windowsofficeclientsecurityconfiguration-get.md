---
title: 获取 windowsOfficeClientSecurityConfiguration
description: 获取特定安全策略 windowsOfficeClientSecurityConfiguration 对象。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adaad0a5a43e415a17c21218272b98afe3a502ec
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666820"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="7f98a-103">获取 windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f98a-103">Get windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="7f98a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f98a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f98a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f98a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f98a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f98a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f98a-107">获取特定安全策略 [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f98a-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f98a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f98a-108">Prerequisites</span></span>
<span data-ttu-id="7f98a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f98a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f98a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f98a-111">Permission type</span></span>|<span data-ttu-id="7f98a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f98a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f98a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f98a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f98a-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f98a-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f98a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f98a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f98a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f98a-116">Not supported.</span></span>|
|<span data-ttu-id="7f98a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f98a-117">Application</span></span>|<span data-ttu-id="7f98a-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f98a-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f98a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f98a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f98a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f98a-120">Optional query parameters</span></span>
<span data-ttu-id="7f98a-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f98a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f98a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f98a-122">Request headers</span></span>
|<span data-ttu-id="7f98a-123">标头</span><span class="sxs-lookup"><span data-stu-id="7f98a-123">Header</span></span>|<span data-ttu-id="7f98a-124">值</span><span class="sxs-lookup"><span data-stu-id="7f98a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f98a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f98a-125">Authorization</span></span>|<span data-ttu-id="7f98a-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f98a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f98a-127">接受</span><span class="sxs-lookup"><span data-stu-id="7f98a-127">Accept</span></span>|<span data-ttu-id="7f98a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f98a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f98a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f98a-129">Request body</span></span>
<span data-ttu-id="7f98a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f98a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f98a-131">响应</span><span class="sxs-lookup"><span data-stu-id="7f98a-131">Response</span></span>
<span data-ttu-id="7f98a-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f98a-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f98a-133">示例</span><span class="sxs-lookup"><span data-stu-id="7f98a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f98a-134">请求</span><span class="sxs-lookup"><span data-stu-id="7f98a-134">Request</span></span>
<span data-ttu-id="7f98a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f98a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="7f98a-136">响应</span><span class="sxs-lookup"><span data-stu-id="7f98a-136">Response</span></span>
<span data-ttu-id="7f98a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f98a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




