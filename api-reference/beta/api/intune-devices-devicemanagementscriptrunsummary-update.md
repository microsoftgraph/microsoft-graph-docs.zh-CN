---
title: 更新 deviceManagementScriptRunSummary
description: 更新 deviceManagementScriptRunSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6cc0ca082152168bf44a5f0da5b4c5a307ed0ac
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530347"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="69546-103">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="69546-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="69546-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69546-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69546-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69546-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69546-106">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69546-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69546-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69546-107">Prerequisites</span></span>
<span data-ttu-id="69546-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69546-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69546-110">Permission type</span></span>|<span data-ttu-id="69546-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69546-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69546-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69546-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69546-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69546-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69546-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69546-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69546-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69546-115">Not supported.</span></span>|
|<span data-ttu-id="69546-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69546-116">Application</span></span>|<span data-ttu-id="69546-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69546-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69546-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69546-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="69546-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="69546-119">Request headers</span></span>
|<span data-ttu-id="69546-120">标头</span><span class="sxs-lookup"><span data-stu-id="69546-120">Header</span></span>|<span data-ttu-id="69546-121">值</span><span class="sxs-lookup"><span data-stu-id="69546-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69546-122">授权</span><span class="sxs-lookup"><span data-stu-id="69546-122">Authorization</span></span>|<span data-ttu-id="69546-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69546-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69546-124">接受</span><span class="sxs-lookup"><span data-stu-id="69546-124">Accept</span></span>|<span data-ttu-id="69546-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69546-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69546-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69546-126">Request body</span></span>
<span data-ttu-id="69546-127">在请求正文中，提供[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69546-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="69546-128">下表显示创建[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69546-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="69546-129">属性</span><span class="sxs-lookup"><span data-stu-id="69546-129">Property</span></span>|<span data-ttu-id="69546-130">类型</span><span class="sxs-lookup"><span data-stu-id="69546-130">Type</span></span>|<span data-ttu-id="69546-131">说明</span><span class="sxs-lookup"><span data-stu-id="69546-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69546-132">id</span><span class="sxs-lookup"><span data-stu-id="69546-132">id</span></span>|<span data-ttu-id="69546-133">字符串</span><span class="sxs-lookup"><span data-stu-id="69546-133">String</span></span>|<span data-ttu-id="69546-134">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="69546-134">Key of the device management script run summary entity.</span></span> <span data-ttu-id="69546-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="69546-135">This property is read-only.</span></span>|
|<span data-ttu-id="69546-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69546-136">successDeviceCount</span></span>|<span data-ttu-id="69546-137">Int32</span><span class="sxs-lookup"><span data-stu-id="69546-137">Int32</span></span>|<span data-ttu-id="69546-138">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="69546-138">Success device count.</span></span>|
|<span data-ttu-id="69546-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69546-139">errorDeviceCount</span></span>|<span data-ttu-id="69546-140">Int32</span><span class="sxs-lookup"><span data-stu-id="69546-140">Int32</span></span>|<span data-ttu-id="69546-141">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="69546-141">Error device count.</span></span>|
|<span data-ttu-id="69546-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="69546-142">successUserCount</span></span>|<span data-ttu-id="69546-143">Int32</span><span class="sxs-lookup"><span data-stu-id="69546-143">Int32</span></span>|<span data-ttu-id="69546-144">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="69546-144">Success user count.</span></span>|
|<span data-ttu-id="69546-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="69546-145">errorUserCount</span></span>|<span data-ttu-id="69546-146">Int32</span><span class="sxs-lookup"><span data-stu-id="69546-146">Int32</span></span>|<span data-ttu-id="69546-147">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="69546-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="69546-148">响应</span><span class="sxs-lookup"><span data-stu-id="69546-148">Response</span></span>
<span data-ttu-id="69546-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69546-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69546-150">示例</span><span class="sxs-lookup"><span data-stu-id="69546-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="69546-151">请求</span><span class="sxs-lookup"><span data-stu-id="69546-151">Request</span></span>
<span data-ttu-id="69546-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69546-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
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

### <a name="response"></a><span data-ttu-id="69546-153">响应</span><span class="sxs-lookup"><span data-stu-id="69546-153">Response</span></span>
<span data-ttu-id="69546-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69546-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






