---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8690e7db843c4769a1f3646ec5199240f1e98765
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625479"
---
# <a name="update-devicecategory"></a><span data-ttu-id="1a26e-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1a26e-103">Update deviceCategory</span></span>

<span data-ttu-id="1a26e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a26e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a26e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a26e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a26e-106">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a26e-106">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a26e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a26e-107">Prerequisites</span></span>
<span data-ttu-id="1a26e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a26e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a26e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a26e-110">Permission type</span></span>|<span data-ttu-id="1a26e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a26e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a26e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a26e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1a26e-113">&nbsp;&nbsp;**载入** 和</span><span class="sxs-lookup"><span data-stu-id="1a26e-113">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="1a26e-114">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="1a26e-114">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="1a26e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a26e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a26e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a26e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a26e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a26e-117">Not supported.</span></span>|
|<span data-ttu-id="1a26e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a26e-118">Application</span></span>|<span data-ttu-id="1a26e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a26e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a26e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a26e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="1a26e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a26e-121">Request headers</span></span>
|<span data-ttu-id="1a26e-122">标头</span><span class="sxs-lookup"><span data-stu-id="1a26e-122">Header</span></span>|<span data-ttu-id="1a26e-123">值</span><span class="sxs-lookup"><span data-stu-id="1a26e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a26e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a26e-124">Authorization</span></span>|<span data-ttu-id="1a26e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a26e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a26e-126">接受</span><span class="sxs-lookup"><span data-stu-id="1a26e-126">Accept</span></span>|<span data-ttu-id="1a26e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1a26e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a26e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a26e-128">Request body</span></span>
<span data-ttu-id="1a26e-129">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a26e-129">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="1a26e-130">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a26e-130">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="1a26e-131">属性</span><span class="sxs-lookup"><span data-stu-id="1a26e-131">Property</span></span>|<span data-ttu-id="1a26e-132">类型</span><span class="sxs-lookup"><span data-stu-id="1a26e-132">Type</span></span>|<span data-ttu-id="1a26e-133">说明</span><span class="sxs-lookup"><span data-stu-id="1a26e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a26e-134">id</span><span class="sxs-lookup"><span data-stu-id="1a26e-134">id</span></span>|<span data-ttu-id="1a26e-135">String</span><span class="sxs-lookup"><span data-stu-id="1a26e-135">String</span></span>|<span data-ttu-id="1a26e-136">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1a26e-136">Unique identifier for the device category.</span></span> <span data-ttu-id="1a26e-137">只读。</span><span class="sxs-lookup"><span data-stu-id="1a26e-137">Read-only.</span></span>|
|<span data-ttu-id="1a26e-138">**载入**</span><span class="sxs-lookup"><span data-stu-id="1a26e-138">**Onboarding**</span></span>|
|<span data-ttu-id="1a26e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1a26e-139">displayName</span></span>|<span data-ttu-id="1a26e-140">String</span><span class="sxs-lookup"><span data-stu-id="1a26e-140">String</span></span>|<span data-ttu-id="1a26e-141">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1a26e-141">Display name for the device category.</span></span>|
|<span data-ttu-id="1a26e-142">说明</span><span class="sxs-lookup"><span data-stu-id="1a26e-142">description</span></span>|<span data-ttu-id="1a26e-143">String</span><span class="sxs-lookup"><span data-stu-id="1a26e-143">String</span></span>|<span data-ttu-id="1a26e-144">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="1a26e-144">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="1a26e-145">响应</span><span class="sxs-lookup"><span data-stu-id="1a26e-145">Response</span></span>
<span data-ttu-id="1a26e-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a26e-146">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a26e-147">示例</span><span class="sxs-lookup"><span data-stu-id="1a26e-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a26e-148">请求</span><span class="sxs-lookup"><span data-stu-id="1a26e-148">Request</span></span>
<span data-ttu-id="1a26e-149">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="1a26e-149">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="1a26e-150">响应</span><span class="sxs-lookup"><span data-stu-id="1a26e-150">Response</span></span>
<span data-ttu-id="1a26e-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a26e-151">Here is an example of the response.</span></span> <span data-ttu-id="1a26e-152">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1a26e-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1a26e-153">响应属性因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="1a26e-153">Response properties will vary according to context.</span></span>
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









