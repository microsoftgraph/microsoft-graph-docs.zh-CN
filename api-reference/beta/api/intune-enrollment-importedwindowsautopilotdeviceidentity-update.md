---
title: Update importedWindowsAutopilotDeviceIdentity
description: 更新 importedWindowsAutopilotDeviceIdentity 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45665498ceb3b1ec52fa7f56bb3e4abd6013cae5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729990"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="a1887-103">Update importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a1887-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="a1887-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1887-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1887-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1887-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1887-106">更新 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1887-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1887-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1887-107">Prerequisites</span></span>
<span data-ttu-id="a1887-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1887-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1887-110">Permission type</span></span>|<span data-ttu-id="a1887-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1887-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1887-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1887-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1887-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1887-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1887-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1887-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1887-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1887-115">Not supported.</span></span>|
|<span data-ttu-id="a1887-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1887-116">Application</span></span>|<span data-ttu-id="a1887-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1887-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1887-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1887-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a1887-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1887-119">Request headers</span></span>
|<span data-ttu-id="a1887-120">标头</span><span class="sxs-lookup"><span data-stu-id="a1887-120">Header</span></span>|<span data-ttu-id="a1887-121">值</span><span class="sxs-lookup"><span data-stu-id="a1887-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1887-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1887-122">Authorization</span></span>|<span data-ttu-id="a1887-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1887-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1887-124">接受</span><span class="sxs-lookup"><span data-stu-id="a1887-124">Accept</span></span>|<span data-ttu-id="a1887-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1887-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1887-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1887-126">Request body</span></span>
<span data-ttu-id="a1887-127">在请求正文中，提供 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1887-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="a1887-128">下表显示创建 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1887-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="a1887-129">属性</span><span class="sxs-lookup"><span data-stu-id="a1887-129">Property</span></span>|<span data-ttu-id="a1887-130">类型</span><span class="sxs-lookup"><span data-stu-id="a1887-130">Type</span></span>|<span data-ttu-id="a1887-131">说明</span><span class="sxs-lookup"><span data-stu-id="a1887-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1887-132">id</span><span class="sxs-lookup"><span data-stu-id="a1887-132">id</span></span>|<span data-ttu-id="a1887-133">String</span><span class="sxs-lookup"><span data-stu-id="a1887-133">String</span></span>|<span data-ttu-id="a1887-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="a1887-134">The GUID for the object</span></span>|
|<span data-ttu-id="a1887-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1887-135">orderIdentifier</span></span>|<span data-ttu-id="a1887-136">String</span><span class="sxs-lookup"><span data-stu-id="a1887-136">String</span></span>|<span data-ttu-id="a1887-137">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="a1887-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="a1887-138">-弃用</span><span class="sxs-lookup"><span data-stu-id="a1887-138">- Deprecate</span></span>|
|<span data-ttu-id="a1887-139">groupTag</span><span class="sxs-lookup"><span data-stu-id="a1887-139">groupTag</span></span>|<span data-ttu-id="a1887-140">String</span><span class="sxs-lookup"><span data-stu-id="a1887-140">String</span></span>|<span data-ttu-id="a1887-141">Windows autopilot 设备的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="a1887-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1887-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a1887-142">serialNumber</span></span>|<span data-ttu-id="a1887-143">String</span><span class="sxs-lookup"><span data-stu-id="a1887-143">String</span></span>|<span data-ttu-id="a1887-144">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="a1887-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1887-145">productKey</span><span class="sxs-lookup"><span data-stu-id="a1887-145">productKey</span></span>|<span data-ttu-id="a1887-146">字符串</span><span class="sxs-lookup"><span data-stu-id="a1887-146">String</span></span>|<span data-ttu-id="a1887-147">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="a1887-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1887-148">importId</span><span class="sxs-lookup"><span data-stu-id="a1887-148">importId</span></span>|<span data-ttu-id="a1887-149">String</span><span class="sxs-lookup"><span data-stu-id="a1887-149">String</span></span>|<span data-ttu-id="a1887-150">Windows autopilot 设备的导入 Id。</span><span class="sxs-lookup"><span data-stu-id="a1887-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1887-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1887-151">hardwareIdentifier</span></span>|<span data-ttu-id="a1887-152">Binary</span><span class="sxs-lookup"><span data-stu-id="a1887-152">Binary</span></span>|<span data-ttu-id="a1887-153">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="a1887-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1887-154">state</span><span class="sxs-lookup"><span data-stu-id="a1887-154">state</span></span>|[<span data-ttu-id="a1887-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="a1887-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="a1887-156">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a1887-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="a1887-157">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a1887-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="a1887-158">String</span><span class="sxs-lookup"><span data-stu-id="a1887-158">String</span></span>|<span data-ttu-id="a1887-159">将为设备分配的用户的 UPN</span><span class="sxs-lookup"><span data-stu-id="a1887-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="a1887-160">响应</span><span class="sxs-lookup"><span data-stu-id="a1887-160">Response</span></span>
<span data-ttu-id="a1887-161">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1887-161">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1887-162">示例</span><span class="sxs-lookup"><span data-stu-id="a1887-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1887-163">请求</span><span class="sxs-lookup"><span data-stu-id="a1887-163">Request</span></span>
<span data-ttu-id="a1887-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1887-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1887-165">响应</span><span class="sxs-lookup"><span data-stu-id="a1887-165">Response</span></span>
<span data-ttu-id="a1887-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1887-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





