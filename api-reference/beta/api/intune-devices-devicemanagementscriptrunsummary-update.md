---
title: 更新 deviceManagementScriptRunSummary
description: 更新 deviceManagementScriptRunSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 040214d3236e877b9c7d12b63bda659058028244
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986339"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="8da6f-103">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="8da6f-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="8da6f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8da6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8da6f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8da6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8da6f-106">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8da6f-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8da6f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8da6f-107">Prerequisites</span></span>
<span data-ttu-id="8da6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8da6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da6f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8da6f-110">Permission type</span></span>|<span data-ttu-id="8da6f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8da6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8da6f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8da6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8da6f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da6f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8da6f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8da6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8da6f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8da6f-115">Not supported.</span></span>|
|<span data-ttu-id="8da6f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8da6f-116">Application</span></span>|<span data-ttu-id="8da6f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8da6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8da6f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8da6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="8da6f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8da6f-119">Request headers</span></span>
|<span data-ttu-id="8da6f-120">标头</span><span class="sxs-lookup"><span data-stu-id="8da6f-120">Header</span></span>|<span data-ttu-id="8da6f-121">值</span><span class="sxs-lookup"><span data-stu-id="8da6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8da6f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8da6f-122">Authorization</span></span>|<span data-ttu-id="8da6f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8da6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8da6f-124">接受</span><span class="sxs-lookup"><span data-stu-id="8da6f-124">Accept</span></span>|<span data-ttu-id="8da6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8da6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da6f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8da6f-126">Request body</span></span>
<span data-ttu-id="8da6f-127">在请求正文中, 提供[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8da6f-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="8da6f-128">下表显示创建[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8da6f-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="8da6f-129">属性</span><span class="sxs-lookup"><span data-stu-id="8da6f-129">Property</span></span>|<span data-ttu-id="8da6f-130">类型</span><span class="sxs-lookup"><span data-stu-id="8da6f-130">Type</span></span>|<span data-ttu-id="8da6f-131">说明</span><span class="sxs-lookup"><span data-stu-id="8da6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8da6f-132">id</span><span class="sxs-lookup"><span data-stu-id="8da6f-132">id</span></span>|<span data-ttu-id="8da6f-133">String</span><span class="sxs-lookup"><span data-stu-id="8da6f-133">String</span></span>|<span data-ttu-id="8da6f-134">设备管理脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="8da6f-134">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="8da6f-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8da6f-135">successDeviceCount</span></span>|<span data-ttu-id="8da6f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8da6f-136">Int32</span></span>|<span data-ttu-id="8da6f-137">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="8da6f-137">Success device count.</span></span>|
|<span data-ttu-id="8da6f-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8da6f-138">errorDeviceCount</span></span>|<span data-ttu-id="8da6f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8da6f-139">Int32</span></span>|<span data-ttu-id="8da6f-140">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="8da6f-140">Error device count.</span></span>|
|<span data-ttu-id="8da6f-141">successUserCount</span><span class="sxs-lookup"><span data-stu-id="8da6f-141">successUserCount</span></span>|<span data-ttu-id="8da6f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8da6f-142">Int32</span></span>|<span data-ttu-id="8da6f-143">成功的用户计数。</span><span class="sxs-lookup"><span data-stu-id="8da6f-143">Success user count.</span></span>|
|<span data-ttu-id="8da6f-144">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="8da6f-144">errorUserCount</span></span>|<span data-ttu-id="8da6f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8da6f-145">Int32</span></span>|<span data-ttu-id="8da6f-146">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="8da6f-146">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="8da6f-147">响应</span><span class="sxs-lookup"><span data-stu-id="8da6f-147">Response</span></span>
<span data-ttu-id="8da6f-148">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8da6f-148">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8da6f-149">示例</span><span class="sxs-lookup"><span data-stu-id="8da6f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8da6f-150">请求</span><span class="sxs-lookup"><span data-stu-id="8da6f-150">Request</span></span>
<span data-ttu-id="8da6f-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8da6f-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8da6f-152">响应</span><span class="sxs-lookup"><span data-stu-id="8da6f-152">Response</span></span>
<span data-ttu-id="8da6f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8da6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




