---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a158ca444c631e8797ab3f3ce2ec95f525f0f1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512095"
---
# <a name="get-devicecategory"></a><span data-ttu-id="6184f-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6184f-103">Get deviceCategory</span></span>

<span data-ttu-id="6184f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6184f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6184f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6184f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6184f-106">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6184f-106">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6184f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6184f-107">Prerequisites</span></span>
<span data-ttu-id="6184f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6184f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6184f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6184f-110">Permission type</span></span>|<span data-ttu-id="6184f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6184f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6184f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6184f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6184f-113">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6184f-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6184f-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6184f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6184f-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="6184f-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6184f-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6184f-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6184f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6184f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6184f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6184f-118">Not supported.</span></span>|
|<span data-ttu-id="6184f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6184f-119">Application</span></span>|<span data-ttu-id="6184f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6184f-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6184f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6184f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6184f-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6184f-122">Optional query parameters</span></span>
<span data-ttu-id="6184f-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6184f-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6184f-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6184f-124">Request headers</span></span>
|<span data-ttu-id="6184f-125">标头</span><span class="sxs-lookup"><span data-stu-id="6184f-125">Header</span></span>|<span data-ttu-id="6184f-126">值</span><span class="sxs-lookup"><span data-stu-id="6184f-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6184f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6184f-127">Authorization</span></span>|<span data-ttu-id="6184f-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6184f-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6184f-129">接受</span><span class="sxs-lookup"><span data-stu-id="6184f-129">Accept</span></span>|<span data-ttu-id="6184f-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6184f-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6184f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6184f-131">Request body</span></span>
<span data-ttu-id="6184f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6184f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6184f-133">响应</span><span class="sxs-lookup"><span data-stu-id="6184f-133">Response</span></span>
<span data-ttu-id="6184f-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6184f-134">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6184f-135">示例</span><span class="sxs-lookup"><span data-stu-id="6184f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="6184f-136">请求</span><span class="sxs-lookup"><span data-stu-id="6184f-136">Request</span></span>
<span data-ttu-id="6184f-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6184f-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="6184f-138">响应</span><span class="sxs-lookup"><span data-stu-id="6184f-138">Response</span></span>
<span data-ttu-id="6184f-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6184f-139">Here is an example of the response.</span></span> <span data-ttu-id="6184f-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6184f-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6184f-141">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="6184f-141">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```




