---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8690e7db843c4769a1f3646ec5199240f1e98765
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732267"
---
# <a name="update-devicecategory"></a><span data-ttu-id="3beef-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3beef-103">Update deviceCategory</span></span>

<span data-ttu-id="3beef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3beef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3beef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3beef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3beef-106">更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3beef-106">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3beef-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3beef-107">Prerequisites</span></span>
<span data-ttu-id="3beef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3beef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3beef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3beef-110">Permission type</span></span>|<span data-ttu-id="3beef-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3beef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3beef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3beef-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3beef-113">&nbsp;&nbsp;**载入** 和</span><span class="sxs-lookup"><span data-stu-id="3beef-113">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="3beef-114">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="3beef-114">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="3beef-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3beef-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3beef-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3beef-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3beef-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3beef-117">Not supported.</span></span>|
|<span data-ttu-id="3beef-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3beef-118">Application</span></span>|<span data-ttu-id="3beef-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3beef-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3beef-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3beef-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="3beef-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3beef-121">Request headers</span></span>
|<span data-ttu-id="3beef-122">标头</span><span class="sxs-lookup"><span data-stu-id="3beef-122">Header</span></span>|<span data-ttu-id="3beef-123">值</span><span class="sxs-lookup"><span data-stu-id="3beef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3beef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3beef-124">Authorization</span></span>|<span data-ttu-id="3beef-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3beef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3beef-126">接受</span><span class="sxs-lookup"><span data-stu-id="3beef-126">Accept</span></span>|<span data-ttu-id="3beef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3beef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3beef-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3beef-128">Request body</span></span>
<span data-ttu-id="3beef-129">在请求正文中，提供 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3beef-129">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="3beef-130">下表显示创建 [deviceCategory](../resources/intune-shared-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3beef-130">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="3beef-131">属性</span><span class="sxs-lookup"><span data-stu-id="3beef-131">Property</span></span>|<span data-ttu-id="3beef-132">类型</span><span class="sxs-lookup"><span data-stu-id="3beef-132">Type</span></span>|<span data-ttu-id="3beef-133">说明</span><span class="sxs-lookup"><span data-stu-id="3beef-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3beef-134">id</span><span class="sxs-lookup"><span data-stu-id="3beef-134">id</span></span>|<span data-ttu-id="3beef-135">String</span><span class="sxs-lookup"><span data-stu-id="3beef-135">String</span></span>|<span data-ttu-id="3beef-136">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3beef-136">Unique identifier for the device category.</span></span> <span data-ttu-id="3beef-137">只读。</span><span class="sxs-lookup"><span data-stu-id="3beef-137">Read-only.</span></span>|
|<span data-ttu-id="3beef-138">**载入**</span><span class="sxs-lookup"><span data-stu-id="3beef-138">**Onboarding**</span></span>|
|<span data-ttu-id="3beef-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3beef-139">displayName</span></span>|<span data-ttu-id="3beef-140">String</span><span class="sxs-lookup"><span data-stu-id="3beef-140">String</span></span>|<span data-ttu-id="3beef-141">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3beef-141">Display name for the device category.</span></span>|
|<span data-ttu-id="3beef-142">说明</span><span class="sxs-lookup"><span data-stu-id="3beef-142">description</span></span>|<span data-ttu-id="3beef-143">String</span><span class="sxs-lookup"><span data-stu-id="3beef-143">String</span></span>|<span data-ttu-id="3beef-144">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="3beef-144">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="3beef-145">响应</span><span class="sxs-lookup"><span data-stu-id="3beef-145">Response</span></span>
<span data-ttu-id="3beef-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3beef-146">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3beef-147">示例</span><span class="sxs-lookup"><span data-stu-id="3beef-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="3beef-148">请求</span><span class="sxs-lookup"><span data-stu-id="3beef-148">Request</span></span>
<span data-ttu-id="3beef-149">下面是请求示例。</span><span class="sxs-lookup"><span data-stu-id="3beef-149">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="3beef-150">响应</span><span class="sxs-lookup"><span data-stu-id="3beef-150">Response</span></span>
<span data-ttu-id="3beef-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3beef-151">Here is an example of the response.</span></span> <span data-ttu-id="3beef-152">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3beef-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3beef-153">响应属性因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="3beef-153">Response properties will vary according to context.</span></span>
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









