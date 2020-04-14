---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新的 importedWindowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef21ddb7f3d392bd833f7396a8c29b9cd92dbe1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452593"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="4fb2d-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="4fb2d-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="4fb2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fb2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fb2d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fb2d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fb2d-107">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fb2d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4fb2d-108">Prerequisites</span></span>
<span data-ttu-id="4fb2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fb2d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fb2d-111">Permission type</span></span>|<span data-ttu-id="4fb2d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4fb2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fb2d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fb2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fb2d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb2d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4fb2d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fb2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fb2d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-116">Not supported.</span></span>|
|<span data-ttu-id="4fb2d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fb2d-117">Application</span></span>|<span data-ttu-id="4fb2d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb2d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fb2d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fb2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="4fb2d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fb2d-120">Request headers</span></span>
|<span data-ttu-id="4fb2d-121">标头</span><span class="sxs-lookup"><span data-stu-id="4fb2d-121">Header</span></span>|<span data-ttu-id="4fb2d-122">值</span><span class="sxs-lookup"><span data-stu-id="4fb2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fb2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fb2d-123">Authorization</span></span>|<span data-ttu-id="4fb2d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fb2d-125">接受</span><span class="sxs-lookup"><span data-stu-id="4fb2d-125">Accept</span></span>|<span data-ttu-id="4fb2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fb2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fb2d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fb2d-127">Request body</span></span>
<span data-ttu-id="4fb2d-128">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="4fb2d-129">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="4fb2d-130">属性</span><span class="sxs-lookup"><span data-stu-id="4fb2d-130">Property</span></span>|<span data-ttu-id="4fb2d-131">类型</span><span class="sxs-lookup"><span data-stu-id="4fb2d-131">Type</span></span>|<span data-ttu-id="4fb2d-132">说明</span><span class="sxs-lookup"><span data-stu-id="4fb2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb2d-133">id</span><span class="sxs-lookup"><span data-stu-id="4fb2d-133">id</span></span>|<span data-ttu-id="4fb2d-134">String</span><span class="sxs-lookup"><span data-stu-id="4fb2d-134">String</span></span>|<span data-ttu-id="4fb2d-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="4fb2d-135">The GUID for the object</span></span>|
|<span data-ttu-id="4fb2d-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="4fb2d-136">orderIdentifier</span></span>|<span data-ttu-id="4fb2d-137">String</span><span class="sxs-lookup"><span data-stu-id="4fb2d-137">String</span></span>|<span data-ttu-id="4fb2d-138">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-138">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="4fb2d-139">-弃用</span><span class="sxs-lookup"><span data-stu-id="4fb2d-139">- Deprecate</span></span>|
|<span data-ttu-id="4fb2d-140">groupTag</span><span class="sxs-lookup"><span data-stu-id="4fb2d-140">groupTag</span></span>|<span data-ttu-id="4fb2d-141">String</span><span class="sxs-lookup"><span data-stu-id="4fb2d-141">String</span></span>|<span data-ttu-id="4fb2d-142">Windows autopilot 设备的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-142">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4fb2d-143">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4fb2d-143">serialNumber</span></span>|<span data-ttu-id="4fb2d-144">String</span><span class="sxs-lookup"><span data-stu-id="4fb2d-144">String</span></span>|<span data-ttu-id="4fb2d-145">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-145">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4fb2d-146">productKey</span><span class="sxs-lookup"><span data-stu-id="4fb2d-146">productKey</span></span>|<span data-ttu-id="4fb2d-147">字符串</span><span class="sxs-lookup"><span data-stu-id="4fb2d-147">String</span></span>|<span data-ttu-id="4fb2d-148">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-148">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4fb2d-149">importId</span><span class="sxs-lookup"><span data-stu-id="4fb2d-149">importId</span></span>|<span data-ttu-id="4fb2d-150">String</span><span class="sxs-lookup"><span data-stu-id="4fb2d-150">String</span></span>|<span data-ttu-id="4fb2d-151">Windows autopilot 设备的导入 Id。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-151">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4fb2d-152">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="4fb2d-152">hardwareIdentifier</span></span>|<span data-ttu-id="4fb2d-153">Binary</span><span class="sxs-lookup"><span data-stu-id="4fb2d-153">Binary</span></span>|<span data-ttu-id="4fb2d-154">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-154">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="4fb2d-155">state</span><span class="sxs-lookup"><span data-stu-id="4fb2d-155">state</span></span>|[<span data-ttu-id="4fb2d-156">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="4fb2d-156">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="4fb2d-157">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-157">Current state of the imported device.</span></span>|
|<span data-ttu-id="4fb2d-158">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fb2d-158">assignedUserPrincipalName</span></span>|<span data-ttu-id="4fb2d-159">String</span><span class="sxs-lookup"><span data-stu-id="4fb2d-159">String</span></span>|<span data-ttu-id="4fb2d-160">将为设备分配的用户的 UPN</span><span class="sxs-lookup"><span data-stu-id="4fb2d-160">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="4fb2d-161">响应</span><span class="sxs-lookup"><span data-stu-id="4fb2d-161">Response</span></span>
<span data-ttu-id="4fb2d-162">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-162">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fb2d-163">示例</span><span class="sxs-lookup"><span data-stu-id="4fb2d-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fb2d-164">请求</span><span class="sxs-lookup"><span data-stu-id="4fb2d-164">Request</span></span>
<span data-ttu-id="4fb2d-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="4fb2d-166">响应</span><span class="sxs-lookup"><span data-stu-id="4fb2d-166">Response</span></span>
<span data-ttu-id="4fb2d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4fb2d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



