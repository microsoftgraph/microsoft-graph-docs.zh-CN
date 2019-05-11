---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c65c06e13067b3ba299e0e6ca4fe15584667c99b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899296"
---
# <a name="get-devicecategory"></a><span data-ttu-id="fbfe2-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbfe2-103">Get deviceCategory</span></span>

> <span data-ttu-id="fbfe2-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbfe2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbfe2-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbfe2-107">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbfe2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbfe2-108">Prerequisites</span></span>

<span data-ttu-id="fbfe2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbfe2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbfe2-111">Permission type</span></span>|<span data-ttu-id="fbfe2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbfe2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbfe2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbfe2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fbfe2-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="fbfe2-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fbfe2-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbfe2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="fbfe2-116">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="fbfe2-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fbfe2-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbfe2-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fbfe2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbfe2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbfe2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-119">Not supported.</span></span>|
|<span data-ttu-id="fbfe2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbfe2-120">Application</span></span>|<span data-ttu-id="fbfe2-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbfe2-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbfe2-122">HTTP Request</span></span>

<span data-ttu-id="fbfe2-123">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="fbfe2-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="fbfe2-124">**载入**</span><span class="sxs-lookup"><span data-stu-id="fbfe2-124">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbfe2-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fbfe2-125">Optional query parameters</span></span>

<span data-ttu-id="fbfe2-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbfe2-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbfe2-127">Request headers</span></span>

|<span data-ttu-id="fbfe2-128">标头</span><span class="sxs-lookup"><span data-stu-id="fbfe2-128">Header</span></span>|<span data-ttu-id="fbfe2-129">值</span><span class="sxs-lookup"><span data-stu-id="fbfe2-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbfe2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbfe2-130">Authorization</span></span>|<span data-ttu-id="fbfe2-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbfe2-132">接受</span><span class="sxs-lookup"><span data-stu-id="fbfe2-132">Accept</span></span>|<span data-ttu-id="fbfe2-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fbfe2-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbfe2-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbfe2-134">Request body</span></span>

<span data-ttu-id="fbfe2-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbfe2-136">响应</span><span class="sxs-lookup"><span data-stu-id="fbfe2-136">Response</span></span>

<span data-ttu-id="fbfe2-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-137">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbfe2-138">示例</span><span class="sxs-lookup"><span data-stu-id="fbfe2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbfe2-139">请求</span><span class="sxs-lookup"><span data-stu-id="fbfe2-139">Request</span></span>

<span data-ttu-id="fbfe2-140">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-140">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="fbfe2-141">响应</span><span class="sxs-lookup"><span data-stu-id="fbfe2-141">Response</span></span>

<span data-ttu-id="fbfe2-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-142">Here is an example of the response.</span></span> <span data-ttu-id="fbfe2-143">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fbfe2-144">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="fbfe2-144">Properties returned from an actual call vary according to context.</span></span>

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



