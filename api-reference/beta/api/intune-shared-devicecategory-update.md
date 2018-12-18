---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: tfitzmac
ms.openlocfilehash: 8676067ff4ce34358bcfd8400d28e1d73bd11f68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321516"
---
# <a name="update-devicecategory"></a><span data-ttu-id="5e192-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5e192-103">Update deviceCategory</span></span>

> <span data-ttu-id="5e192-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e192-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e192-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e192-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e192-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5e192-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e192-107">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e192-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e192-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e192-108">Prerequisites</span></span>

<span data-ttu-id="5e192-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5e192-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e192-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e192-111">Permission type</span></span>|<span data-ttu-id="5e192-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e192-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e192-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e192-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5e192-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5e192-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5e192-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e192-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5e192-116">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="5e192-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5e192-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e192-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e192-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e192-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e192-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e192-119">Not supported.</span></span>|
|<span data-ttu-id="5e192-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e192-120">Application</span></span>|<span data-ttu-id="5e192-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e192-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e192-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e192-122">HTTP Request</span></span>

<span data-ttu-id="5e192-123">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="5e192-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="5e192-124">**在白板**</span><span class="sxs-lookup"><span data-stu-id="5e192-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5e192-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e192-125">Request headers</span></span>

|<span data-ttu-id="5e192-126">标头</span><span class="sxs-lookup"><span data-stu-id="5e192-126">Header</span></span>|<span data-ttu-id="5e192-127">值</span><span class="sxs-lookup"><span data-stu-id="5e192-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e192-128">授权</span><span class="sxs-lookup"><span data-stu-id="5e192-128">Authorization</span></span>|<span data-ttu-id="5e192-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e192-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e192-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5e192-130">Accept</span></span>|<span data-ttu-id="5e192-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5e192-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e192-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e192-132">Request body</span></span>

<span data-ttu-id="5e192-133">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e192-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="5e192-134">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5e192-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="5e192-135">属性</span><span class="sxs-lookup"><span data-stu-id="5e192-135">Property</span></span>|<span data-ttu-id="5e192-136">类型</span><span class="sxs-lookup"><span data-stu-id="5e192-136">Type</span></span>|<span data-ttu-id="5e192-137">说明</span><span class="sxs-lookup"><span data-stu-id="5e192-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e192-138">id</span><span class="sxs-lookup"><span data-stu-id="5e192-138">id</span></span>|<span data-ttu-id="5e192-139">String</span><span class="sxs-lookup"><span data-stu-id="5e192-139">String</span></span>|<span data-ttu-id="5e192-140">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e192-140">Unique identifier for the device category.</span></span> <span data-ttu-id="5e192-141">只读。</span><span class="sxs-lookup"><span data-stu-id="5e192-141">Read-only.</span></span>|
|<span data-ttu-id="5e192-142">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="5e192-142">**Onboarding**</span></span>|
|<span data-ttu-id="5e192-143">说明</span><span class="sxs-lookup"><span data-stu-id="5e192-143">description</span></span>|<span data-ttu-id="5e192-144">String</span><span class="sxs-lookup"><span data-stu-id="5e192-144">String</span></span>|<span data-ttu-id="5e192-145">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="5e192-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="5e192-146">displayName</span><span class="sxs-lookup"><span data-stu-id="5e192-146">displayName</span></span>|<span data-ttu-id="5e192-147">String</span><span class="sxs-lookup"><span data-stu-id="5e192-147">String</span></span>|<span data-ttu-id="5e192-148">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5e192-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="5e192-149">响应</span><span class="sxs-lookup"><span data-stu-id="5e192-149">Response</span></span>

<span data-ttu-id="5e192-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e192-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e192-151">示例</span><span class="sxs-lookup"><span data-stu-id="5e192-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e192-152">请求</span><span class="sxs-lookup"><span data-stu-id="5e192-152">Request</span></span>

<span data-ttu-id="5e192-153">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="5e192-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="5e192-154">响应</span><span class="sxs-lookup"><span data-stu-id="5e192-154">Response</span></span>

<span data-ttu-id="5e192-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e192-155">Here is an example of the response.</span></span> <span data-ttu-id="5e192-156">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5e192-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5e192-157">响应属性根据上下文不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="5e192-157">Response properties will vary according to context.</span></span>

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



