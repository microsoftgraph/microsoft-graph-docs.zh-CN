---
title: 更新 detectedApp
description: 更新 detectedApp 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0d181cc6eae44954e5fce16fb03299b4dc74618d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364520"
---
# <a name="update-detectedapp"></a><span data-ttu-id="2a9f2-103">更新 detectedApp</span><span class="sxs-lookup"><span data-stu-id="2a9f2-103">Update detectedApp</span></span>

> <span data-ttu-id="2a9f2-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a9f2-105">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-105">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a9f2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a9f2-106">Prerequisites</span></span>
<span data-ttu-id="2a9f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a9f2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a9f2-109">Permission type</span></span>|<span data-ttu-id="2a9f2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a9f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a9f2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a9f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a9f2-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a9f2-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2a9f2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a9f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a9f2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-114">Not supported.</span></span>|
|<span data-ttu-id="2a9f2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a9f2-115">Application</span></span>|<span data-ttu-id="2a9f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a9f2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a9f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2a9f2-118">请求头</span><span class="sxs-lookup"><span data-stu-id="2a9f2-118">Request headers</span></span>
|<span data-ttu-id="2a9f2-119">标头</span><span class="sxs-lookup"><span data-stu-id="2a9f2-119">Header</span></span>|<span data-ttu-id="2a9f2-120">值</span><span class="sxs-lookup"><span data-stu-id="2a9f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a9f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a9f2-121">Authorization</span></span>|<span data-ttu-id="2a9f2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a9f2-123">接受</span><span class="sxs-lookup"><span data-stu-id="2a9f2-123">Accept</span></span>|<span data-ttu-id="2a9f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2a9f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a9f2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a9f2-125">Request body</span></span>
<span data-ttu-id="2a9f2-126">在请求正文中，提供 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-126">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="2a9f2-127">下表显示创建 [detectedApp](../resources/intune-devices-detectedapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-127">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="2a9f2-128">属性</span><span class="sxs-lookup"><span data-stu-id="2a9f2-128">Property</span></span>|<span data-ttu-id="2a9f2-129">类型</span><span class="sxs-lookup"><span data-stu-id="2a9f2-129">Type</span></span>|<span data-ttu-id="2a9f2-130">说明</span><span class="sxs-lookup"><span data-stu-id="2a9f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a9f2-131">id</span><span class="sxs-lookup"><span data-stu-id="2a9f2-131">id</span></span>|<span data-ttu-id="2a9f2-132">String</span><span class="sxs-lookup"><span data-stu-id="2a9f2-132">String</span></span>|<span data-ttu-id="2a9f2-133">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="2a9f2-134">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="2a9f2-135">只读。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-135">Read-only.</span></span>|
|<span data-ttu-id="2a9f2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2a9f2-136">displayName</span></span>|<span data-ttu-id="2a9f2-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2a9f2-137">String</span></span>|<span data-ttu-id="2a9f2-138">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-138">Name of the discovered application.</span></span> <span data-ttu-id="2a9f2-139">只读</span><span class="sxs-lookup"><span data-stu-id="2a9f2-139">Read-only</span></span>|
|<span data-ttu-id="2a9f2-140">version</span><span class="sxs-lookup"><span data-stu-id="2a9f2-140">version</span></span>|<span data-ttu-id="2a9f2-141">String</span><span class="sxs-lookup"><span data-stu-id="2a9f2-141">String</span></span>|<span data-ttu-id="2a9f2-142">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-142">Version of the discovered application.</span></span> <span data-ttu-id="2a9f2-143">只读</span><span class="sxs-lookup"><span data-stu-id="2a9f2-143">Read-only</span></span>|
|<span data-ttu-id="2a9f2-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="2a9f2-144">sizeInByte</span></span>|<span data-ttu-id="2a9f2-145">Int64</span><span class="sxs-lookup"><span data-stu-id="2a9f2-145">Int64</span></span>|<span data-ttu-id="2a9f2-146">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-146">Discovered application size in bytes.</span></span> <span data-ttu-id="2a9f2-147">只读</span><span class="sxs-lookup"><span data-stu-id="2a9f2-147">Read-only</span></span>|
|<span data-ttu-id="2a9f2-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9f2-148">deviceCount</span></span>|<span data-ttu-id="2a9f2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9f2-149">Int32</span></span>|<span data-ttu-id="2a9f2-150">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="2a9f2-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="2a9f2-151">响应</span><span class="sxs-lookup"><span data-stu-id="2a9f2-151">Response</span></span>
<span data-ttu-id="2a9f2-152">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-152">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a9f2-153">示例</span><span class="sxs-lookup"><span data-stu-id="2a9f2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a9f2-154">请求</span><span class="sxs-lookup"><span data-stu-id="2a9f2-154">Request</span></span>
<span data-ttu-id="2a9f2-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2a9f2-156">响应</span><span class="sxs-lookup"><span data-stu-id="2a9f2-156">Response</span></span>
<span data-ttu-id="2a9f2-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a9f2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```




