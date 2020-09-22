---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 248bb5627243bc9724f54e46e36cce593a18bd05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980384"
---
# <a name="update-devicecategory"></a><span data-ttu-id="54b33-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="54b33-103">Update deviceCategory</span></span>

<span data-ttu-id="54b33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54b33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54b33-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="54b33-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54b33-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54b33-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54b33-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54b33-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54b33-108">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="54b33-108">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54b33-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="54b33-109">Prerequisites</span></span>

<span data-ttu-id="54b33-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54b33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54b33-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="54b33-112">Permission type</span></span>|<span data-ttu-id="54b33-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="54b33-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54b33-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54b33-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="54b33-115">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="54b33-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="54b33-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b33-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="54b33-117">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="54b33-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="54b33-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b33-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="54b33-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54b33-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54b33-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="54b33-120">Not supported.</span></span>|
|<span data-ttu-id="54b33-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="54b33-121">Application</span></span>||
| <span data-ttu-id="54b33-122">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="54b33-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="54b33-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b33-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="54b33-124">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="54b33-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="54b33-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b33-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54b33-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54b33-126">HTTP Request</span></span>

<span data-ttu-id="54b33-127">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="54b33-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="54b33-128">**入职**</span><span class="sxs-lookup"><span data-stu-id="54b33-128">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="54b33-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="54b33-129">Request headers</span></span>

|<span data-ttu-id="54b33-130">标头</span><span class="sxs-lookup"><span data-stu-id="54b33-130">Header</span></span>|<span data-ttu-id="54b33-131">值</span><span class="sxs-lookup"><span data-stu-id="54b33-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54b33-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="54b33-132">Authorization</span></span>|<span data-ttu-id="54b33-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54b33-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54b33-134">接受</span><span class="sxs-lookup"><span data-stu-id="54b33-134">Accept</span></span>|<span data-ttu-id="54b33-135">application/json</span><span class="sxs-lookup"><span data-stu-id="54b33-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54b33-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="54b33-136">Request body</span></span>

<span data-ttu-id="54b33-137">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54b33-137">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="54b33-138">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="54b33-138">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="54b33-139">属性</span><span class="sxs-lookup"><span data-stu-id="54b33-139">Property</span></span>|<span data-ttu-id="54b33-140">类型</span><span class="sxs-lookup"><span data-stu-id="54b33-140">Type</span></span>|<span data-ttu-id="54b33-141">说明</span><span class="sxs-lookup"><span data-stu-id="54b33-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54b33-142">id</span><span class="sxs-lookup"><span data-stu-id="54b33-142">id</span></span>|<span data-ttu-id="54b33-143">String</span><span class="sxs-lookup"><span data-stu-id="54b33-143">String</span></span>|<span data-ttu-id="54b33-144">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="54b33-144">Unique identifier for the device category.</span></span> <span data-ttu-id="54b33-145">只读。</span><span class="sxs-lookup"><span data-stu-id="54b33-145">Read-only.</span></span>|
|<span data-ttu-id="54b33-146">**载入**</span><span class="sxs-lookup"><span data-stu-id="54b33-146">**Onboarding**</span></span>|
|<span data-ttu-id="54b33-147">description</span><span class="sxs-lookup"><span data-stu-id="54b33-147">description</span></span>|<span data-ttu-id="54b33-148">String</span><span class="sxs-lookup"><span data-stu-id="54b33-148">String</span></span>|<span data-ttu-id="54b33-149">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="54b33-149">Optional description for the device category.</span></span>|
|<span data-ttu-id="54b33-150">displayName</span><span class="sxs-lookup"><span data-stu-id="54b33-150">displayName</span></span>|<span data-ttu-id="54b33-151">String</span><span class="sxs-lookup"><span data-stu-id="54b33-151">String</span></span>|<span data-ttu-id="54b33-152">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="54b33-152">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="54b33-153">响应</span><span class="sxs-lookup"><span data-stu-id="54b33-153">Response</span></span>

<span data-ttu-id="54b33-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54b33-154">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54b33-155">示例</span><span class="sxs-lookup"><span data-stu-id="54b33-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="54b33-156">请求</span><span class="sxs-lookup"><span data-stu-id="54b33-156">Request</span></span>

<span data-ttu-id="54b33-157">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="54b33-157">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="54b33-158">响应</span><span class="sxs-lookup"><span data-stu-id="54b33-158">Response</span></span>

<span data-ttu-id="54b33-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="54b33-159">Here is an example of the response.</span></span> <span data-ttu-id="54b33-160">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54b33-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="54b33-161">响应属性将根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="54b33-161">Response properties will vary according to context.</span></span>

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












