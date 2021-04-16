---
title: 获取 deviceCategory
description: 读取 deviceCategory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6708e74f63dd64b5f993da0405e01c65287415d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863420"
---
# <a name="get-devicecategory"></a><span data-ttu-id="dcae5-103">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="dcae5-103">Get deviceCategory</span></span>

<span data-ttu-id="dcae5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcae5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcae5-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="dcae5-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dcae5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dcae5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcae5-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcae5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcae5-108">读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dcae5-108">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcae5-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="dcae5-109">Prerequisites</span></span>

<span data-ttu-id="dcae5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcae5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcae5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcae5-112">Permission type</span></span>|<span data-ttu-id="dcae5-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dcae5-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcae5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcae5-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dcae5-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="dcae5-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="dcae5-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcae5-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="dcae5-117">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="dcae5-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="dcae5-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcae5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="dcae5-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcae5-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcae5-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcae5-120">Not supported.</span></span>|
|<span data-ttu-id="dcae5-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcae5-121">Application</span></span>||
| <span data-ttu-id="dcae5-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="dcae5-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="dcae5-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcae5-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="dcae5-124">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="dcae5-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="dcae5-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcae5-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcae5-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcae5-126">HTTP Request</span></span>

<span data-ttu-id="dcae5-127">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="dcae5-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="dcae5-128">**载入**</span><span class="sxs-lookup"><span data-stu-id="dcae5-128">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcae5-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dcae5-129">Optional query parameters</span></span>

<span data-ttu-id="dcae5-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dcae5-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcae5-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcae5-131">Request headers</span></span>

|<span data-ttu-id="dcae5-132">标头</span><span class="sxs-lookup"><span data-stu-id="dcae5-132">Header</span></span>|<span data-ttu-id="dcae5-133">值</span><span class="sxs-lookup"><span data-stu-id="dcae5-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcae5-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcae5-134">Authorization</span></span>|<span data-ttu-id="dcae5-135">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dcae5-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcae5-136">接受</span><span class="sxs-lookup"><span data-stu-id="dcae5-136">Accept</span></span>|<span data-ttu-id="dcae5-137">application/json</span><span class="sxs-lookup"><span data-stu-id="dcae5-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcae5-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcae5-138">Request body</span></span>

<span data-ttu-id="dcae5-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcae5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcae5-140">响应</span><span class="sxs-lookup"><span data-stu-id="dcae5-140">Response</span></span>

<span data-ttu-id="dcae5-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dcae5-141">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcae5-142">示例</span><span class="sxs-lookup"><span data-stu-id="dcae5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcae5-143">请求</span><span class="sxs-lookup"><span data-stu-id="dcae5-143">Request</span></span>

<span data-ttu-id="dcae5-144">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="dcae5-144">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="dcae5-145">响应</span><span class="sxs-lookup"><span data-stu-id="dcae5-145">Response</span></span>

<span data-ttu-id="dcae5-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dcae5-146">Here is an example of the response.</span></span> <span data-ttu-id="dcae5-147">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dcae5-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dcae5-148">从实际调用返回的属性因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="dcae5-148">Properties returned from an actual call vary according to context.</span></span>

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










