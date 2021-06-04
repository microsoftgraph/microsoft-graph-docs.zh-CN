---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e371567d984285365fcadb6c2304a560638d0a04
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732270"
---
# <a name="get-devicecategory"></a><span data-ttu-id="78e63-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="78e63-103">Get deviceCategory</span></span>

<span data-ttu-id="78e63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78e63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e63-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78e63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e63-106">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78e63-106">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e63-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="78e63-107">Prerequisites</span></span>
<span data-ttu-id="78e63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e63-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="78e63-110">Permission type</span></span>|<span data-ttu-id="78e63-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78e63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e63-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78e63-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="78e63-113">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="78e63-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="78e63-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78e63-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="78e63-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="78e63-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="78e63-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78e63-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="78e63-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78e63-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e63-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e63-118">Not supported.</span></span>|
|<span data-ttu-id="78e63-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="78e63-119">Application</span></span>|<span data-ttu-id="78e63-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e63-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e63-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78e63-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78e63-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78e63-122">Optional query parameters</span></span>
<span data-ttu-id="78e63-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="78e63-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78e63-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="78e63-124">Request headers</span></span>
|<span data-ttu-id="78e63-125">标头</span><span class="sxs-lookup"><span data-stu-id="78e63-125">Header</span></span>|<span data-ttu-id="78e63-126">值</span><span class="sxs-lookup"><span data-stu-id="78e63-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e63-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="78e63-127">Authorization</span></span>|<span data-ttu-id="78e63-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78e63-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e63-129">接受</span><span class="sxs-lookup"><span data-stu-id="78e63-129">Accept</span></span>|<span data-ttu-id="78e63-130">application/json</span><span class="sxs-lookup"><span data-stu-id="78e63-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e63-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="78e63-131">Request body</span></span>
<span data-ttu-id="78e63-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78e63-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78e63-133">响应</span><span class="sxs-lookup"><span data-stu-id="78e63-133">Response</span></span>
<span data-ttu-id="78e63-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78e63-134">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e63-135">示例</span><span class="sxs-lookup"><span data-stu-id="78e63-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e63-136">请求</span><span class="sxs-lookup"><span data-stu-id="78e63-136">Request</span></span>
<span data-ttu-id="78e63-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78e63-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="78e63-138">响应</span><span class="sxs-lookup"><span data-stu-id="78e63-138">Response</span></span>
<span data-ttu-id="78e63-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78e63-139">Here is an example of the response.</span></span> <span data-ttu-id="78e63-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="78e63-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="78e63-141">从实际调用返回的属性因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="78e63-141">Properties returned from an actual call vary according to context.</span></span>

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