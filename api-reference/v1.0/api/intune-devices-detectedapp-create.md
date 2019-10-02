---
title: 创建 detectedApp
description: 创建新的 detectedApp 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81eafad351604335d125bc01d7f314aa7a19b02c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364597"
---
# <a name="create-detectedapp"></a><span data-ttu-id="44171-103">创建 detectedApp</span><span class="sxs-lookup"><span data-stu-id="44171-103">Create detectedApp</span></span>

> <span data-ttu-id="44171-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44171-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44171-105">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44171-105">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44171-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="44171-106">Prerequisites</span></span>
<span data-ttu-id="44171-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44171-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44171-109">Permission type</span></span>|<span data-ttu-id="44171-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44171-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44171-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44171-111">Delegated (work or school account)</span></span>|<span data-ttu-id="44171-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44171-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44171-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44171-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44171-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="44171-114">Not supported.</span></span>|
|<span data-ttu-id="44171-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44171-115">Application</span></span>|<span data-ttu-id="44171-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44171-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44171-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44171-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="44171-118">请求头</span><span class="sxs-lookup"><span data-stu-id="44171-118">Request headers</span></span>
|<span data-ttu-id="44171-119">标头</span><span class="sxs-lookup"><span data-stu-id="44171-119">Header</span></span>|<span data-ttu-id="44171-120">值</span><span class="sxs-lookup"><span data-stu-id="44171-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44171-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44171-121">Authorization</span></span>|<span data-ttu-id="44171-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44171-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44171-123">接受</span><span class="sxs-lookup"><span data-stu-id="44171-123">Accept</span></span>|<span data-ttu-id="44171-124">application/json</span><span class="sxs-lookup"><span data-stu-id="44171-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44171-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="44171-125">Request body</span></span>
<span data-ttu-id="44171-126">在请求正文中，提供 detectedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44171-126">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="44171-127">下表显示创建 detectedApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44171-127">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="44171-128">属性</span><span class="sxs-lookup"><span data-stu-id="44171-128">Property</span></span>|<span data-ttu-id="44171-129">类型</span><span class="sxs-lookup"><span data-stu-id="44171-129">Type</span></span>|<span data-ttu-id="44171-130">说明</span><span class="sxs-lookup"><span data-stu-id="44171-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44171-131">id</span><span class="sxs-lookup"><span data-stu-id="44171-131">id</span></span>|<span data-ttu-id="44171-132">String</span><span class="sxs-lookup"><span data-stu-id="44171-132">String</span></span>|<span data-ttu-id="44171-133">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="44171-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="44171-134">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="44171-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="44171-135">只读。</span><span class="sxs-lookup"><span data-stu-id="44171-135">Read-only.</span></span>|
|<span data-ttu-id="44171-136">displayName</span><span class="sxs-lookup"><span data-stu-id="44171-136">displayName</span></span>|<span data-ttu-id="44171-137">字符串</span><span class="sxs-lookup"><span data-stu-id="44171-137">String</span></span>|<span data-ttu-id="44171-138">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="44171-138">Name of the discovered application.</span></span> <span data-ttu-id="44171-139">只读</span><span class="sxs-lookup"><span data-stu-id="44171-139">Read-only</span></span>|
|<span data-ttu-id="44171-140">version</span><span class="sxs-lookup"><span data-stu-id="44171-140">version</span></span>|<span data-ttu-id="44171-141">String</span><span class="sxs-lookup"><span data-stu-id="44171-141">String</span></span>|<span data-ttu-id="44171-142">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="44171-142">Version of the discovered application.</span></span> <span data-ttu-id="44171-143">只读</span><span class="sxs-lookup"><span data-stu-id="44171-143">Read-only</span></span>|
|<span data-ttu-id="44171-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="44171-144">sizeInByte</span></span>|<span data-ttu-id="44171-145">Int64</span><span class="sxs-lookup"><span data-stu-id="44171-145">Int64</span></span>|<span data-ttu-id="44171-146">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="44171-146">Discovered application size in bytes.</span></span> <span data-ttu-id="44171-147">只读</span><span class="sxs-lookup"><span data-stu-id="44171-147">Read-only</span></span>|
|<span data-ttu-id="44171-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="44171-148">deviceCount</span></span>|<span data-ttu-id="44171-149">Int32</span><span class="sxs-lookup"><span data-stu-id="44171-149">Int32</span></span>|<span data-ttu-id="44171-150">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="44171-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="44171-151">响应</span><span class="sxs-lookup"><span data-stu-id="44171-151">Response</span></span>
<span data-ttu-id="44171-152">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44171-152">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44171-153">示例</span><span class="sxs-lookup"><span data-stu-id="44171-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="44171-154">请求</span><span class="sxs-lookup"><span data-stu-id="44171-154">Request</span></span>
<span data-ttu-id="44171-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44171-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="44171-156">响应</span><span class="sxs-lookup"><span data-stu-id="44171-156">Response</span></span>
<span data-ttu-id="44171-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44171-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




