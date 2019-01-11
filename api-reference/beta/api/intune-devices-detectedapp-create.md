---
title: 创建 detectedApp
description: 创建新的 detectedApp 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: da35940ba44790bdaec19a6c841bb5d90312b5f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856313"
---
# <a name="create-detectedapp"></a><span data-ttu-id="31daa-103">创建 detectedApp</span><span class="sxs-lookup"><span data-stu-id="31daa-103">Create detectedApp</span></span>

> <span data-ttu-id="31daa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="31daa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31daa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="31daa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31daa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="31daa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31daa-107">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31daa-107">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31daa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="31daa-108">Prerequisites</span></span>
<span data-ttu-id="31daa-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="31daa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31daa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="31daa-111">Permission type</span></span>|<span data-ttu-id="31daa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31daa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31daa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31daa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31daa-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31daa-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="31daa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31daa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31daa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31daa-116">Not supported.</span></span>|
|<span data-ttu-id="31daa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="31daa-117">Application</span></span>|<span data-ttu-id="31daa-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="31daa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31daa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31daa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="31daa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="31daa-120">Request headers</span></span>
|<span data-ttu-id="31daa-121">标头</span><span class="sxs-lookup"><span data-stu-id="31daa-121">Header</span></span>|<span data-ttu-id="31daa-122">值</span><span class="sxs-lookup"><span data-stu-id="31daa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31daa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31daa-123">Authorization</span></span>|<span data-ttu-id="31daa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31daa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31daa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31daa-125">Accept</span></span>|<span data-ttu-id="31daa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31daa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31daa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31daa-127">Request body</span></span>
<span data-ttu-id="31daa-128">在请求正文中，提供 detectedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31daa-128">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="31daa-129">下表显示创建 detectedApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="31daa-129">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="31daa-130">属性</span><span class="sxs-lookup"><span data-stu-id="31daa-130">Property</span></span>|<span data-ttu-id="31daa-131">类型</span><span class="sxs-lookup"><span data-stu-id="31daa-131">Type</span></span>|<span data-ttu-id="31daa-132">说明</span><span class="sxs-lookup"><span data-stu-id="31daa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31daa-133">id</span><span class="sxs-lookup"><span data-stu-id="31daa-133">id</span></span>|<span data-ttu-id="31daa-134">String</span><span class="sxs-lookup"><span data-stu-id="31daa-134">String</span></span>|<span data-ttu-id="31daa-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31daa-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="31daa-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="31daa-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="31daa-137">只读。</span><span class="sxs-lookup"><span data-stu-id="31daa-137">Read-only.</span></span>|
|<span data-ttu-id="31daa-138">displayName</span><span class="sxs-lookup"><span data-stu-id="31daa-138">displayName</span></span>|<span data-ttu-id="31daa-139">String</span><span class="sxs-lookup"><span data-stu-id="31daa-139">String</span></span>|<span data-ttu-id="31daa-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="31daa-140">Name of the discovered application.</span></span> <span data-ttu-id="31daa-141">只读</span><span class="sxs-lookup"><span data-stu-id="31daa-141">Read-only</span></span>|
|<span data-ttu-id="31daa-142">version</span><span class="sxs-lookup"><span data-stu-id="31daa-142">version</span></span>|<span data-ttu-id="31daa-143">String</span><span class="sxs-lookup"><span data-stu-id="31daa-143">String</span></span>|<span data-ttu-id="31daa-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="31daa-144">Version of the discovered application.</span></span> <span data-ttu-id="31daa-145">只读</span><span class="sxs-lookup"><span data-stu-id="31daa-145">Read-only</span></span>|
|<span data-ttu-id="31daa-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="31daa-146">sizeInByte</span></span>|<span data-ttu-id="31daa-147">Int64</span><span class="sxs-lookup"><span data-stu-id="31daa-147">Int64</span></span>|<span data-ttu-id="31daa-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="31daa-148">Discovered application size in bytes.</span></span> <span data-ttu-id="31daa-149">只读</span><span class="sxs-lookup"><span data-stu-id="31daa-149">Read-only</span></span>|
|<span data-ttu-id="31daa-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="31daa-150">deviceCount</span></span>|<span data-ttu-id="31daa-151">Int32</span><span class="sxs-lookup"><span data-stu-id="31daa-151">Int32</span></span>|<span data-ttu-id="31daa-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="31daa-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="31daa-153">响应</span><span class="sxs-lookup"><span data-stu-id="31daa-153">Response</span></span>
<span data-ttu-id="31daa-154">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31daa-154">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31daa-155">示例</span><span class="sxs-lookup"><span data-stu-id="31daa-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="31daa-156">请求</span><span class="sxs-lookup"><span data-stu-id="31daa-156">Request</span></span>
<span data-ttu-id="31daa-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31daa-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="31daa-158">响应</span><span class="sxs-lookup"><span data-stu-id="31daa-158">Response</span></span>
<span data-ttu-id="31daa-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31daa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





