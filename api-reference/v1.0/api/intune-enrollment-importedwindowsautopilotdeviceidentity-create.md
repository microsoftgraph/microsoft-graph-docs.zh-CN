---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新的 importedWindowsAutopilotDeviceIdentity 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 664b0d52eea5d61918e234c9fa582fa57f50d8b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980094"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="3a240-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3a240-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="3a240-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a240-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a240-105">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a240-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a240-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3a240-106">Prerequisites</span></span>
<span data-ttu-id="3a240-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a240-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a240-109">Permission type</span></span>|<span data-ttu-id="3a240-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3a240-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a240-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a240-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a240-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a240-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a240-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a240-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a240-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a240-114">Not supported.</span></span>|
|<span data-ttu-id="3a240-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a240-115">Application</span></span>|<span data-ttu-id="3a240-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a240-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a240-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a240-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="3a240-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a240-118">Request headers</span></span>
|<span data-ttu-id="3a240-119">标头</span><span class="sxs-lookup"><span data-stu-id="3a240-119">Header</span></span>|<span data-ttu-id="3a240-120">值</span><span class="sxs-lookup"><span data-stu-id="3a240-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a240-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a240-121">Authorization</span></span>|<span data-ttu-id="3a240-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3a240-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a240-123">接受</span><span class="sxs-lookup"><span data-stu-id="3a240-123">Accept</span></span>|<span data-ttu-id="3a240-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a240-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a240-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a240-125">Request body</span></span>
<span data-ttu-id="3a240-126">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a240-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="3a240-127">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3a240-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="3a240-128">属性</span><span class="sxs-lookup"><span data-stu-id="3a240-128">Property</span></span>|<span data-ttu-id="3a240-129">类型</span><span class="sxs-lookup"><span data-stu-id="3a240-129">Type</span></span>|<span data-ttu-id="3a240-130">说明</span><span class="sxs-lookup"><span data-stu-id="3a240-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a240-131">id</span><span class="sxs-lookup"><span data-stu-id="3a240-131">id</span></span>|<span data-ttu-id="3a240-132">String</span><span class="sxs-lookup"><span data-stu-id="3a240-132">String</span></span>|<span data-ttu-id="3a240-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="3a240-133">The GUID for the object</span></span>|
|<span data-ttu-id="3a240-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="3a240-134">orderIdentifier</span></span>|<span data-ttu-id="3a240-135">String</span><span class="sxs-lookup"><span data-stu-id="3a240-135">String</span></span>|<span data-ttu-id="3a240-136">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="3a240-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="3a240-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="3a240-137">serialNumber</span></span>|<span data-ttu-id="3a240-138">String</span><span class="sxs-lookup"><span data-stu-id="3a240-138">String</span></span>|<span data-ttu-id="3a240-139">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="3a240-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="3a240-140">productKey</span><span class="sxs-lookup"><span data-stu-id="3a240-140">productKey</span></span>|<span data-ttu-id="3a240-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3a240-141">String</span></span>|<span data-ttu-id="3a240-142">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="3a240-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="3a240-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="3a240-143">hardwareIdentifier</span></span>|<span data-ttu-id="3a240-144">Binary</span><span class="sxs-lookup"><span data-stu-id="3a240-144">Binary</span></span>|<span data-ttu-id="3a240-145">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="3a240-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="3a240-146">state</span><span class="sxs-lookup"><span data-stu-id="3a240-146">state</span></span>|[<span data-ttu-id="3a240-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="3a240-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="3a240-148">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="3a240-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="3a240-149">响应</span><span class="sxs-lookup"><span data-stu-id="3a240-149">Response</span></span>
<span data-ttu-id="3a240-150">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a240-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a240-151">示例</span><span class="sxs-lookup"><span data-stu-id="3a240-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a240-152">请求</span><span class="sxs-lookup"><span data-stu-id="3a240-152">Request</span></span>
<span data-ttu-id="3a240-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a240-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="3a240-154">响应</span><span class="sxs-lookup"><span data-stu-id="3a240-154">Response</span></span>
<span data-ttu-id="3a240-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a240-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```



