---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
ms.openlocfilehash: 89b8f46aae22c87ea1462cc70eeb3e28e9bfa230
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010936"
---
# <a name="get-devicecategory"></a><span data-ttu-id="71d27-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="71d27-103">Get deviceCategory</span></span>



> <span data-ttu-id="71d27-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="71d27-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71d27-105">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71d27-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d27-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="71d27-106">Prerequisites</span></span>
<span data-ttu-id="71d27-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="71d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71d27-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="71d27-109">Permission type</span></span>|<span data-ttu-id="71d27-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71d27-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d27-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71d27-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="71d27-112">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="71d27-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="71d27-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="71d27-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="71d27-114">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="71d27-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="71d27-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="71d27-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="71d27-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71d27-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d27-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71d27-117">Not supported.</span></span>|
|<span data-ttu-id="71d27-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="71d27-118">Application</span></span>|<span data-ttu-id="71d27-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="71d27-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d27-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71d27-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71d27-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71d27-121">Optional query parameters</span></span>
<span data-ttu-id="71d27-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="71d27-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71d27-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="71d27-123">Request headers</span></span>
|<span data-ttu-id="71d27-124">标头</span><span class="sxs-lookup"><span data-stu-id="71d27-124">Header</span></span>|<span data-ttu-id="71d27-125">值</span><span class="sxs-lookup"><span data-stu-id="71d27-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d27-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="71d27-126">Authorization</span></span>|<span data-ttu-id="71d27-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71d27-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d27-128">Accept</span><span class="sxs-lookup"><span data-stu-id="71d27-128">Accept</span></span>|<span data-ttu-id="71d27-129">application/json</span><span class="sxs-lookup"><span data-stu-id="71d27-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d27-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="71d27-130">Request body</span></span>
<span data-ttu-id="71d27-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71d27-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71d27-132">响应</span><span class="sxs-lookup"><span data-stu-id="71d27-132">Response</span></span>
<span data-ttu-id="71d27-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71d27-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d27-134">示例</span><span class="sxs-lookup"><span data-stu-id="71d27-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d27-135">请求</span><span class="sxs-lookup"><span data-stu-id="71d27-135">Request</span></span>
<span data-ttu-id="71d27-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71d27-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="71d27-137">响应</span><span class="sxs-lookup"><span data-stu-id="71d27-137">Response</span></span>
<span data-ttu-id="71d27-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71d27-138">Here is an example of the response.</span></span> <span data-ttu-id="71d27-139">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="71d27-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="71d27-140">从实际的调用返回的属性有所不同根据上下文。</span><span class="sxs-lookup"><span data-stu-id="71d27-140">Properties returned from an actual call vary according to context.</span></span>

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



