---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6153c384d0de170899e2cf684a9b10a0b986b84
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402392"
---
# <a name="get-devicecategory"></a><span data-ttu-id="7b4af-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7b4af-103">Get deviceCategory</span></span>

<span data-ttu-id="7b4af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b4af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b4af-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b4af-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b4af-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b4af-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b4af-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b4af-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b4af-108">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b4af-108">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b4af-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b4af-109">Prerequisites</span></span>

<span data-ttu-id="7b4af-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b4af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b4af-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b4af-112">Permission type</span></span>|<span data-ttu-id="7b4af-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b4af-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b4af-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b4af-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7b4af-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="7b4af-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7b4af-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b4af-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="7b4af-117">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="7b4af-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7b4af-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b4af-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7b4af-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b4af-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b4af-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b4af-120">Not supported.</span></span>|
|<span data-ttu-id="7b4af-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b4af-121">Application</span></span>||
| <span data-ttu-id="7b4af-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="7b4af-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7b4af-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b4af-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="7b4af-124">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="7b4af-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7b4af-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b4af-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b4af-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b4af-126">HTTP Request</span></span>

<span data-ttu-id="7b4af-127">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="7b4af-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="7b4af-128">**载入**</span><span class="sxs-lookup"><span data-stu-id="7b4af-128">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b4af-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b4af-129">Optional query parameters</span></span>

<span data-ttu-id="7b4af-130">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7b4af-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b4af-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b4af-131">Request headers</span></span>

|<span data-ttu-id="7b4af-132">标头</span><span class="sxs-lookup"><span data-stu-id="7b4af-132">Header</span></span>|<span data-ttu-id="7b4af-133">值</span><span class="sxs-lookup"><span data-stu-id="7b4af-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b4af-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b4af-134">Authorization</span></span>|<span data-ttu-id="7b4af-135">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b4af-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b4af-136">接受</span><span class="sxs-lookup"><span data-stu-id="7b4af-136">Accept</span></span>|<span data-ttu-id="7b4af-137">application/json</span><span class="sxs-lookup"><span data-stu-id="7b4af-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b4af-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b4af-138">Request body</span></span>

<span data-ttu-id="7b4af-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b4af-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b4af-140">响应</span><span class="sxs-lookup"><span data-stu-id="7b4af-140">Response</span></span>

<span data-ttu-id="7b4af-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b4af-141">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b4af-142">示例</span><span class="sxs-lookup"><span data-stu-id="7b4af-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b4af-143">请求</span><span class="sxs-lookup"><span data-stu-id="7b4af-143">Request</span></span>

<span data-ttu-id="7b4af-144">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="7b4af-144">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="7b4af-145">响应</span><span class="sxs-lookup"><span data-stu-id="7b4af-145">Response</span></span>

<span data-ttu-id="7b4af-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7b4af-146">Here is an example of the response.</span></span> <span data-ttu-id="7b4af-147">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b4af-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7b4af-148">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="7b4af-148">Properties returned from an actual call vary according to context.</span></span>

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