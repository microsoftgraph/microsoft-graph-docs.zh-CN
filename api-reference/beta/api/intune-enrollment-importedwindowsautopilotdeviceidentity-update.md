---
title: Update importedWindowsAutopilotDeviceIdentity
description: 更新 importedWindowsAutopilotDeviceIdentity 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5fa7434a5ee9e5218e6bfd40bad6b6497b5f4b47
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404783"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="88404-103">Update importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="88404-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="88404-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="88404-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88404-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88404-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88404-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88404-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88404-107">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88404-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88404-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88404-108">Prerequisites</span></span>
<span data-ttu-id="88404-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="88404-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88404-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88404-111">Permission type</span></span>|<span data-ttu-id="88404-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88404-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88404-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88404-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88404-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88404-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88404-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88404-116">Not supported.</span></span>|
|<span data-ttu-id="88404-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88404-117">Application</span></span>|<span data-ttu-id="88404-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="88404-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88404-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="88404-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88404-120">Request headers</span></span>
|<span data-ttu-id="88404-121">标头</span><span class="sxs-lookup"><span data-stu-id="88404-121">Header</span></span>|<span data-ttu-id="88404-122">值</span><span class="sxs-lookup"><span data-stu-id="88404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88404-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88404-123">Authorization</span></span>|<span data-ttu-id="88404-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88404-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88404-125">Accept</span></span>|<span data-ttu-id="88404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88404-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88404-127">Request body</span></span>
<span data-ttu-id="88404-128">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88404-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="88404-129">下表显示创建 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88404-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="88404-130">属性</span><span class="sxs-lookup"><span data-stu-id="88404-130">Property</span></span>|<span data-ttu-id="88404-131">类型</span><span class="sxs-lookup"><span data-stu-id="88404-131">Type</span></span>|<span data-ttu-id="88404-132">说明</span><span class="sxs-lookup"><span data-stu-id="88404-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88404-133">id</span><span class="sxs-lookup"><span data-stu-id="88404-133">id</span></span>|<span data-ttu-id="88404-134">String</span><span class="sxs-lookup"><span data-stu-id="88404-134">String</span></span>|<span data-ttu-id="88404-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="88404-135">The GUID for the object</span></span>|
|<span data-ttu-id="88404-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="88404-136">orderIdentifier</span></span>|<span data-ttu-id="88404-137">String</span><span class="sxs-lookup"><span data-stu-id="88404-137">String</span></span>|<span data-ttu-id="88404-138">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="88404-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="88404-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="88404-139">serialNumber</span></span>|<span data-ttu-id="88404-140">String</span><span class="sxs-lookup"><span data-stu-id="88404-140">String</span></span>|<span data-ttu-id="88404-141">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="88404-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="88404-142">productKey</span><span class="sxs-lookup"><span data-stu-id="88404-142">productKey</span></span>|<span data-ttu-id="88404-143">String</span><span class="sxs-lookup"><span data-stu-id="88404-143">String</span></span>|<span data-ttu-id="88404-144">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="88404-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="88404-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="88404-145">hardwareIdentifier</span></span>|<span data-ttu-id="88404-146">Binary</span><span class="sxs-lookup"><span data-stu-id="88404-146">Binary</span></span>|<span data-ttu-id="88404-147">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="88404-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="88404-148">state</span><span class="sxs-lookup"><span data-stu-id="88404-148">state</span></span>|[<span data-ttu-id="88404-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="88404-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="88404-150">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="88404-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="88404-151">响应</span><span class="sxs-lookup"><span data-stu-id="88404-151">Response</span></span>
<span data-ttu-id="88404-152">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88404-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88404-153">示例</span><span class="sxs-lookup"><span data-stu-id="88404-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="88404-154">请求</span><span class="sxs-lookup"><span data-stu-id="88404-154">Request</span></span>
<span data-ttu-id="88404-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88404-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="88404-156">响应</span><span class="sxs-lookup"><span data-stu-id="88404-156">Response</span></span>
<span data-ttu-id="88404-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88404-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




