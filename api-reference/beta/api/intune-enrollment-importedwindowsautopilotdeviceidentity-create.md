---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新的 importedWindowsAutopilotDeviceIdentity 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dcd78ce37bdc4718bb69ed324ab34c12d2c7096
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908418"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="9905b-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="9905b-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="9905b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9905b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9905b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9905b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9905b-106">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9905b-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9905b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9905b-107">Prerequisites</span></span>
<span data-ttu-id="9905b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9905b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9905b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9905b-110">Permission type</span></span>|<span data-ttu-id="9905b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9905b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9905b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9905b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9905b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9905b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9905b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9905b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9905b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9905b-115">Not supported.</span></span>|
|<span data-ttu-id="9905b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9905b-116">Application</span></span>|<span data-ttu-id="9905b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9905b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9905b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9905b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="9905b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9905b-119">Request headers</span></span>
|<span data-ttu-id="9905b-120">标头</span><span class="sxs-lookup"><span data-stu-id="9905b-120">Header</span></span>|<span data-ttu-id="9905b-121">值</span><span class="sxs-lookup"><span data-stu-id="9905b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9905b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9905b-122">Authorization</span></span>|<span data-ttu-id="9905b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9905b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9905b-124">接受</span><span class="sxs-lookup"><span data-stu-id="9905b-124">Accept</span></span>|<span data-ttu-id="9905b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9905b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9905b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9905b-126">Request body</span></span>
<span data-ttu-id="9905b-127">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9905b-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="9905b-128">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9905b-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="9905b-129">属性</span><span class="sxs-lookup"><span data-stu-id="9905b-129">Property</span></span>|<span data-ttu-id="9905b-130">类型</span><span class="sxs-lookup"><span data-stu-id="9905b-130">Type</span></span>|<span data-ttu-id="9905b-131">说明</span><span class="sxs-lookup"><span data-stu-id="9905b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9905b-132">id</span><span class="sxs-lookup"><span data-stu-id="9905b-132">id</span></span>|<span data-ttu-id="9905b-133">String</span><span class="sxs-lookup"><span data-stu-id="9905b-133">String</span></span>|<span data-ttu-id="9905b-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="9905b-134">The GUID for the object</span></span>|
|<span data-ttu-id="9905b-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="9905b-135">orderIdentifier</span></span>|<span data-ttu-id="9905b-136">String</span><span class="sxs-lookup"><span data-stu-id="9905b-136">String</span></span>|<span data-ttu-id="9905b-137">Windows autopilot 设备订单 Id。</span><span class="sxs-lookup"><span data-stu-id="9905b-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9905b-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9905b-138">serialNumber</span></span>|<span data-ttu-id="9905b-139">String</span><span class="sxs-lookup"><span data-stu-id="9905b-139">String</span></span>|<span data-ttu-id="9905b-140">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="9905b-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9905b-141">productKey</span><span class="sxs-lookup"><span data-stu-id="9905b-141">productKey</span></span>|<span data-ttu-id="9905b-142">字符串</span><span class="sxs-lookup"><span data-stu-id="9905b-142">String</span></span>|<span data-ttu-id="9905b-143">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="9905b-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9905b-144">importId</span><span class="sxs-lookup"><span data-stu-id="9905b-144">importId</span></span>|<span data-ttu-id="9905b-145">String</span><span class="sxs-lookup"><span data-stu-id="9905b-145">String</span></span>|<span data-ttu-id="9905b-146">Windows autopilot 设备的导入 Id。</span><span class="sxs-lookup"><span data-stu-id="9905b-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9905b-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="9905b-147">hardwareIdentifier</span></span>|<span data-ttu-id="9905b-148">Binary</span><span class="sxs-lookup"><span data-stu-id="9905b-148">Binary</span></span>|<span data-ttu-id="9905b-149">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="9905b-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="9905b-150">state</span><span class="sxs-lookup"><span data-stu-id="9905b-150">state</span></span>|[<span data-ttu-id="9905b-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="9905b-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="9905b-152">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="9905b-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="9905b-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9905b-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="9905b-154">String</span><span class="sxs-lookup"><span data-stu-id="9905b-154">String</span></span>|<span data-ttu-id="9905b-155">将为设备分配的用户的 UPN</span><span class="sxs-lookup"><span data-stu-id="9905b-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="9905b-156">响应</span><span class="sxs-lookup"><span data-stu-id="9905b-156">Response</span></span>
<span data-ttu-id="9905b-157">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9905b-157">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9905b-158">示例</span><span class="sxs-lookup"><span data-stu-id="9905b-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="9905b-159">请求</span><span class="sxs-lookup"><span data-stu-id="9905b-159">Request</span></span>
<span data-ttu-id="9905b-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9905b-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 645

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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="9905b-161">响应</span><span class="sxs-lookup"><span data-stu-id="9905b-161">Response</span></span>
<span data-ttu-id="9905b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9905b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 694

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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```




