---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b055f8865592e935aaa32e8a3a541151886d36de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986857"
---
# <a name="update-devicecategory"></a><span data-ttu-id="c47fd-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c47fd-103">Update deviceCategory</span></span>

> <span data-ttu-id="c47fd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c47fd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c47fd-105">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c47fd-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c47fd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c47fd-106">Prerequisites</span></span>
<span data-ttu-id="c47fd-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c47fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c47fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c47fd-109">Permission type</span></span>|<span data-ttu-id="c47fd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c47fd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c47fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c47fd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c47fd-112">&nbsp;&nbsp; **入职培训**和</span><span class="sxs-lookup"><span data-stu-id="c47fd-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="c47fd-113">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c47fd-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="c47fd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c47fd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c47fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c47fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c47fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c47fd-116">Not supported.</span></span>|
|<span data-ttu-id="c47fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c47fd-117">Application</span></span>|<span data-ttu-id="c47fd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c47fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c47fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c47fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="c47fd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c47fd-120">Request headers</span></span>
|<span data-ttu-id="c47fd-121">标头</span><span class="sxs-lookup"><span data-stu-id="c47fd-121">Header</span></span>|<span data-ttu-id="c47fd-122">值</span><span class="sxs-lookup"><span data-stu-id="c47fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c47fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c47fd-123">Authorization</span></span>|<span data-ttu-id="c47fd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c47fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c47fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c47fd-125">Accept</span></span>|<span data-ttu-id="c47fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c47fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c47fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c47fd-127">Request body</span></span>
<span data-ttu-id="c47fd-128">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c47fd-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="c47fd-129">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c47fd-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="c47fd-130">属性</span><span class="sxs-lookup"><span data-stu-id="c47fd-130">Property</span></span>|<span data-ttu-id="c47fd-131">类型</span><span class="sxs-lookup"><span data-stu-id="c47fd-131">Type</span></span>|<span data-ttu-id="c47fd-132">说明</span><span class="sxs-lookup"><span data-stu-id="c47fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c47fd-133">id</span><span class="sxs-lookup"><span data-stu-id="c47fd-133">id</span></span>|<span data-ttu-id="c47fd-134">String</span><span class="sxs-lookup"><span data-stu-id="c47fd-134">String</span></span>|<span data-ttu-id="c47fd-135">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c47fd-135">Unique identifier for the device category.</span></span> <span data-ttu-id="c47fd-136">只读。</span><span class="sxs-lookup"><span data-stu-id="c47fd-136">Read-only.</span></span>|
|<span data-ttu-id="c47fd-137">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="c47fd-137">**Onboarding**</span></span>|
|<span data-ttu-id="c47fd-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c47fd-138">displayName</span></span>|<span data-ttu-id="c47fd-139">String</span><span class="sxs-lookup"><span data-stu-id="c47fd-139">String</span></span>|<span data-ttu-id="c47fd-140">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c47fd-140">Display name for the device category.</span></span>|
|<span data-ttu-id="c47fd-141">description</span><span class="sxs-lookup"><span data-stu-id="c47fd-141">description</span></span>|<span data-ttu-id="c47fd-142">String</span><span class="sxs-lookup"><span data-stu-id="c47fd-142">String</span></span>|<span data-ttu-id="c47fd-143">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="c47fd-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="c47fd-144">响应</span><span class="sxs-lookup"><span data-stu-id="c47fd-144">Response</span></span>
<span data-ttu-id="c47fd-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c47fd-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c47fd-146">示例</span><span class="sxs-lookup"><span data-stu-id="c47fd-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="c47fd-147">请求</span><span class="sxs-lookup"><span data-stu-id="c47fd-147">Request</span></span>
<span data-ttu-id="c47fd-148">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="c47fd-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c47fd-149">响应</span><span class="sxs-lookup"><span data-stu-id="c47fd-149">Response</span></span>
<span data-ttu-id="c47fd-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c47fd-150">Here is an example of the response.</span></span> <span data-ttu-id="c47fd-151">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c47fd-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c47fd-152">响应属性根据上下文不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="c47fd-152">Response properties will vary according to context.</span></span>
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



