---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新的 importedWindowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0478e84f3bf0679588fbc9f962b3471dec90f1d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753026"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="a3c87-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a3c87-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="a3c87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3c87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3c87-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3c87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3c87-106">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3c87-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3c87-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3c87-107">Prerequisites</span></span>
<span data-ttu-id="a3c87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3c87-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3c87-110">Permission type</span></span>|<span data-ttu-id="a3c87-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3c87-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3c87-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3c87-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3c87-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c87-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a3c87-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3c87-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3c87-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3c87-115">Not supported.</span></span>|
|<span data-ttu-id="a3c87-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3c87-116">Application</span></span>|<span data-ttu-id="a3c87-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c87-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3c87-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3c87-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a3c87-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3c87-119">Request headers</span></span>
|<span data-ttu-id="a3c87-120">标头</span><span class="sxs-lookup"><span data-stu-id="a3c87-120">Header</span></span>|<span data-ttu-id="a3c87-121">值</span><span class="sxs-lookup"><span data-stu-id="a3c87-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3c87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3c87-122">Authorization</span></span>|<span data-ttu-id="a3c87-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3c87-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3c87-124">接受</span><span class="sxs-lookup"><span data-stu-id="a3c87-124">Accept</span></span>|<span data-ttu-id="a3c87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3c87-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3c87-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3c87-126">Request body</span></span>
<span data-ttu-id="a3c87-127">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3c87-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="a3c87-128">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a3c87-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="a3c87-129">属性</span><span class="sxs-lookup"><span data-stu-id="a3c87-129">Property</span></span>|<span data-ttu-id="a3c87-130">类型</span><span class="sxs-lookup"><span data-stu-id="a3c87-130">Type</span></span>|<span data-ttu-id="a3c87-131">说明</span><span class="sxs-lookup"><span data-stu-id="a3c87-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3c87-132">id</span><span class="sxs-lookup"><span data-stu-id="a3c87-132">id</span></span>|<span data-ttu-id="a3c87-133">String</span><span class="sxs-lookup"><span data-stu-id="a3c87-133">String</span></span>|<span data-ttu-id="a3c87-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="a3c87-134">The GUID for the object</span></span>|
|<span data-ttu-id="a3c87-135">groupTag</span><span class="sxs-lookup"><span data-stu-id="a3c87-135">groupTag</span></span>|<span data-ttu-id="a3c87-136">String</span><span class="sxs-lookup"><span data-stu-id="a3c87-136">String</span></span>|<span data-ttu-id="a3c87-137">autopilot Windows的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="a3c87-137">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a3c87-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a3c87-138">serialNumber</span></span>|<span data-ttu-id="a3c87-139">String</span><span class="sxs-lookup"><span data-stu-id="a3c87-139">String</span></span>|<span data-ttu-id="a3c87-140">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="a3c87-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a3c87-141">productKey</span><span class="sxs-lookup"><span data-stu-id="a3c87-141">productKey</span></span>|<span data-ttu-id="a3c87-142">String</span><span class="sxs-lookup"><span data-stu-id="a3c87-142">String</span></span>|<span data-ttu-id="a3c87-143">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="a3c87-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a3c87-144">importId</span><span class="sxs-lookup"><span data-stu-id="a3c87-144">importId</span></span>|<span data-ttu-id="a3c87-145">String</span><span class="sxs-lookup"><span data-stu-id="a3c87-145">String</span></span>|<span data-ttu-id="a3c87-146">autopilot 设备的Windows ID。</span><span class="sxs-lookup"><span data-stu-id="a3c87-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a3c87-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="a3c87-147">hardwareIdentifier</span></span>|<span data-ttu-id="a3c87-148">Binary</span><span class="sxs-lookup"><span data-stu-id="a3c87-148">Binary</span></span>|<span data-ttu-id="a3c87-149">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="a3c87-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a3c87-150">state</span><span class="sxs-lookup"><span data-stu-id="a3c87-150">state</span></span>|[<span data-ttu-id="a3c87-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="a3c87-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="a3c87-152">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a3c87-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="a3c87-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3c87-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="a3c87-154">String</span><span class="sxs-lookup"><span data-stu-id="a3c87-154">String</span></span>|<span data-ttu-id="a3c87-155">将分配设备的用户的 UPN</span><span class="sxs-lookup"><span data-stu-id="a3c87-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="a3c87-156">响应</span><span class="sxs-lookup"><span data-stu-id="a3c87-156">Response</span></span>
<span data-ttu-id="a3c87-157">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3c87-157">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3c87-158">示例</span><span class="sxs-lookup"><span data-stu-id="a3c87-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3c87-159">请求</span><span class="sxs-lookup"><span data-stu-id="a3c87-159">Request</span></span>
<span data-ttu-id="a3c87-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3c87-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 631

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="a3c87-161">响应</span><span class="sxs-lookup"><span data-stu-id="a3c87-161">Response</span></span>
<span data-ttu-id="a3c87-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3c87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 680

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
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




