---
title: 更新 deviceManagementScriptRunSummary
description: 更新 deviceManagementScriptRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecb6ebfda52ad87a7ac75af8915e3b6b8023442a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380122"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="fb469-103">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="fb469-103">Update deviceManagementScriptRunSummary</span></span>

<span data-ttu-id="fb469-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb469-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb469-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb469-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb469-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb469-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb469-107">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb469-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb469-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb469-108">Prerequisites</span></span>
<span data-ttu-id="fb469-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb469-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb469-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb469-111">Permission type</span></span>|<span data-ttu-id="fb469-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb469-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb469-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb469-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb469-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb469-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb469-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb469-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb469-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb469-116">Not supported.</span></span>|
|<span data-ttu-id="fb469-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb469-117">Application</span></span>|<span data-ttu-id="fb469-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb469-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb469-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb469-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="fb469-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb469-120">Request headers</span></span>
|<span data-ttu-id="fb469-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb469-121">Header</span></span>|<span data-ttu-id="fb469-122">值</span><span class="sxs-lookup"><span data-stu-id="fb469-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb469-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb469-123">Authorization</span></span>|<span data-ttu-id="fb469-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb469-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb469-125">接受</span><span class="sxs-lookup"><span data-stu-id="fb469-125">Accept</span></span>|<span data-ttu-id="fb469-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb469-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb469-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb469-127">Request body</span></span>
<span data-ttu-id="fb469-128">在请求正文中，提供[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb469-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="fb469-129">下表显示创建[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb469-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="fb469-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb469-130">Property</span></span>|<span data-ttu-id="fb469-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb469-131">Type</span></span>|<span data-ttu-id="fb469-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb469-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb469-133">id</span><span class="sxs-lookup"><span data-stu-id="fb469-133">id</span></span>|<span data-ttu-id="fb469-134">字符串</span><span class="sxs-lookup"><span data-stu-id="fb469-134">String</span></span>|<span data-ttu-id="fb469-135">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="fb469-135">Key of the device management script run summary entity.</span></span> <span data-ttu-id="fb469-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fb469-136">This property is read-only.</span></span>|
|<span data-ttu-id="fb469-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fb469-137">successDeviceCount</span></span>|<span data-ttu-id="fb469-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fb469-138">Int32</span></span>|<span data-ttu-id="fb469-139">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="fb469-139">Success device count.</span></span>|
|<span data-ttu-id="fb469-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fb469-140">errorDeviceCount</span></span>|<span data-ttu-id="fb469-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fb469-141">Int32</span></span>|<span data-ttu-id="fb469-142">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="fb469-142">Error device count.</span></span>|
|<span data-ttu-id="fb469-143">successUserCount</span><span class="sxs-lookup"><span data-stu-id="fb469-143">successUserCount</span></span>|<span data-ttu-id="fb469-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fb469-144">Int32</span></span>|<span data-ttu-id="fb469-145">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="fb469-145">Success user count.</span></span>|
|<span data-ttu-id="fb469-146">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="fb469-146">errorUserCount</span></span>|<span data-ttu-id="fb469-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fb469-147">Int32</span></span>|<span data-ttu-id="fb469-148">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="fb469-148">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="fb469-149">响应</span><span class="sxs-lookup"><span data-stu-id="fb469-149">Response</span></span>
<span data-ttu-id="fb469-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb469-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb469-151">示例</span><span class="sxs-lookup"><span data-stu-id="fb469-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb469-152">请求</span><span class="sxs-lookup"><span data-stu-id="fb469-152">Request</span></span>
<span data-ttu-id="fb469-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb469-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="fb469-154">响应</span><span class="sxs-lookup"><span data-stu-id="fb469-154">Response</span></span>
<span data-ttu-id="fb469-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb469-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```



