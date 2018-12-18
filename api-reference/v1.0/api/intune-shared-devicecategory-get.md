---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: c69e3ecf97889636dd00deab213caf116233f6b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309696"
---
# <a name="get-devicecategory"></a><span data-ttu-id="7febe-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7febe-103">Get deviceCategory</span></span>



> <span data-ttu-id="7febe-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7febe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7febe-105">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7febe-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7febe-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7febe-106">Prerequisites</span></span>
<span data-ttu-id="7febe-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7febe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7febe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7febe-109">Permission type</span></span>|<span data-ttu-id="7febe-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7febe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7febe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7febe-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7febe-112">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="7febe-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7febe-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7febe-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="7febe-114">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="7febe-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7febe-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7febe-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7febe-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7febe-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7febe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7febe-117">Not supported.</span></span>|
|<span data-ttu-id="7febe-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7febe-118">Application</span></span>|<span data-ttu-id="7febe-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7febe-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7febe-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7febe-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7febe-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7febe-121">Optional query parameters</span></span>
<span data-ttu-id="7febe-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7febe-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7febe-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7febe-123">Request headers</span></span>
|<span data-ttu-id="7febe-124">标头</span><span class="sxs-lookup"><span data-stu-id="7febe-124">Header</span></span>|<span data-ttu-id="7febe-125">值</span><span class="sxs-lookup"><span data-stu-id="7febe-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7febe-126">授权</span><span class="sxs-lookup"><span data-stu-id="7febe-126">Authorization</span></span>|<span data-ttu-id="7febe-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7febe-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7febe-128">Accept</span><span class="sxs-lookup"><span data-stu-id="7febe-128">Accept</span></span>|<span data-ttu-id="7febe-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7febe-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7febe-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7febe-130">Request body</span></span>
<span data-ttu-id="7febe-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7febe-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7febe-132">响应</span><span class="sxs-lookup"><span data-stu-id="7febe-132">Response</span></span>
<span data-ttu-id="7febe-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7febe-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7febe-134">示例</span><span class="sxs-lookup"><span data-stu-id="7febe-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7febe-135">请求</span><span class="sxs-lookup"><span data-stu-id="7febe-135">Request</span></span>
<span data-ttu-id="7febe-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7febe-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="7febe-137">响应</span><span class="sxs-lookup"><span data-stu-id="7febe-137">Response</span></span>
<span data-ttu-id="7febe-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7febe-138">Here is an example of the response.</span></span> <span data-ttu-id="7febe-139">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7febe-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7febe-140">从实际的调用返回的属性有所不同根据上下文。</span><span class="sxs-lookup"><span data-stu-id="7febe-140">Properties returned from an actual call vary according to context.</span></span>

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



