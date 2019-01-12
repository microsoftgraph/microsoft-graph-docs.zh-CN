---
title: 获取 deviceManagementPartner
description: 读取 deviceManagementPartner 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bd08b5dd189d9f21871ba7a5f1f3b6ecdda969b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950009"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="cdc67-103">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="cdc67-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="cdc67-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cdc67-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdc67-105">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cdc67-105">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdc67-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cdc67-106">Prerequisites</span></span>
<span data-ttu-id="cdc67-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cdc67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc67-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdc67-109">Permission type</span></span>|<span data-ttu-id="cdc67-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cdc67-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc67-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdc67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdc67-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdc67-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cdc67-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdc67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdc67-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdc67-114">Not supported.</span></span>|
|<span data-ttu-id="cdc67-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdc67-115">Application</span></span>|<span data-ttu-id="cdc67-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdc67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdc67-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdc67-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdc67-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cdc67-118">Optional query parameters</span></span>
<span data-ttu-id="cdc67-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cdc67-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdc67-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdc67-120">Request headers</span></span>
|<span data-ttu-id="cdc67-121">标头</span><span class="sxs-lookup"><span data-stu-id="cdc67-121">Header</span></span>|<span data-ttu-id="cdc67-122">值</span><span class="sxs-lookup"><span data-stu-id="cdc67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdc67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdc67-123">Authorization</span></span>|<span data-ttu-id="cdc67-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cdc67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdc67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdc67-125">Accept</span></span>|<span data-ttu-id="cdc67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdc67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc67-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdc67-127">Request body</span></span>
<span data-ttu-id="cdc67-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdc67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc67-129">响应</span><span class="sxs-lookup"><span data-stu-id="cdc67-129">Response</span></span>
<span data-ttu-id="cdc67-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cdc67-130">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc67-131">示例</span><span class="sxs-lookup"><span data-stu-id="cdc67-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdc67-132">请求</span><span class="sxs-lookup"><span data-stu-id="cdc67-132">Request</span></span>
<span data-ttu-id="cdc67-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdc67-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="cdc67-134">响应</span><span class="sxs-lookup"><span data-stu-id="cdc67-134">Response</span></span>
<span data-ttu-id="cdc67-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdc67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
  }
}
```



