---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: tfitzmac
ms.openlocfilehash: 73980aa4c178ff610ce44dc3b832c8c931d72740
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344301"
---
# <a name="update-devicecategory"></a><span data-ttu-id="4d00f-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4d00f-103">Update deviceCategory</span></span>

> <span data-ttu-id="4d00f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4d00f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d00f-105">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d00f-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d00f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d00f-106">Prerequisites</span></span>
<span data-ttu-id="4d00f-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4d00f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d00f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d00f-109">Permission type</span></span>|<span data-ttu-id="4d00f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d00f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d00f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d00f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4d00f-112">&nbsp;&nbsp; **入职培训**和</span><span class="sxs-lookup"><span data-stu-id="4d00f-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="4d00f-113">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4d00f-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="4d00f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d00f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4d00f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d00f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d00f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d00f-116">Not supported.</span></span>|
|<span data-ttu-id="4d00f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d00f-117">Application</span></span>|<span data-ttu-id="4d00f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d00f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d00f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d00f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="4d00f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d00f-120">Request headers</span></span>
|<span data-ttu-id="4d00f-121">标头</span><span class="sxs-lookup"><span data-stu-id="4d00f-121">Header</span></span>|<span data-ttu-id="4d00f-122">值</span><span class="sxs-lookup"><span data-stu-id="4d00f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d00f-123">授权</span><span class="sxs-lookup"><span data-stu-id="4d00f-123">Authorization</span></span>|<span data-ttu-id="4d00f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d00f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d00f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d00f-125">Accept</span></span>|<span data-ttu-id="4d00f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d00f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d00f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d00f-127">Request body</span></span>
<span data-ttu-id="4d00f-128">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d00f-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="4d00f-129">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d00f-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="4d00f-130">属性</span><span class="sxs-lookup"><span data-stu-id="4d00f-130">Property</span></span>|<span data-ttu-id="4d00f-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d00f-131">Type</span></span>|<span data-ttu-id="4d00f-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d00f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d00f-133">id</span><span class="sxs-lookup"><span data-stu-id="4d00f-133">id</span></span>|<span data-ttu-id="4d00f-134">String</span><span class="sxs-lookup"><span data-stu-id="4d00f-134">String</span></span>|<span data-ttu-id="4d00f-135">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4d00f-135">Unique identifier for the device category.</span></span> <span data-ttu-id="4d00f-136">只读。</span><span class="sxs-lookup"><span data-stu-id="4d00f-136">Read-only.</span></span>|
|<span data-ttu-id="4d00f-137">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="4d00f-137">**Onboarding**</span></span>|
|<span data-ttu-id="4d00f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4d00f-138">displayName</span></span>|<span data-ttu-id="4d00f-139">String</span><span class="sxs-lookup"><span data-stu-id="4d00f-139">String</span></span>|<span data-ttu-id="4d00f-140">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4d00f-140">Display name for the device category.</span></span>|
|<span data-ttu-id="4d00f-141">description</span><span class="sxs-lookup"><span data-stu-id="4d00f-141">description</span></span>|<span data-ttu-id="4d00f-142">String</span><span class="sxs-lookup"><span data-stu-id="4d00f-142">String</span></span>|<span data-ttu-id="4d00f-143">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="4d00f-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="4d00f-144">响应</span><span class="sxs-lookup"><span data-stu-id="4d00f-144">Response</span></span>
<span data-ttu-id="4d00f-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d00f-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d00f-146">示例</span><span class="sxs-lookup"><span data-stu-id="4d00f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d00f-147">请求</span><span class="sxs-lookup"><span data-stu-id="4d00f-147">Request</span></span>
<span data-ttu-id="4d00f-148">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="4d00f-148">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="4d00f-149">响应</span><span class="sxs-lookup"><span data-stu-id="4d00f-149">Response</span></span>
<span data-ttu-id="4d00f-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4d00f-150">Here is an example of the response.</span></span> <span data-ttu-id="4d00f-151">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4d00f-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4d00f-152">响应属性根据上下文不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="4d00f-152">Response properties will vary according to context.</span></span>
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



