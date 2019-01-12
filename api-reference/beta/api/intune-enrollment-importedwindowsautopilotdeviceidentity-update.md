---
title: Update importedWindowsAutopilotDeviceIdentity
description: 更新 importedWindowsAutopilotDeviceIdentity 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e2f5385729233d975b35fb7bd78e51931bdab34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959466"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="7273c-103">Update importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="7273c-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="7273c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7273c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7273c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7273c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7273c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7273c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7273c-107">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7273c-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7273c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7273c-108">Prerequisites</span></span>
<span data-ttu-id="7273c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7273c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7273c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7273c-111">Permission type</span></span>|<span data-ttu-id="7273c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7273c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7273c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7273c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7273c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7273c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7273c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7273c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7273c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7273c-116">Not supported.</span></span>|
|<span data-ttu-id="7273c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7273c-117">Application</span></span>|<span data-ttu-id="7273c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7273c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7273c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7273c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="7273c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7273c-120">Request headers</span></span>
|<span data-ttu-id="7273c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7273c-121">Header</span></span>|<span data-ttu-id="7273c-122">值</span><span class="sxs-lookup"><span data-stu-id="7273c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7273c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7273c-123">Authorization</span></span>|<span data-ttu-id="7273c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7273c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7273c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7273c-125">Accept</span></span>|<span data-ttu-id="7273c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7273c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7273c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7273c-127">Request body</span></span>
<span data-ttu-id="7273c-128">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7273c-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="7273c-129">下表显示创建 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7273c-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="7273c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7273c-130">Property</span></span>|<span data-ttu-id="7273c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7273c-131">Type</span></span>|<span data-ttu-id="7273c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7273c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7273c-133">id</span><span class="sxs-lookup"><span data-stu-id="7273c-133">id</span></span>|<span data-ttu-id="7273c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7273c-134">String</span></span>|<span data-ttu-id="7273c-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="7273c-135">The GUID for the object</span></span>|
|<span data-ttu-id="7273c-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="7273c-136">orderIdentifier</span></span>|<span data-ttu-id="7273c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7273c-137">String</span></span>|<span data-ttu-id="7273c-138">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="7273c-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7273c-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7273c-139">serialNumber</span></span>|<span data-ttu-id="7273c-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7273c-140">String</span></span>|<span data-ttu-id="7273c-141">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="7273c-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7273c-142">productKey</span><span class="sxs-lookup"><span data-stu-id="7273c-142">productKey</span></span>|<span data-ttu-id="7273c-143">字符串</span><span class="sxs-lookup"><span data-stu-id="7273c-143">String</span></span>|<span data-ttu-id="7273c-144">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="7273c-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7273c-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="7273c-145">hardwareIdentifier</span></span>|<span data-ttu-id="7273c-146">Binary</span><span class="sxs-lookup"><span data-stu-id="7273c-146">Binary</span></span>|<span data-ttu-id="7273c-147">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="7273c-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7273c-148">状态</span><span class="sxs-lookup"><span data-stu-id="7273c-148">state</span></span>|[<span data-ttu-id="7273c-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="7273c-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="7273c-150">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="7273c-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="7273c-151">响应</span><span class="sxs-lookup"><span data-stu-id="7273c-151">Response</span></span>
<span data-ttu-id="7273c-152">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7273c-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7273c-153">示例</span><span class="sxs-lookup"><span data-stu-id="7273c-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="7273c-154">请求</span><span class="sxs-lookup"><span data-stu-id="7273c-154">Request</span></span>
<span data-ttu-id="7273c-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7273c-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 464

{
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

### <a name="response"></a><span data-ttu-id="7273c-156">响应</span><span class="sxs-lookup"><span data-stu-id="7273c-156">Response</span></span>
<span data-ttu-id="7273c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7273c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





