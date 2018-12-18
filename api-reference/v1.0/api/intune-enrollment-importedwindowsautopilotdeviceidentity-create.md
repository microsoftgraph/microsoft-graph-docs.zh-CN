---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新importedWindowsAutopilotDeviceIdentity对象。
author: tfitzmac
ms.openlocfilehash: 10dbaed9d10a0b37df9e229d501bb6e469847ea5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334291"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="92d08-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="92d08-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="92d08-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="92d08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92d08-105">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92d08-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92d08-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="92d08-106">Prerequisites</span></span>
<span data-ttu-id="92d08-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="92d08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d08-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="92d08-109">Permission type</span></span>|<span data-ttu-id="92d08-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92d08-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92d08-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92d08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92d08-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d08-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="92d08-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92d08-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92d08-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="92d08-114">Not supported.</span></span>|
|<span data-ttu-id="92d08-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="92d08-115">Application</span></span>|<span data-ttu-id="92d08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92d08-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92d08-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92d08-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="92d08-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="92d08-118">Request headers</span></span>
|<span data-ttu-id="92d08-119">标头</span><span class="sxs-lookup"><span data-stu-id="92d08-119">Header</span></span>|<span data-ttu-id="92d08-120">值</span><span class="sxs-lookup"><span data-stu-id="92d08-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92d08-121">授权</span><span class="sxs-lookup"><span data-stu-id="92d08-121">Authorization</span></span>|<span data-ttu-id="92d08-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92d08-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92d08-123">Accept</span><span class="sxs-lookup"><span data-stu-id="92d08-123">Accept</span></span>|<span data-ttu-id="92d08-124">application/json</span><span class="sxs-lookup"><span data-stu-id="92d08-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92d08-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92d08-125">Request body</span></span>
<span data-ttu-id="92d08-126">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92d08-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="92d08-127">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92d08-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="92d08-128">属性</span><span class="sxs-lookup"><span data-stu-id="92d08-128">Property</span></span>|<span data-ttu-id="92d08-129">类型</span><span class="sxs-lookup"><span data-stu-id="92d08-129">Type</span></span>|<span data-ttu-id="92d08-130">说明</span><span class="sxs-lookup"><span data-stu-id="92d08-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92d08-131">id</span><span class="sxs-lookup"><span data-stu-id="92d08-131">id</span></span>|<span data-ttu-id="92d08-132">字符串</span><span class="sxs-lookup"><span data-stu-id="92d08-132">String</span></span>|<span data-ttu-id="92d08-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="92d08-133">The GUID for the object</span></span>|
|<span data-ttu-id="92d08-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="92d08-134">orderIdentifier</span></span>|<span data-ttu-id="92d08-135">字符串</span><span class="sxs-lookup"><span data-stu-id="92d08-135">String</span></span>|<span data-ttu-id="92d08-136">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="92d08-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="92d08-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="92d08-137">serialNumber</span></span>|<span data-ttu-id="92d08-138">字符串</span><span class="sxs-lookup"><span data-stu-id="92d08-138">String</span></span>|<span data-ttu-id="92d08-139">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="92d08-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="92d08-140">productKey</span><span class="sxs-lookup"><span data-stu-id="92d08-140">productKey</span></span>|<span data-ttu-id="92d08-141">字符串</span><span class="sxs-lookup"><span data-stu-id="92d08-141">String</span></span>|<span data-ttu-id="92d08-142">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="92d08-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="92d08-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="92d08-143">hardwareIdentifier</span></span>|<span data-ttu-id="92d08-144">Binary</span><span class="sxs-lookup"><span data-stu-id="92d08-144">Binary</span></span>|<span data-ttu-id="92d08-145">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="92d08-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="92d08-146">状态</span><span class="sxs-lookup"><span data-stu-id="92d08-146">state</span></span>|[<span data-ttu-id="92d08-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="92d08-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="92d08-148">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="92d08-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="92d08-149">响应</span><span class="sxs-lookup"><span data-stu-id="92d08-149">Response</span></span>
<span data-ttu-id="92d08-150">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92d08-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d08-151">示例</span><span class="sxs-lookup"><span data-stu-id="92d08-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="92d08-152">请求</span><span class="sxs-lookup"><span data-stu-id="92d08-152">Request</span></span>
<span data-ttu-id="92d08-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92d08-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92d08-154">响应</span><span class="sxs-lookup"><span data-stu-id="92d08-154">Response</span></span>
<span data-ttu-id="92d08-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92d08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



