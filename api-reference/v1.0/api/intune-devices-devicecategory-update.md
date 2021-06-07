---
title: 更新 deviceCategory
description: 更新 deviceCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40fecdf307c73c0fed94f10122c40ac268bafa45
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748990"
---
# <a name="update-devicecategory"></a><span data-ttu-id="346e4-103">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="346e4-103">Update deviceCategory</span></span>

<span data-ttu-id="346e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="346e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="346e4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="346e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="346e4-106">更新 [deviceCategory](../resources/intune-devices-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="346e4-106">Update the properties of a [deviceCategory](../resources/intune-devices-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="346e4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="346e4-107">Prerequisites</span></span>
<span data-ttu-id="346e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="346e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="346e4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="346e4-110">Permission type</span></span>|<span data-ttu-id="346e4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="346e4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="346e4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="346e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="346e4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346e4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="346e4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="346e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="346e4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="346e4-115">Not supported.</span></span>|
|<span data-ttu-id="346e4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="346e4-116">Application</span></span>|<span data-ttu-id="346e4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346e4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="346e4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="346e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="346e4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="346e4-119">Request headers</span></span>
|<span data-ttu-id="346e4-120">标头</span><span class="sxs-lookup"><span data-stu-id="346e4-120">Header</span></span>|<span data-ttu-id="346e4-121">值</span><span class="sxs-lookup"><span data-stu-id="346e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="346e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="346e4-122">Authorization</span></span>|<span data-ttu-id="346e4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="346e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="346e4-124">接受</span><span class="sxs-lookup"><span data-stu-id="346e4-124">Accept</span></span>|<span data-ttu-id="346e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="346e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="346e4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="346e4-126">Request body</span></span>
<span data-ttu-id="346e4-127">在请求正文中，提供 [deviceCategory](../resources/intune-devices-devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="346e4-127">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-devices-devicecategory.md) object.</span></span>

<span data-ttu-id="346e4-128">下表显示创建 [deviceCategory](../resources/intune-devices-devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="346e4-128">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-devices-devicecategory.md).</span></span>

|<span data-ttu-id="346e4-129">属性</span><span class="sxs-lookup"><span data-stu-id="346e4-129">Property</span></span>|<span data-ttu-id="346e4-130">类型</span><span class="sxs-lookup"><span data-stu-id="346e4-130">Type</span></span>|<span data-ttu-id="346e4-131">说明</span><span class="sxs-lookup"><span data-stu-id="346e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346e4-132">id</span><span class="sxs-lookup"><span data-stu-id="346e4-132">id</span></span>|<span data-ttu-id="346e4-133">String</span><span class="sxs-lookup"><span data-stu-id="346e4-133">String</span></span>|<span data-ttu-id="346e4-134">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="346e4-134">Unique identifier for the device category.</span></span> <span data-ttu-id="346e4-135">只读。</span><span class="sxs-lookup"><span data-stu-id="346e4-135">Read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="346e4-136">响应</span><span class="sxs-lookup"><span data-stu-id="346e4-136">Response</span></span>
<span data-ttu-id="346e4-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune-devices-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="346e4-137">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-devices-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="346e4-138">示例</span><span class="sxs-lookup"><span data-stu-id="346e4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="346e4-139">请求</span><span class="sxs-lookup"><span data-stu-id="346e4-139">Request</span></span>
<span data-ttu-id="346e4-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="346e4-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.deviceCategory"
}
```

### <a name="response"></a><span data-ttu-id="346e4-141">响应</span><span class="sxs-lookup"><span data-stu-id="346e4-141">Response</span></span>
<span data-ttu-id="346e4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="346e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```




