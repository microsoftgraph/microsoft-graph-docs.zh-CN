---
title: 创建 importedWindowsAutopilotDeviceIdentity
description: 创建新的 importedWindowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c39fed44dd8d4d7f0516f2215534ed861e13ec4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149861"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="490b3-103">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="490b3-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="490b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="490b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="490b3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="490b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="490b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="490b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="490b3-107">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="490b3-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="490b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="490b3-108">Prerequisites</span></span>
<span data-ttu-id="490b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="490b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="490b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="490b3-111">Permission type</span></span>|<span data-ttu-id="490b3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="490b3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="490b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="490b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="490b3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490b3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="490b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="490b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="490b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="490b3-116">Not supported.</span></span>|
|<span data-ttu-id="490b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="490b3-117">Application</span></span>|<span data-ttu-id="490b3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490b3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="490b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="490b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="490b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="490b3-120">Request headers</span></span>
|<span data-ttu-id="490b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="490b3-121">Header</span></span>|<span data-ttu-id="490b3-122">值</span><span class="sxs-lookup"><span data-stu-id="490b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="490b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="490b3-123">Authorization</span></span>|<span data-ttu-id="490b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="490b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="490b3-125">接受</span><span class="sxs-lookup"><span data-stu-id="490b3-125">Accept</span></span>|<span data-ttu-id="490b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="490b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="490b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="490b3-127">Request body</span></span>
<span data-ttu-id="490b3-128">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="490b3-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="490b3-129">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="490b3-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="490b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="490b3-130">Property</span></span>|<span data-ttu-id="490b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="490b3-131">Type</span></span>|<span data-ttu-id="490b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="490b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="490b3-133">id</span><span class="sxs-lookup"><span data-stu-id="490b3-133">id</span></span>|<span data-ttu-id="490b3-134">String</span><span class="sxs-lookup"><span data-stu-id="490b3-134">String</span></span>|<span data-ttu-id="490b3-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="490b3-135">The GUID for the object</span></span>|
|<span data-ttu-id="490b3-136">groupTag</span><span class="sxs-lookup"><span data-stu-id="490b3-136">groupTag</span></span>|<span data-ttu-id="490b3-137">String</span><span class="sxs-lookup"><span data-stu-id="490b3-137">String</span></span>|<span data-ttu-id="490b3-138">Windows autopilot 设备的组标记。</span><span class="sxs-lookup"><span data-stu-id="490b3-138">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="490b3-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="490b3-139">serialNumber</span></span>|<span data-ttu-id="490b3-140">String</span><span class="sxs-lookup"><span data-stu-id="490b3-140">String</span></span>|<span data-ttu-id="490b3-141">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="490b3-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="490b3-142">productKey</span><span class="sxs-lookup"><span data-stu-id="490b3-142">productKey</span></span>|<span data-ttu-id="490b3-143">String</span><span class="sxs-lookup"><span data-stu-id="490b3-143">String</span></span>|<span data-ttu-id="490b3-144">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="490b3-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="490b3-145">importId</span><span class="sxs-lookup"><span data-stu-id="490b3-145">importId</span></span>|<span data-ttu-id="490b3-146">String</span><span class="sxs-lookup"><span data-stu-id="490b3-146">String</span></span>|<span data-ttu-id="490b3-147">Windows autopilot 设备的导入 ID。</span><span class="sxs-lookup"><span data-stu-id="490b3-147">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="490b3-148">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="490b3-148">hardwareIdentifier</span></span>|<span data-ttu-id="490b3-149">Binary</span><span class="sxs-lookup"><span data-stu-id="490b3-149">Binary</span></span>|<span data-ttu-id="490b3-150">Windows autopilot 设备硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="490b3-150">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="490b3-151">state</span><span class="sxs-lookup"><span data-stu-id="490b3-151">state</span></span>|[<span data-ttu-id="490b3-152">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="490b3-152">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="490b3-153">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="490b3-153">Current state of the imported device.</span></span>|
|<span data-ttu-id="490b3-154">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="490b3-154">assignedUserPrincipalName</span></span>|<span data-ttu-id="490b3-155">String</span><span class="sxs-lookup"><span data-stu-id="490b3-155">String</span></span>|<span data-ttu-id="490b3-156">将分配设备的用户的 UPN</span><span class="sxs-lookup"><span data-stu-id="490b3-156">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="490b3-157">响应</span><span class="sxs-lookup"><span data-stu-id="490b3-157">Response</span></span>
<span data-ttu-id="490b3-158">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="490b3-158">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="490b3-159">示例</span><span class="sxs-lookup"><span data-stu-id="490b3-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="490b3-160">请求</span><span class="sxs-lookup"><span data-stu-id="490b3-160">Request</span></span>
<span data-ttu-id="490b3-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="490b3-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="490b3-162">响应</span><span class="sxs-lookup"><span data-stu-id="490b3-162">Response</span></span>
<span data-ttu-id="490b3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="490b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




