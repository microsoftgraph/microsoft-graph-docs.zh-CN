---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4542f202c08b97d2107fb8085a89acee640ee490
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194682"
---
# <a name="update-devicecategory"></a><span data-ttu-id="073f1-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="073f1-103">Update deviceCategory</span></span>

> <span data-ttu-id="073f1-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="073f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="073f1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="073f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="073f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="073f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="073f1-107">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="073f1-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="073f1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="073f1-108">Prerequisites</span></span>

<span data-ttu-id="073f1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="073f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="073f1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="073f1-111">Permission type</span></span>|<span data-ttu-id="073f1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="073f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="073f1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="073f1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="073f1-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="073f1-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="073f1-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073f1-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="073f1-116">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="073f1-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="073f1-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073f1-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="073f1-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="073f1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="073f1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="073f1-119">Not supported.</span></span>|
|<span data-ttu-id="073f1-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="073f1-120">Application</span></span>||
| <span data-ttu-id="073f1-121">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="073f1-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="073f1-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073f1-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="073f1-123">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="073f1-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="073f1-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073f1-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="073f1-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="073f1-125">HTTP Request</span></span>

<span data-ttu-id="073f1-126">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="073f1-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="073f1-127">**入职**</span><span class="sxs-lookup"><span data-stu-id="073f1-127">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="073f1-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="073f1-128">Request headers</span></span>

|<span data-ttu-id="073f1-129">标头</span><span class="sxs-lookup"><span data-stu-id="073f1-129">Header</span></span>|<span data-ttu-id="073f1-130">值</span><span class="sxs-lookup"><span data-stu-id="073f1-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="073f1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="073f1-131">Authorization</span></span>|<span data-ttu-id="073f1-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="073f1-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="073f1-133">接受</span><span class="sxs-lookup"><span data-stu-id="073f1-133">Accept</span></span>|<span data-ttu-id="073f1-134">application/json</span><span class="sxs-lookup"><span data-stu-id="073f1-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="073f1-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="073f1-135">Request body</span></span>

<span data-ttu-id="073f1-136">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="073f1-136">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="073f1-137">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="073f1-137">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="073f1-138">属性</span><span class="sxs-lookup"><span data-stu-id="073f1-138">Property</span></span>|<span data-ttu-id="073f1-139">类型</span><span class="sxs-lookup"><span data-stu-id="073f1-139">Type</span></span>|<span data-ttu-id="073f1-140">说明</span><span class="sxs-lookup"><span data-stu-id="073f1-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="073f1-141">id</span><span class="sxs-lookup"><span data-stu-id="073f1-141">id</span></span>|<span data-ttu-id="073f1-142">字符串</span><span class="sxs-lookup"><span data-stu-id="073f1-142">String</span></span>|<span data-ttu-id="073f1-143">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="073f1-143">Unique identifier for the device category.</span></span> <span data-ttu-id="073f1-144">只读。</span><span class="sxs-lookup"><span data-stu-id="073f1-144">Read-only.</span></span>|
|<span data-ttu-id="073f1-145">**载入**</span><span class="sxs-lookup"><span data-stu-id="073f1-145">**Onboarding**</span></span>|
|<span data-ttu-id="073f1-146">说明</span><span class="sxs-lookup"><span data-stu-id="073f1-146">description</span></span>|<span data-ttu-id="073f1-147">String</span><span class="sxs-lookup"><span data-stu-id="073f1-147">String</span></span>|<span data-ttu-id="073f1-148">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="073f1-148">Optional description for the device category.</span></span>|
|<span data-ttu-id="073f1-149">displayName</span><span class="sxs-lookup"><span data-stu-id="073f1-149">displayName</span></span>|<span data-ttu-id="073f1-150">String</span><span class="sxs-lookup"><span data-stu-id="073f1-150">String</span></span>|<span data-ttu-id="073f1-151">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="073f1-151">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="073f1-152">响应</span><span class="sxs-lookup"><span data-stu-id="073f1-152">Response</span></span>

<span data-ttu-id="073f1-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="073f1-153">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="073f1-154">示例</span><span class="sxs-lookup"><span data-stu-id="073f1-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="073f1-155">请求</span><span class="sxs-lookup"><span data-stu-id="073f1-155">Request</span></span>

<span data-ttu-id="073f1-156">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="073f1-156">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="073f1-157">响应</span><span class="sxs-lookup"><span data-stu-id="073f1-157">Response</span></span>

<span data-ttu-id="073f1-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="073f1-158">Here is an example of the response.</span></span> <span data-ttu-id="073f1-159">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="073f1-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="073f1-160">响应属性将根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="073f1-160">Response properties will vary according to context.</span></span>

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







