---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3978378e3ea962636fb53dc2187a1ca69c83eff
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086226"
---
# <a name="get-devicecategory"></a><span data-ttu-id="78aea-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="78aea-103">Get deviceCategory</span></span>

> <span data-ttu-id="78aea-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="78aea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78aea-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="78aea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78aea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78aea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78aea-107">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78aea-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78aea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="78aea-108">Prerequisites</span></span>

<span data-ttu-id="78aea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78aea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78aea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="78aea-111">Permission type</span></span>|<span data-ttu-id="78aea-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78aea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78aea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78aea-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="78aea-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="78aea-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="78aea-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78aea-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="78aea-116">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="78aea-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="78aea-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78aea-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="78aea-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78aea-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78aea-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="78aea-119">Not supported.</span></span>|
|<span data-ttu-id="78aea-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="78aea-120">Application</span></span>||
| <span data-ttu-id="78aea-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="78aea-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="78aea-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78aea-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="78aea-123">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="78aea-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="78aea-124">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="78aea-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78aea-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78aea-125">HTTP Request</span></span>

<span data-ttu-id="78aea-126">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="78aea-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="78aea-127">**载入**</span><span class="sxs-lookup"><span data-stu-id="78aea-127">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78aea-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78aea-128">Optional query parameters</span></span>

<span data-ttu-id="78aea-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="78aea-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78aea-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="78aea-130">Request headers</span></span>

|<span data-ttu-id="78aea-131">标头</span><span class="sxs-lookup"><span data-stu-id="78aea-131">Header</span></span>|<span data-ttu-id="78aea-132">值</span><span class="sxs-lookup"><span data-stu-id="78aea-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78aea-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="78aea-133">Authorization</span></span>|<span data-ttu-id="78aea-134">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78aea-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78aea-135">接受</span><span class="sxs-lookup"><span data-stu-id="78aea-135">Accept</span></span>|<span data-ttu-id="78aea-136">application/json</span><span class="sxs-lookup"><span data-stu-id="78aea-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78aea-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="78aea-137">Request body</span></span>

<span data-ttu-id="78aea-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78aea-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78aea-139">响应</span><span class="sxs-lookup"><span data-stu-id="78aea-139">Response</span></span>

<span data-ttu-id="78aea-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78aea-140">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78aea-141">示例</span><span class="sxs-lookup"><span data-stu-id="78aea-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="78aea-142">请求</span><span class="sxs-lookup"><span data-stu-id="78aea-142">Request</span></span>

<span data-ttu-id="78aea-143">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="78aea-143">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="78aea-144">响应</span><span class="sxs-lookup"><span data-stu-id="78aea-144">Response</span></span>

<span data-ttu-id="78aea-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78aea-145">Here is an example of the response.</span></span> <span data-ttu-id="78aea-146">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="78aea-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="78aea-147">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="78aea-147">Properties returned from an actual call vary according to context.</span></span>

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












