---
title: Update importedWindowsAutopilotDeviceIdentity
description: 更新 importedWindowsAutopilotDeviceIdentity 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1170bbb7e852a8b63939137a04fd11d2d5203e4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986495"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="40bce-103">Update importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="40bce-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="40bce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40bce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40bce-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40bce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40bce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40bce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40bce-107">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="40bce-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40bce-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40bce-108">Prerequisites</span></span>
<span data-ttu-id="40bce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40bce-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40bce-111">Permission type</span></span>|<span data-ttu-id="40bce-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40bce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40bce-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40bce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40bce-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40bce-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="40bce-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40bce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40bce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40bce-116">Not supported.</span></span>|
|<span data-ttu-id="40bce-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40bce-117">Application</span></span>|<span data-ttu-id="40bce-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40bce-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40bce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40bce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="40bce-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40bce-120">Request headers</span></span>
|<span data-ttu-id="40bce-121">标头</span><span class="sxs-lookup"><span data-stu-id="40bce-121">Header</span></span>|<span data-ttu-id="40bce-122">值</span><span class="sxs-lookup"><span data-stu-id="40bce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40bce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40bce-123">Authorization</span></span>|<span data-ttu-id="40bce-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40bce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40bce-125">接受</span><span class="sxs-lookup"><span data-stu-id="40bce-125">Accept</span></span>|<span data-ttu-id="40bce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40bce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40bce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40bce-127">Request body</span></span>
<span data-ttu-id="40bce-128">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40bce-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="40bce-129">下表显示创建 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40bce-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="40bce-130">属性</span><span class="sxs-lookup"><span data-stu-id="40bce-130">Property</span></span>|<span data-ttu-id="40bce-131">类型</span><span class="sxs-lookup"><span data-stu-id="40bce-131">Type</span></span>|<span data-ttu-id="40bce-132">说明</span><span class="sxs-lookup"><span data-stu-id="40bce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40bce-133">id</span><span class="sxs-lookup"><span data-stu-id="40bce-133">id</span></span>|<span data-ttu-id="40bce-134">String</span><span class="sxs-lookup"><span data-stu-id="40bce-134">String</span></span>|<span data-ttu-id="40bce-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="40bce-135">The GUID for the object</span></span>|
|<span data-ttu-id="40bce-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="40bce-136">orderIdentifier</span></span>|<span data-ttu-id="40bce-137">String</span><span class="sxs-lookup"><span data-stu-id="40bce-137">String</span></span>|<span data-ttu-id="40bce-138">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="40bce-138">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="40bce-139">-弃用</span><span class="sxs-lookup"><span data-stu-id="40bce-139">- Deprecate</span></span>|
|<span data-ttu-id="40bce-140">groupTag</span><span class="sxs-lookup"><span data-stu-id="40bce-140">groupTag</span></span>|<span data-ttu-id="40bce-141">String</span><span class="sxs-lookup"><span data-stu-id="40bce-141">String</span></span>|<span data-ttu-id="40bce-142">Windows autopilot 设备的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="40bce-142">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="40bce-143">serialNumber</span><span class="sxs-lookup"><span data-stu-id="40bce-143">serialNumber</span></span>|<span data-ttu-id="40bce-144">String</span><span class="sxs-lookup"><span data-stu-id="40bce-144">String</span></span>|<span data-ttu-id="40bce-145">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="40bce-145">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="40bce-146">productKey</span><span class="sxs-lookup"><span data-stu-id="40bce-146">productKey</span></span>|<span data-ttu-id="40bce-147">String</span><span class="sxs-lookup"><span data-stu-id="40bce-147">String</span></span>|<span data-ttu-id="40bce-148">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="40bce-148">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="40bce-149">importId</span><span class="sxs-lookup"><span data-stu-id="40bce-149">importId</span></span>|<span data-ttu-id="40bce-150">String</span><span class="sxs-lookup"><span data-stu-id="40bce-150">String</span></span>|<span data-ttu-id="40bce-151">Windows autopilot 设备的导入 Id。</span><span class="sxs-lookup"><span data-stu-id="40bce-151">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="40bce-152">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="40bce-152">hardwareIdentifier</span></span>|<span data-ttu-id="40bce-153">Binary</span><span class="sxs-lookup"><span data-stu-id="40bce-153">Binary</span></span>|<span data-ttu-id="40bce-154">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="40bce-154">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="40bce-155">state</span><span class="sxs-lookup"><span data-stu-id="40bce-155">state</span></span>|[<span data-ttu-id="40bce-156">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="40bce-156">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="40bce-157">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="40bce-157">Current state of the imported device.</span></span>|
|<span data-ttu-id="40bce-158">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="40bce-158">assignedUserPrincipalName</span></span>|<span data-ttu-id="40bce-159">String</span><span class="sxs-lookup"><span data-stu-id="40bce-159">String</span></span>|<span data-ttu-id="40bce-160">将为设备分配的用户的 UPN</span><span class="sxs-lookup"><span data-stu-id="40bce-160">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="40bce-161">响应</span><span class="sxs-lookup"><span data-stu-id="40bce-161">Response</span></span>
<span data-ttu-id="40bce-162">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40bce-162">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40bce-163">示例</span><span class="sxs-lookup"><span data-stu-id="40bce-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="40bce-164">请求</span><span class="sxs-lookup"><span data-stu-id="40bce-164">Request</span></span>
<span data-ttu-id="40bce-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40bce-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 679

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="40bce-166">响应</span><span class="sxs-lookup"><span data-stu-id="40bce-166">Response</span></span>
<span data-ttu-id="40bce-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40bce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 728

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```






