---
title: 更新 detectedApp
description: 更新 detectedApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 277affa12d91ca51165e40324c74c2649801b3a9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146452"
---
# <a name="update-detectedapp"></a><span data-ttu-id="21842-103">更新 detectedApp</span><span class="sxs-lookup"><span data-stu-id="21842-103">Update detectedApp</span></span>

<span data-ttu-id="21842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21842-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21842-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21842-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21842-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21842-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21842-107">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="21842-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21842-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="21842-108">Prerequisites</span></span>
<span data-ttu-id="21842-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21842-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="21842-111">Permission type</span></span>|<span data-ttu-id="21842-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21842-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21842-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21842-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21842-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21842-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="21842-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21842-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21842-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21842-116">Not supported.</span></span>|
|<span data-ttu-id="21842-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="21842-117">Application</span></span>|<span data-ttu-id="21842-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21842-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21842-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21842-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="21842-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="21842-120">Request headers</span></span>
|<span data-ttu-id="21842-121">标头</span><span class="sxs-lookup"><span data-stu-id="21842-121">Header</span></span>|<span data-ttu-id="21842-122">值</span><span class="sxs-lookup"><span data-stu-id="21842-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21842-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21842-123">Authorization</span></span>|<span data-ttu-id="21842-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21842-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21842-125">接受</span><span class="sxs-lookup"><span data-stu-id="21842-125">Accept</span></span>|<span data-ttu-id="21842-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21842-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21842-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="21842-127">Request body</span></span>
<span data-ttu-id="21842-128">在请求正文中，提供 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21842-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="21842-129">下表显示创建 [detectedApp](../resources/intune-devices-detectedapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="21842-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="21842-130">属性</span><span class="sxs-lookup"><span data-stu-id="21842-130">Property</span></span>|<span data-ttu-id="21842-131">类型</span><span class="sxs-lookup"><span data-stu-id="21842-131">Type</span></span>|<span data-ttu-id="21842-132">说明</span><span class="sxs-lookup"><span data-stu-id="21842-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21842-133">id</span><span class="sxs-lookup"><span data-stu-id="21842-133">id</span></span>|<span data-ttu-id="21842-134">String</span><span class="sxs-lookup"><span data-stu-id="21842-134">String</span></span>|<span data-ttu-id="21842-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="21842-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="21842-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="21842-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="21842-137">只读。</span><span class="sxs-lookup"><span data-stu-id="21842-137">Read-only.</span></span>|
|<span data-ttu-id="21842-138">displayName</span><span class="sxs-lookup"><span data-stu-id="21842-138">displayName</span></span>|<span data-ttu-id="21842-139">String</span><span class="sxs-lookup"><span data-stu-id="21842-139">String</span></span>|<span data-ttu-id="21842-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="21842-140">Name of the discovered application.</span></span> <span data-ttu-id="21842-141">只读</span><span class="sxs-lookup"><span data-stu-id="21842-141">Read-only</span></span>|
|<span data-ttu-id="21842-142">version</span><span class="sxs-lookup"><span data-stu-id="21842-142">version</span></span>|<span data-ttu-id="21842-143">String</span><span class="sxs-lookup"><span data-stu-id="21842-143">String</span></span>|<span data-ttu-id="21842-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="21842-144">Version of the discovered application.</span></span> <span data-ttu-id="21842-145">只读</span><span class="sxs-lookup"><span data-stu-id="21842-145">Read-only</span></span>|
|<span data-ttu-id="21842-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="21842-146">sizeInByte</span></span>|<span data-ttu-id="21842-147">Int64</span><span class="sxs-lookup"><span data-stu-id="21842-147">Int64</span></span>|<span data-ttu-id="21842-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="21842-148">Discovered application size in bytes.</span></span> <span data-ttu-id="21842-149">只读</span><span class="sxs-lookup"><span data-stu-id="21842-149">Read-only</span></span>|
|<span data-ttu-id="21842-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="21842-150">deviceCount</span></span>|<span data-ttu-id="21842-151">Int32</span><span class="sxs-lookup"><span data-stu-id="21842-151">Int32</span></span>|<span data-ttu-id="21842-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="21842-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="21842-153">响应</span><span class="sxs-lookup"><span data-stu-id="21842-153">Response</span></span>
<span data-ttu-id="21842-154">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21842-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21842-155">示例</span><span class="sxs-lookup"><span data-stu-id="21842-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="21842-156">请求</span><span class="sxs-lookup"><span data-stu-id="21842-156">Request</span></span>
<span data-ttu-id="21842-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21842-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
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

### <a name="response"></a><span data-ttu-id="21842-158">响应</span><span class="sxs-lookup"><span data-stu-id="21842-158">Response</span></span>
<span data-ttu-id="21842-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21842-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




