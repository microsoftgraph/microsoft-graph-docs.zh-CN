---
title: 更新 detectedApp
description: 更新 detectedApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77cd21373eb2912bbc6364a674b9f5b71ae0cbcf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752635"
---
# <a name="update-detectedapp"></a><span data-ttu-id="61996-103">更新 detectedApp</span><span class="sxs-lookup"><span data-stu-id="61996-103">Update detectedApp</span></span>

<span data-ttu-id="61996-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61996-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61996-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61996-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61996-106">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="61996-106">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61996-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="61996-107">Prerequisites</span></span>
<span data-ttu-id="61996-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61996-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61996-110">Permission type</span></span>|<span data-ttu-id="61996-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61996-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61996-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61996-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61996-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61996-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61996-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61996-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61996-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61996-115">Not supported.</span></span>|
|<span data-ttu-id="61996-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61996-116">Application</span></span>|<span data-ttu-id="61996-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61996-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61996-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61996-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="61996-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="61996-119">Request headers</span></span>
|<span data-ttu-id="61996-120">标头</span><span class="sxs-lookup"><span data-stu-id="61996-120">Header</span></span>|<span data-ttu-id="61996-121">值</span><span class="sxs-lookup"><span data-stu-id="61996-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61996-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61996-122">Authorization</span></span>|<span data-ttu-id="61996-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="61996-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61996-124">接受</span><span class="sxs-lookup"><span data-stu-id="61996-124">Accept</span></span>|<span data-ttu-id="61996-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61996-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61996-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="61996-126">Request body</span></span>
<span data-ttu-id="61996-127">在请求正文中，提供 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61996-127">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="61996-128">下表显示创建 [detectedApp](../resources/intune-devices-detectedapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="61996-128">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="61996-129">属性</span><span class="sxs-lookup"><span data-stu-id="61996-129">Property</span></span>|<span data-ttu-id="61996-130">类型</span><span class="sxs-lookup"><span data-stu-id="61996-130">Type</span></span>|<span data-ttu-id="61996-131">说明</span><span class="sxs-lookup"><span data-stu-id="61996-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61996-132">id</span><span class="sxs-lookup"><span data-stu-id="61996-132">id</span></span>|<span data-ttu-id="61996-133">String</span><span class="sxs-lookup"><span data-stu-id="61996-133">String</span></span>|<span data-ttu-id="61996-134">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="61996-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="61996-135">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="61996-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="61996-136">只读。</span><span class="sxs-lookup"><span data-stu-id="61996-136">Read-only.</span></span>|
|<span data-ttu-id="61996-137">displayName</span><span class="sxs-lookup"><span data-stu-id="61996-137">displayName</span></span>|<span data-ttu-id="61996-138">String</span><span class="sxs-lookup"><span data-stu-id="61996-138">String</span></span>|<span data-ttu-id="61996-139">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="61996-139">Name of the discovered application.</span></span> <span data-ttu-id="61996-140">只读</span><span class="sxs-lookup"><span data-stu-id="61996-140">Read-only</span></span>|
|<span data-ttu-id="61996-141">version</span><span class="sxs-lookup"><span data-stu-id="61996-141">version</span></span>|<span data-ttu-id="61996-142">String</span><span class="sxs-lookup"><span data-stu-id="61996-142">String</span></span>|<span data-ttu-id="61996-143">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="61996-143">Version of the discovered application.</span></span> <span data-ttu-id="61996-144">只读</span><span class="sxs-lookup"><span data-stu-id="61996-144">Read-only</span></span>|
|<span data-ttu-id="61996-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="61996-145">sizeInByte</span></span>|<span data-ttu-id="61996-146">Int64</span><span class="sxs-lookup"><span data-stu-id="61996-146">Int64</span></span>|<span data-ttu-id="61996-147">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="61996-147">Discovered application size in bytes.</span></span> <span data-ttu-id="61996-148">只读</span><span class="sxs-lookup"><span data-stu-id="61996-148">Read-only</span></span>|
|<span data-ttu-id="61996-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="61996-149">deviceCount</span></span>|<span data-ttu-id="61996-150">Int32</span><span class="sxs-lookup"><span data-stu-id="61996-150">Int32</span></span>|<span data-ttu-id="61996-151">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="61996-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="61996-152">响应</span><span class="sxs-lookup"><span data-stu-id="61996-152">Response</span></span>
<span data-ttu-id="61996-153">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61996-153">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61996-154">示例</span><span class="sxs-lookup"><span data-stu-id="61996-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="61996-155">请求</span><span class="sxs-lookup"><span data-stu-id="61996-155">Request</span></span>
<span data-ttu-id="61996-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61996-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61996-157">响应</span><span class="sxs-lookup"><span data-stu-id="61996-157">Response</span></span>
<span data-ttu-id="61996-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61996-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




