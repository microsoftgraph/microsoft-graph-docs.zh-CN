---
title: Update importedWindowsAutopilotDeviceIdentity
description: 更新 importedWindowsAutopilotDeviceIdentity 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a81e7b8291bab7698869c60d5403fd07be08cb5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261332"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="8f671-103">Update importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8f671-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="8f671-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f671-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f671-105">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8f671-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f671-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f671-106">Prerequisites</span></span>
<span data-ttu-id="8f671-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8f671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f671-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f671-109">Permission type</span></span>|<span data-ttu-id="8f671-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f671-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f671-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f671-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f671-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f671-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8f671-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f671-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f671-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f671-114">Not supported.</span></span>|
|<span data-ttu-id="8f671-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f671-115">Application</span></span>|<span data-ttu-id="8f671-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f671-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f671-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f671-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="8f671-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f671-118">Request headers</span></span>
|<span data-ttu-id="8f671-119">标头</span><span class="sxs-lookup"><span data-stu-id="8f671-119">Header</span></span>|<span data-ttu-id="8f671-120">值</span><span class="sxs-lookup"><span data-stu-id="8f671-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f671-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f671-121">Authorization</span></span>|<span data-ttu-id="8f671-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f671-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f671-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8f671-123">Accept</span></span>|<span data-ttu-id="8f671-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f671-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f671-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f671-125">Request body</span></span>
<span data-ttu-id="8f671-126">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f671-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="8f671-127">下表显示创建 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8f671-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="8f671-128">属性</span><span class="sxs-lookup"><span data-stu-id="8f671-128">Property</span></span>|<span data-ttu-id="8f671-129">类型</span><span class="sxs-lookup"><span data-stu-id="8f671-129">Type</span></span>|<span data-ttu-id="8f671-130">说明</span><span class="sxs-lookup"><span data-stu-id="8f671-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f671-131">id</span><span class="sxs-lookup"><span data-stu-id="8f671-131">id</span></span>|<span data-ttu-id="8f671-132">字符串</span><span class="sxs-lookup"><span data-stu-id="8f671-132">String</span></span>|<span data-ttu-id="8f671-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="8f671-133">The GUID for the object</span></span>|
|<span data-ttu-id="8f671-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="8f671-134">orderIdentifier</span></span>|<span data-ttu-id="8f671-135">String</span><span class="sxs-lookup"><span data-stu-id="8f671-135">String</span></span>|<span data-ttu-id="8f671-136">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="8f671-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f671-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="8f671-137">serialNumber</span></span>|<span data-ttu-id="8f671-138">String</span><span class="sxs-lookup"><span data-stu-id="8f671-138">String</span></span>|<span data-ttu-id="8f671-139">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="8f671-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f671-140">productKey</span><span class="sxs-lookup"><span data-stu-id="8f671-140">productKey</span></span>|<span data-ttu-id="8f671-141">字符串</span><span class="sxs-lookup"><span data-stu-id="8f671-141">String</span></span>|<span data-ttu-id="8f671-142">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="8f671-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f671-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="8f671-143">hardwareIdentifier</span></span>|<span data-ttu-id="8f671-144">Binary</span><span class="sxs-lookup"><span data-stu-id="8f671-144">Binary</span></span>|<span data-ttu-id="8f671-145">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="8f671-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f671-146">state</span><span class="sxs-lookup"><span data-stu-id="8f671-146">state</span></span>|[<span data-ttu-id="8f671-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="8f671-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="8f671-148">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="8f671-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="8f671-149">响应</span><span class="sxs-lookup"><span data-stu-id="8f671-149">Response</span></span>
<span data-ttu-id="8f671-150">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f671-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f671-151">示例</span><span class="sxs-lookup"><span data-stu-id="8f671-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f671-152">请求</span><span class="sxs-lookup"><span data-stu-id="8f671-152">Request</span></span>
<span data-ttu-id="8f671-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f671-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="8f671-154">响应</span><span class="sxs-lookup"><span data-stu-id="8f671-154">Response</span></span>
<span data-ttu-id="8f671-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f671-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



