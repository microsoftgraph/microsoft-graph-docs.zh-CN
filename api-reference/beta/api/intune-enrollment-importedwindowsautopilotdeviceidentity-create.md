---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新importedWindowsAutopilotDeviceIdentity对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c951e6b0489d5d42035d6f415efe64a8b6fb5d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400723"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="1fae8-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="1fae8-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="1fae8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1fae8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1fae8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1fae8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fae8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fae8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fae8-107">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fae8-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fae8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fae8-108">Prerequisites</span></span>
<span data-ttu-id="1fae8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1fae8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1fae8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fae8-111">Permission type</span></span>|<span data-ttu-id="1fae8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1fae8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fae8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fae8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fae8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fae8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1fae8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fae8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fae8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fae8-116">Not supported.</span></span>|
|<span data-ttu-id="1fae8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fae8-117">Application</span></span>|<span data-ttu-id="1fae8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fae8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fae8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fae8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1fae8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fae8-120">Request headers</span></span>
|<span data-ttu-id="1fae8-121">标头</span><span class="sxs-lookup"><span data-stu-id="1fae8-121">Header</span></span>|<span data-ttu-id="1fae8-122">值</span><span class="sxs-lookup"><span data-stu-id="1fae8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fae8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fae8-123">Authorization</span></span>|<span data-ttu-id="1fae8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1fae8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fae8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fae8-125">Accept</span></span>|<span data-ttu-id="1fae8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fae8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fae8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fae8-127">Request body</span></span>
<span data-ttu-id="1fae8-128">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fae8-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="1fae8-129">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1fae8-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="1fae8-130">属性</span><span class="sxs-lookup"><span data-stu-id="1fae8-130">Property</span></span>|<span data-ttu-id="1fae8-131">类型</span><span class="sxs-lookup"><span data-stu-id="1fae8-131">Type</span></span>|<span data-ttu-id="1fae8-132">说明</span><span class="sxs-lookup"><span data-stu-id="1fae8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fae8-133">id</span><span class="sxs-lookup"><span data-stu-id="1fae8-133">id</span></span>|<span data-ttu-id="1fae8-134">String</span><span class="sxs-lookup"><span data-stu-id="1fae8-134">String</span></span>|<span data-ttu-id="1fae8-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="1fae8-135">The GUID for the object</span></span>|
|<span data-ttu-id="1fae8-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1fae8-136">orderIdentifier</span></span>|<span data-ttu-id="1fae8-137">String</span><span class="sxs-lookup"><span data-stu-id="1fae8-137">String</span></span>|<span data-ttu-id="1fae8-138">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="1fae8-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1fae8-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1fae8-139">serialNumber</span></span>|<span data-ttu-id="1fae8-140">String</span><span class="sxs-lookup"><span data-stu-id="1fae8-140">String</span></span>|<span data-ttu-id="1fae8-141">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="1fae8-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1fae8-142">productKey</span><span class="sxs-lookup"><span data-stu-id="1fae8-142">productKey</span></span>|<span data-ttu-id="1fae8-143">String</span><span class="sxs-lookup"><span data-stu-id="1fae8-143">String</span></span>|<span data-ttu-id="1fae8-144">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="1fae8-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1fae8-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="1fae8-145">hardwareIdentifier</span></span>|<span data-ttu-id="1fae8-146">Binary</span><span class="sxs-lookup"><span data-stu-id="1fae8-146">Binary</span></span>|<span data-ttu-id="1fae8-147">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="1fae8-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1fae8-148">state</span><span class="sxs-lookup"><span data-stu-id="1fae8-148">state</span></span>|[<span data-ttu-id="1fae8-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="1fae8-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="1fae8-150">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="1fae8-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="1fae8-151">响应</span><span class="sxs-lookup"><span data-stu-id="1fae8-151">Response</span></span>
<span data-ttu-id="1fae8-152">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fae8-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fae8-153">示例</span><span class="sxs-lookup"><span data-stu-id="1fae8-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fae8-154">请求</span><span class="sxs-lookup"><span data-stu-id="1fae8-154">Request</span></span>
<span data-ttu-id="1fae8-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fae8-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="1fae8-156">响应</span><span class="sxs-lookup"><span data-stu-id="1fae8-156">Response</span></span>
<span data-ttu-id="1fae8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fae8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




