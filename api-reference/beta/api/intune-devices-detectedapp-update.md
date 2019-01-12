---
title: 更新 detectedApp
description: 更新 detectedApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 77bfb3880db9b7e36c8e6b9e8d2a8b53ab3450d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914995"
---
# <a name="update-detectedapp"></a><span data-ttu-id="2a41f-103">更新 detectedApp</span><span class="sxs-lookup"><span data-stu-id="2a41f-103">Update detectedApp</span></span>

> <span data-ttu-id="2a41f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2a41f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a41f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2a41f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a41f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a41f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a41f-107">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a41f-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a41f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a41f-108">Prerequisites</span></span>
<span data-ttu-id="2a41f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2a41f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a41f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a41f-111">Permission type</span></span>|<span data-ttu-id="2a41f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a41f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a41f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a41f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a41f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a41f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2a41f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a41f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a41f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a41f-116">Not supported.</span></span>|
|<span data-ttu-id="2a41f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a41f-117">Application</span></span>|<span data-ttu-id="2a41f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a41f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a41f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a41f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2a41f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a41f-120">Request headers</span></span>
|<span data-ttu-id="2a41f-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a41f-121">Header</span></span>|<span data-ttu-id="2a41f-122">值</span><span class="sxs-lookup"><span data-stu-id="2a41f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a41f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a41f-123">Authorization</span></span>|<span data-ttu-id="2a41f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a41f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a41f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a41f-125">Accept</span></span>|<span data-ttu-id="2a41f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a41f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a41f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a41f-127">Request body</span></span>
<span data-ttu-id="2a41f-128">在请求正文中，提供 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a41f-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="2a41f-129">下表显示创建 [detectedApp](../resources/intune-devices-detectedapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a41f-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="2a41f-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a41f-130">Property</span></span>|<span data-ttu-id="2a41f-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a41f-131">Type</span></span>|<span data-ttu-id="2a41f-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a41f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a41f-133">id</span><span class="sxs-lookup"><span data-stu-id="2a41f-133">id</span></span>|<span data-ttu-id="2a41f-134">String</span><span class="sxs-lookup"><span data-stu-id="2a41f-134">String</span></span>|<span data-ttu-id="2a41f-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a41f-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="2a41f-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="2a41f-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="2a41f-137">只读。</span><span class="sxs-lookup"><span data-stu-id="2a41f-137">Read-only.</span></span>|
|<span data-ttu-id="2a41f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2a41f-138">displayName</span></span>|<span data-ttu-id="2a41f-139">String</span><span class="sxs-lookup"><span data-stu-id="2a41f-139">String</span></span>|<span data-ttu-id="2a41f-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="2a41f-140">Name of the discovered application.</span></span> <span data-ttu-id="2a41f-141">只读</span><span class="sxs-lookup"><span data-stu-id="2a41f-141">Read-only</span></span>|
|<span data-ttu-id="2a41f-142">version</span><span class="sxs-lookup"><span data-stu-id="2a41f-142">version</span></span>|<span data-ttu-id="2a41f-143">String</span><span class="sxs-lookup"><span data-stu-id="2a41f-143">String</span></span>|<span data-ttu-id="2a41f-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="2a41f-144">Version of the discovered application.</span></span> <span data-ttu-id="2a41f-145">只读</span><span class="sxs-lookup"><span data-stu-id="2a41f-145">Read-only</span></span>|
|<span data-ttu-id="2a41f-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="2a41f-146">sizeInByte</span></span>|<span data-ttu-id="2a41f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="2a41f-147">Int64</span></span>|<span data-ttu-id="2a41f-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="2a41f-148">Discovered application size in bytes.</span></span> <span data-ttu-id="2a41f-149">只读</span><span class="sxs-lookup"><span data-stu-id="2a41f-149">Read-only</span></span>|
|<span data-ttu-id="2a41f-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2a41f-150">deviceCount</span></span>|<span data-ttu-id="2a41f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2a41f-151">Int32</span></span>|<span data-ttu-id="2a41f-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="2a41f-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="2a41f-153">响应</span><span class="sxs-lookup"><span data-stu-id="2a41f-153">Response</span></span>
<span data-ttu-id="2a41f-154">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a41f-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a41f-155">示例</span><span class="sxs-lookup"><span data-stu-id="2a41f-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a41f-156">请求</span><span class="sxs-lookup"><span data-stu-id="2a41f-156">Request</span></span>
<span data-ttu-id="2a41f-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a41f-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 117

{
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2a41f-158">响应</span><span class="sxs-lookup"><span data-stu-id="2a41f-158">Response</span></span>
<span data-ttu-id="2a41f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a41f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





