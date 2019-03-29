---
title: 列出 deviceManagementPartners
description: 列出 deviceManagementPartner 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aa405a500d1d4cfd1ceeca5695fdd405667d571
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969713"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="e829a-103">列出 deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="e829a-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="e829a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e829a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e829a-105">列出 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e829a-105">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e829a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e829a-106">Prerequisites</span></span>
<span data-ttu-id="e829a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e829a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e829a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e829a-109">Permission type</span></span>|<span data-ttu-id="e829a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e829a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e829a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e829a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e829a-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e829a-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e829a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e829a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e829a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e829a-114">Not supported.</span></span>|
|<span data-ttu-id="e829a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e829a-115">Application</span></span>|<span data-ttu-id="e829a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e829a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e829a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e829a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e829a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e829a-118">Request headers</span></span>
|<span data-ttu-id="e829a-119">标头</span><span class="sxs-lookup"><span data-stu-id="e829a-119">Header</span></span>|<span data-ttu-id="e829a-120">值</span><span class="sxs-lookup"><span data-stu-id="e829a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e829a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e829a-121">Authorization</span></span>|<span data-ttu-id="e829a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e829a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e829a-123">接受</span><span class="sxs-lookup"><span data-stu-id="e829a-123">Accept</span></span>|<span data-ttu-id="e829a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e829a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e829a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e829a-125">Request body</span></span>
<span data-ttu-id="e829a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e829a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e829a-127">响应</span><span class="sxs-lookup"><span data-stu-id="e829a-127">Response</span></span>
<span data-ttu-id="e829a-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e829a-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e829a-129">示例</span><span class="sxs-lookup"><span data-stu-id="e829a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e829a-130">请求</span><span class="sxs-lookup"><span data-stu-id="e829a-130">Request</span></span>
<span data-ttu-id="e829a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e829a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="e829a-132">响应</span><span class="sxs-lookup"><span data-stu-id="e829a-132">Response</span></span>
<span data-ttu-id="e829a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e829a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
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
  ]
}
```



