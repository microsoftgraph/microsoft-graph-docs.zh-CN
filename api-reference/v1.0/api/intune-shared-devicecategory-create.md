---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76c1d0c8b22484b3a35d0db49c5a4e578e656880
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255169"
---
# <a name="create-devicecategory"></a><span data-ttu-id="12773-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="12773-103">Create deviceCategory</span></span>

> <span data-ttu-id="12773-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12773-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12773-105">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12773-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12773-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="12773-106">Prerequisites</span></span>
<span data-ttu-id="12773-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12773-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12773-109">Permission type</span></span>|<span data-ttu-id="12773-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12773-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12773-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12773-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="12773-112">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="12773-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="12773-113">DeviceManagementManaged 设备。 ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="12773-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="12773-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12773-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12773-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12773-115">Not supported.</span></span>|
|<span data-ttu-id="12773-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12773-116">Application</span></span>|<span data-ttu-id="12773-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="12773-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12773-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12773-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="12773-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12773-119">Request headers</span></span>
|<span data-ttu-id="12773-120">标头</span><span class="sxs-lookup"><span data-stu-id="12773-120">Header</span></span>|<span data-ttu-id="12773-121">值</span><span class="sxs-lookup"><span data-stu-id="12773-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12773-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12773-122">Authorization</span></span>|<span data-ttu-id="12773-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12773-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12773-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12773-124">Accept</span></span>|<span data-ttu-id="12773-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12773-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12773-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12773-126">Request body</span></span>
<span data-ttu-id="12773-127">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12773-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="12773-128">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12773-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="12773-129">属性</span><span class="sxs-lookup"><span data-stu-id="12773-129">Property</span></span>|<span data-ttu-id="12773-130">类型</span><span class="sxs-lookup"><span data-stu-id="12773-130">Type</span></span>|<span data-ttu-id="12773-131">说明</span><span class="sxs-lookup"><span data-stu-id="12773-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12773-132">id</span><span class="sxs-lookup"><span data-stu-id="12773-132">id</span></span>|<span data-ttu-id="12773-133">String</span><span class="sxs-lookup"><span data-stu-id="12773-133">String</span></span>|<span data-ttu-id="12773-134">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12773-134">Unique identifier for the device category.</span></span> <span data-ttu-id="12773-135">只读。</span><span class="sxs-lookup"><span data-stu-id="12773-135">Read-only.</span></span>|
|<span data-ttu-id="12773-136">**载入**</span><span class="sxs-lookup"><span data-stu-id="12773-136">**Onboarding**</span></span>|
|<span data-ttu-id="12773-137">displayName</span><span class="sxs-lookup"><span data-stu-id="12773-137">displayName</span></span>|<span data-ttu-id="12773-138">String</span><span class="sxs-lookup"><span data-stu-id="12773-138">String</span></span>|<span data-ttu-id="12773-139">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="12773-139">Display name for the device category.</span></span>|
|<span data-ttu-id="12773-140">description</span><span class="sxs-lookup"><span data-stu-id="12773-140">description</span></span>|<span data-ttu-id="12773-141">String</span><span class="sxs-lookup"><span data-stu-id="12773-141">String</span></span>|<span data-ttu-id="12773-142">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="12773-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="12773-143">响应</span><span class="sxs-lookup"><span data-stu-id="12773-143">Response</span></span>
<span data-ttu-id="12773-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12773-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12773-145">示例</span><span class="sxs-lookup"><span data-stu-id="12773-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="12773-146">请求</span><span class="sxs-lookup"><span data-stu-id="12773-146">Request</span></span>
<span data-ttu-id="12773-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12773-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="12773-148">响应</span><span class="sxs-lookup"><span data-stu-id="12773-148">Response</span></span>
<span data-ttu-id="12773-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12773-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



