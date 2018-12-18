---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新importedWindowsAutopilotDeviceIdentity对象。
author: tfitzmac
ms.openlocfilehash: 9f4c6519746690290af6ec243d6b309dfeb6782d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350062"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="b6747-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b6747-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="b6747-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6747-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6747-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6747-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6747-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b6747-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6747-107">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6747-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6747-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6747-108">Prerequisites</span></span>
<span data-ttu-id="b6747-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b6747-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6747-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6747-111">Permission type</span></span>|<span data-ttu-id="b6747-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6747-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6747-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6747-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6747-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6747-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6747-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6747-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6747-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6747-116">Not supported.</span></span>|
|<span data-ttu-id="b6747-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6747-117">Application</span></span>|<span data-ttu-id="b6747-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6747-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6747-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6747-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="b6747-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6747-120">Request headers</span></span>
|<span data-ttu-id="b6747-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6747-121">Header</span></span>|<span data-ttu-id="b6747-122">值</span><span class="sxs-lookup"><span data-stu-id="b6747-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6747-123">授权</span><span class="sxs-lookup"><span data-stu-id="b6747-123">Authorization</span></span>|<span data-ttu-id="b6747-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6747-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6747-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6747-125">Accept</span></span>|<span data-ttu-id="b6747-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6747-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6747-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6747-127">Request body</span></span>
<span data-ttu-id="b6747-128">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6747-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="b6747-129">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6747-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="b6747-130">属性</span><span class="sxs-lookup"><span data-stu-id="b6747-130">Property</span></span>|<span data-ttu-id="b6747-131">类型</span><span class="sxs-lookup"><span data-stu-id="b6747-131">Type</span></span>|<span data-ttu-id="b6747-132">说明</span><span class="sxs-lookup"><span data-stu-id="b6747-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6747-133">id</span><span class="sxs-lookup"><span data-stu-id="b6747-133">id</span></span>|<span data-ttu-id="b6747-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b6747-134">String</span></span>|<span data-ttu-id="b6747-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="b6747-135">The GUID for the object</span></span>|
|<span data-ttu-id="b6747-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="b6747-136">orderIdentifier</span></span>|<span data-ttu-id="b6747-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b6747-137">String</span></span>|<span data-ttu-id="b6747-138">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="b6747-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b6747-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b6747-139">serialNumber</span></span>|<span data-ttu-id="b6747-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b6747-140">String</span></span>|<span data-ttu-id="b6747-141">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="b6747-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b6747-142">productKey</span><span class="sxs-lookup"><span data-stu-id="b6747-142">productKey</span></span>|<span data-ttu-id="b6747-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b6747-143">String</span></span>|<span data-ttu-id="b6747-144">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="b6747-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b6747-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="b6747-145">hardwareIdentifier</span></span>|<span data-ttu-id="b6747-146">Binary</span><span class="sxs-lookup"><span data-stu-id="b6747-146">Binary</span></span>|<span data-ttu-id="b6747-147">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="b6747-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b6747-148">状态</span><span class="sxs-lookup"><span data-stu-id="b6747-148">state</span></span>|[<span data-ttu-id="b6747-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="b6747-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="b6747-150">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="b6747-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="b6747-151">响应</span><span class="sxs-lookup"><span data-stu-id="b6747-151">Response</span></span>
<span data-ttu-id="b6747-152">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6747-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6747-153">示例</span><span class="sxs-lookup"><span data-stu-id="b6747-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6747-154">请求</span><span class="sxs-lookup"><span data-stu-id="b6747-154">Request</span></span>
<span data-ttu-id="b6747-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6747-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6747-156">响应</span><span class="sxs-lookup"><span data-stu-id="b6747-156">Response</span></span>
<span data-ttu-id="b6747-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6747-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





