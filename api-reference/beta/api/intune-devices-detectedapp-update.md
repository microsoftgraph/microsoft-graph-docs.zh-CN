---
title: 更新 detectedApp
description: 更新 detectedApp 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7bfea341aafb25ea010162d270eab451900c0d04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394941"
---
# <a name="update-detectedapp"></a><span data-ttu-id="b5d8f-103">更新 detectedApp</span><span class="sxs-lookup"><span data-stu-id="b5d8f-103">Update detectedApp</span></span>

> <span data-ttu-id="b5d8f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5d8f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5d8f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5d8f-107">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5d8f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5d8f-108">Prerequisites</span></span>
<span data-ttu-id="b5d8f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b5d8f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5d8f-111">Permission type</span></span>|<span data-ttu-id="b5d8f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5d8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5d8f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5d8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5d8f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d8f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b5d8f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5d8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5d8f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-116">Not supported.</span></span>|
|<span data-ttu-id="b5d8f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5d8f-117">Application</span></span>|<span data-ttu-id="b5d8f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5d8f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5d8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b5d8f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5d8f-120">Request headers</span></span>
|<span data-ttu-id="b5d8f-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5d8f-121">Header</span></span>|<span data-ttu-id="b5d8f-122">值</span><span class="sxs-lookup"><span data-stu-id="b5d8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5d8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d8f-123">Authorization</span></span>|<span data-ttu-id="b5d8f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5d8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b5d8f-125">Accept</span></span>|<span data-ttu-id="b5d8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5d8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5d8f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5d8f-127">Request body</span></span>
<span data-ttu-id="b5d8f-128">在请求正文中，提供 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="b5d8f-129">下表显示创建 [detectedApp](../resources/intune-devices-detectedapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="b5d8f-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5d8f-130">Property</span></span>|<span data-ttu-id="b5d8f-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5d8f-131">Type</span></span>|<span data-ttu-id="b5d8f-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5d8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5d8f-133">id</span><span class="sxs-lookup"><span data-stu-id="b5d8f-133">id</span></span>|<span data-ttu-id="b5d8f-134">String</span><span class="sxs-lookup"><span data-stu-id="b5d8f-134">String</span></span>|<span data-ttu-id="b5d8f-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="b5d8f-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="b5d8f-137">只读。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-137">Read-only.</span></span>|
|<span data-ttu-id="b5d8f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b5d8f-138">displayName</span></span>|<span data-ttu-id="b5d8f-139">String</span><span class="sxs-lookup"><span data-stu-id="b5d8f-139">String</span></span>|<span data-ttu-id="b5d8f-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-140">Name of the discovered application.</span></span> <span data-ttu-id="b5d8f-141">只读</span><span class="sxs-lookup"><span data-stu-id="b5d8f-141">Read-only</span></span>|
|<span data-ttu-id="b5d8f-142">version</span><span class="sxs-lookup"><span data-stu-id="b5d8f-142">version</span></span>|<span data-ttu-id="b5d8f-143">String</span><span class="sxs-lookup"><span data-stu-id="b5d8f-143">String</span></span>|<span data-ttu-id="b5d8f-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-144">Version of the discovered application.</span></span> <span data-ttu-id="b5d8f-145">只读</span><span class="sxs-lookup"><span data-stu-id="b5d8f-145">Read-only</span></span>|
|<span data-ttu-id="b5d8f-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="b5d8f-146">sizeInByte</span></span>|<span data-ttu-id="b5d8f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="b5d8f-147">Int64</span></span>|<span data-ttu-id="b5d8f-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-148">Discovered application size in bytes.</span></span> <span data-ttu-id="b5d8f-149">只读</span><span class="sxs-lookup"><span data-stu-id="b5d8f-149">Read-only</span></span>|
|<span data-ttu-id="b5d8f-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b5d8f-150">deviceCount</span></span>|<span data-ttu-id="b5d8f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b5d8f-151">Int32</span></span>|<span data-ttu-id="b5d8f-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="b5d8f-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="b5d8f-153">响应</span><span class="sxs-lookup"><span data-stu-id="b5d8f-153">Response</span></span>
<span data-ttu-id="b5d8f-154">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5d8f-155">示例</span><span class="sxs-lookup"><span data-stu-id="b5d8f-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5d8f-156">请求</span><span class="sxs-lookup"><span data-stu-id="b5d8f-156">Request</span></span>
<span data-ttu-id="b5d8f-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5d8f-158">响应</span><span class="sxs-lookup"><span data-stu-id="b5d8f-158">Response</span></span>
<span data-ttu-id="b5d8f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5d8f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




