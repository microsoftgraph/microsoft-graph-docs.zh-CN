---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 761ae7f5b7279f2f5bbad9077312bcb2b73f4859
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898435"
---
# <a name="update-devicecategory"></a><span data-ttu-id="58880-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="58880-103">Update deviceCategory</span></span>

> <span data-ttu-id="58880-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="58880-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58880-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="58880-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58880-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58880-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58880-107">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="58880-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58880-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="58880-108">Prerequisites</span></span>

<span data-ttu-id="58880-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58880-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58880-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="58880-111">Permission type</span></span>|<span data-ttu-id="58880-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58880-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58880-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58880-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="58880-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="58880-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="58880-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58880-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="58880-116">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="58880-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="58880-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58880-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58880-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58880-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58880-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="58880-119">Not supported.</span></span>|
|<span data-ttu-id="58880-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="58880-120">Application</span></span>|<span data-ttu-id="58880-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="58880-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58880-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58880-122">HTTP Request</span></span>

<span data-ttu-id="58880-123">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="58880-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="58880-124">**入职**</span><span class="sxs-lookup"><span data-stu-id="58880-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="58880-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="58880-125">Request headers</span></span>

|<span data-ttu-id="58880-126">标头</span><span class="sxs-lookup"><span data-stu-id="58880-126">Header</span></span>|<span data-ttu-id="58880-127">值</span><span class="sxs-lookup"><span data-stu-id="58880-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58880-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="58880-128">Authorization</span></span>|<span data-ttu-id="58880-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58880-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58880-130">接受</span><span class="sxs-lookup"><span data-stu-id="58880-130">Accept</span></span>|<span data-ttu-id="58880-131">application/json</span><span class="sxs-lookup"><span data-stu-id="58880-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58880-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="58880-132">Request body</span></span>

<span data-ttu-id="58880-133">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58880-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="58880-134">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58880-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="58880-135">属性</span><span class="sxs-lookup"><span data-stu-id="58880-135">Property</span></span>|<span data-ttu-id="58880-136">类型</span><span class="sxs-lookup"><span data-stu-id="58880-136">Type</span></span>|<span data-ttu-id="58880-137">说明</span><span class="sxs-lookup"><span data-stu-id="58880-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58880-138">id</span><span class="sxs-lookup"><span data-stu-id="58880-138">id</span></span>|<span data-ttu-id="58880-139">字符串</span><span class="sxs-lookup"><span data-stu-id="58880-139">String</span></span>|<span data-ttu-id="58880-140">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="58880-140">Unique identifier for the device category.</span></span> <span data-ttu-id="58880-141">只读。</span><span class="sxs-lookup"><span data-stu-id="58880-141">Read-only.</span></span>|
|<span data-ttu-id="58880-142">**载入**</span><span class="sxs-lookup"><span data-stu-id="58880-142">**Onboarding**</span></span>|
|<span data-ttu-id="58880-143">说明</span><span class="sxs-lookup"><span data-stu-id="58880-143">description</span></span>|<span data-ttu-id="58880-144">String</span><span class="sxs-lookup"><span data-stu-id="58880-144">String</span></span>|<span data-ttu-id="58880-145">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="58880-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="58880-146">displayName</span><span class="sxs-lookup"><span data-stu-id="58880-146">displayName</span></span>|<span data-ttu-id="58880-147">String</span><span class="sxs-lookup"><span data-stu-id="58880-147">String</span></span>|<span data-ttu-id="58880-148">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="58880-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="58880-149">响应</span><span class="sxs-lookup"><span data-stu-id="58880-149">Response</span></span>

<span data-ttu-id="58880-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58880-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58880-151">示例</span><span class="sxs-lookup"><span data-stu-id="58880-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="58880-152">请求</span><span class="sxs-lookup"><span data-stu-id="58880-152">Request</span></span>

<span data-ttu-id="58880-153">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="58880-153">Here are examples of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="58880-154">响应</span><span class="sxs-lookup"><span data-stu-id="58880-154">Response</span></span>

<span data-ttu-id="58880-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="58880-155">Here is an example of the response.</span></span> <span data-ttu-id="58880-156">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="58880-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="58880-157">响应属性将根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="58880-157">Response properties will vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



