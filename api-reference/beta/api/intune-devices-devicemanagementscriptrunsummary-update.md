---
title: 更新 deviceManagementScriptRunSummary
description: 更新 deviceManagementScriptRunSummary 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55582147aff81bc8d566634a5fb9fdc1ff4ff2fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413988"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="60f2b-103">更新 deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="60f2b-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="60f2b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="60f2b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60f2b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60f2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60f2b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60f2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60f2b-107">更新[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60f2b-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60f2b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60f2b-108">Prerequisites</span></span>
<span data-ttu-id="60f2b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="60f2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="60f2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60f2b-111">Permission type</span></span>|<span data-ttu-id="60f2b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60f2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60f2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60f2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60f2b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60f2b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="60f2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60f2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60f2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60f2b-116">Not supported.</span></span>|
|<span data-ttu-id="60f2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60f2b-117">Application</span></span>|<span data-ttu-id="60f2b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60f2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60f2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60f2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="60f2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60f2b-120">Request headers</span></span>
|<span data-ttu-id="60f2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="60f2b-121">Header</span></span>|<span data-ttu-id="60f2b-122">值</span><span class="sxs-lookup"><span data-stu-id="60f2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60f2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60f2b-123">Authorization</span></span>|<span data-ttu-id="60f2b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60f2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60f2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60f2b-125">Accept</span></span>|<span data-ttu-id="60f2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60f2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60f2b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60f2b-127">Request body</span></span>
<span data-ttu-id="60f2b-128">在请求正文中，提供[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60f2b-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="60f2b-129">下表显示时创建[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60f2b-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="60f2b-130">属性</span><span class="sxs-lookup"><span data-stu-id="60f2b-130">Property</span></span>|<span data-ttu-id="60f2b-131">类型</span><span class="sxs-lookup"><span data-stu-id="60f2b-131">Type</span></span>|<span data-ttu-id="60f2b-132">说明</span><span class="sxs-lookup"><span data-stu-id="60f2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60f2b-133">id</span><span class="sxs-lookup"><span data-stu-id="60f2b-133">id</span></span>|<span data-ttu-id="60f2b-134">String</span><span class="sxs-lookup"><span data-stu-id="60f2b-134">String</span></span>|<span data-ttu-id="60f2b-135">运行摘要实体的设备管理脚本的键。</span><span class="sxs-lookup"><span data-stu-id="60f2b-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="60f2b-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60f2b-136">successDeviceCount</span></span>|<span data-ttu-id="60f2b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="60f2b-137">Int32</span></span>|<span data-ttu-id="60f2b-138">成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="60f2b-138">Success device count.</span></span>|
|<span data-ttu-id="60f2b-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60f2b-139">errorDeviceCount</span></span>|<span data-ttu-id="60f2b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="60f2b-140">Int32</span></span>|<span data-ttu-id="60f2b-141">错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="60f2b-141">Error device count.</span></span>|
|<span data-ttu-id="60f2b-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="60f2b-142">successUserCount</span></span>|<span data-ttu-id="60f2b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="60f2b-143">Int32</span></span>|<span data-ttu-id="60f2b-144">成功用户计数。</span><span class="sxs-lookup"><span data-stu-id="60f2b-144">Success user count.</span></span>|
|<span data-ttu-id="60f2b-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="60f2b-145">errorUserCount</span></span>|<span data-ttu-id="60f2b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="60f2b-146">Int32</span></span>|<span data-ttu-id="60f2b-147">错误用户计数。</span><span class="sxs-lookup"><span data-stu-id="60f2b-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="60f2b-148">响应</span><span class="sxs-lookup"><span data-stu-id="60f2b-148">Response</span></span>
<span data-ttu-id="60f2b-149">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60f2b-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60f2b-150">示例</span><span class="sxs-lookup"><span data-stu-id="60f2b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="60f2b-151">请求</span><span class="sxs-lookup"><span data-stu-id="60f2b-151">Request</span></span>
<span data-ttu-id="60f2b-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60f2b-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60f2b-153">响应</span><span class="sxs-lookup"><span data-stu-id="60f2b-153">Response</span></span>
<span data-ttu-id="60f2b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60f2b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




