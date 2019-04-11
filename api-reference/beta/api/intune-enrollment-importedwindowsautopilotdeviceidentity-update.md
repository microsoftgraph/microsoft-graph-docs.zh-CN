---
title: Update importedWindowsAutopilotDeviceIdentity
description: 更新 importedWindowsAutopilotDeviceIdentity 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18bb8a3ffbae8c191344a3d24fdac85a51d3e82f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776036"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="94cb5-103">Update importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="94cb5-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="94cb5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94cb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94cb5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94cb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94cb5-106">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94cb5-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94cb5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="94cb5-107">Prerequisites</span></span>
<span data-ttu-id="94cb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94cb5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94cb5-110">Permission type</span></span>|<span data-ttu-id="94cb5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="94cb5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94cb5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94cb5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94cb5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94cb5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94cb5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94cb5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94cb5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94cb5-115">Not supported.</span></span>|
|<span data-ttu-id="94cb5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94cb5-116">Application</span></span>|<span data-ttu-id="94cb5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="94cb5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94cb5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94cb5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="94cb5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94cb5-119">Request headers</span></span>
|<span data-ttu-id="94cb5-120">标头</span><span class="sxs-lookup"><span data-stu-id="94cb5-120">Header</span></span>|<span data-ttu-id="94cb5-121">值</span><span class="sxs-lookup"><span data-stu-id="94cb5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94cb5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94cb5-122">Authorization</span></span>|<span data-ttu-id="94cb5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94cb5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94cb5-124">接受</span><span class="sxs-lookup"><span data-stu-id="94cb5-124">Accept</span></span>|<span data-ttu-id="94cb5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94cb5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94cb5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="94cb5-126">Request body</span></span>
<span data-ttu-id="94cb5-127">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94cb5-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="94cb5-128">下表显示创建 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="94cb5-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="94cb5-129">属性</span><span class="sxs-lookup"><span data-stu-id="94cb5-129">Property</span></span>|<span data-ttu-id="94cb5-130">类型</span><span class="sxs-lookup"><span data-stu-id="94cb5-130">Type</span></span>|<span data-ttu-id="94cb5-131">说明</span><span class="sxs-lookup"><span data-stu-id="94cb5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94cb5-132">id</span><span class="sxs-lookup"><span data-stu-id="94cb5-132">id</span></span>|<span data-ttu-id="94cb5-133">String</span><span class="sxs-lookup"><span data-stu-id="94cb5-133">String</span></span>|<span data-ttu-id="94cb5-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="94cb5-134">The GUID for the object</span></span>|
|<span data-ttu-id="94cb5-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="94cb5-135">orderIdentifier</span></span>|<span data-ttu-id="94cb5-136">String</span><span class="sxs-lookup"><span data-stu-id="94cb5-136">String</span></span>|<span data-ttu-id="94cb5-137">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="94cb5-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94cb5-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="94cb5-138">serialNumber</span></span>|<span data-ttu-id="94cb5-139">String</span><span class="sxs-lookup"><span data-stu-id="94cb5-139">String</span></span>|<span data-ttu-id="94cb5-140">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="94cb5-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94cb5-141">productKey</span><span class="sxs-lookup"><span data-stu-id="94cb5-141">productKey</span></span>|<span data-ttu-id="94cb5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="94cb5-142">String</span></span>|<span data-ttu-id="94cb5-143">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="94cb5-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94cb5-144">importId</span><span class="sxs-lookup"><span data-stu-id="94cb5-144">importId</span></span>|<span data-ttu-id="94cb5-145">String</span><span class="sxs-lookup"><span data-stu-id="94cb5-145">String</span></span>|<span data-ttu-id="94cb5-146">Windows autopilot 设备的导入 Id。</span><span class="sxs-lookup"><span data-stu-id="94cb5-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94cb5-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="94cb5-147">hardwareIdentifier</span></span>|<span data-ttu-id="94cb5-148">Binary</span><span class="sxs-lookup"><span data-stu-id="94cb5-148">Binary</span></span>|<span data-ttu-id="94cb5-149">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="94cb5-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="94cb5-150">state</span><span class="sxs-lookup"><span data-stu-id="94cb5-150">state</span></span>|[<span data-ttu-id="94cb5-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="94cb5-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="94cb5-152">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="94cb5-152">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="94cb5-153">响应</span><span class="sxs-lookup"><span data-stu-id="94cb5-153">Response</span></span>
<span data-ttu-id="94cb5-154">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94cb5-154">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94cb5-155">示例</span><span class="sxs-lookup"><span data-stu-id="94cb5-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="94cb5-156">请求</span><span class="sxs-lookup"><span data-stu-id="94cb5-156">Request</span></span>
<span data-ttu-id="94cb5-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94cb5-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "importId": "Import Id value",
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

### <a name="response"></a><span data-ttu-id="94cb5-158">响应</span><span class="sxs-lookup"><span data-stu-id="94cb5-158">Response</span></span>
<span data-ttu-id="94cb5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94cb5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "importId": "Import Id value",
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





