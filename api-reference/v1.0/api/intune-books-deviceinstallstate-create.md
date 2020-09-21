---
title: 创建 deviceInstallState
description: 创建新的 deviceInstallState 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4f8c2d1761ee6dd8e49caaa1fb8270d20dc1631
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966084"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="1e3dd-103">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="1e3dd-103">Create deviceInstallState</span></span>

<span data-ttu-id="1e3dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e3dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e3dd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e3dd-106">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e3dd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e3dd-107">Prerequisites</span></span>
<span data-ttu-id="1e3dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e3dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e3dd-110">Permission type</span></span>|<span data-ttu-id="1e3dd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e3dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e3dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e3dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e3dd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e3dd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e3dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e3dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e3dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-115">Not supported.</span></span>|
|<span data-ttu-id="1e3dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e3dd-116">Application</span></span>|<span data-ttu-id="1e3dd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e3dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e3dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="1e3dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e3dd-119">Request headers</span></span>
|<span data-ttu-id="1e3dd-120">标头</span><span class="sxs-lookup"><span data-stu-id="1e3dd-120">Header</span></span>|<span data-ttu-id="1e3dd-121">值</span><span class="sxs-lookup"><span data-stu-id="1e3dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e3dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e3dd-122">Authorization</span></span>|<span data-ttu-id="1e3dd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e3dd-124">接受</span><span class="sxs-lookup"><span data-stu-id="1e3dd-124">Accept</span></span>|<span data-ttu-id="1e3dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e3dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e3dd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e3dd-126">Request body</span></span>
<span data-ttu-id="1e3dd-127">在请求正文中，提供 deviceInstallState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="1e3dd-128">下表显示创建 deviceInstallState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="1e3dd-129">属性</span><span class="sxs-lookup"><span data-stu-id="1e3dd-129">Property</span></span>|<span data-ttu-id="1e3dd-130">类型</span><span class="sxs-lookup"><span data-stu-id="1e3dd-130">Type</span></span>|<span data-ttu-id="1e3dd-131">说明</span><span class="sxs-lookup"><span data-stu-id="1e3dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e3dd-132">id</span><span class="sxs-lookup"><span data-stu-id="1e3dd-132">id</span></span>|<span data-ttu-id="1e3dd-133">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-133">String</span></span>|<span data-ttu-id="1e3dd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-134">Key of the entity.</span></span>|
|<span data-ttu-id="1e3dd-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="1e3dd-135">deviceName</span></span>|<span data-ttu-id="1e3dd-136">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-136">String</span></span>|<span data-ttu-id="1e3dd-137">设备名称。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-137">Device name.</span></span>|
|<span data-ttu-id="1e3dd-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="1e3dd-138">deviceId</span></span>|<span data-ttu-id="1e3dd-139">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-139">String</span></span>|<span data-ttu-id="1e3dd-140">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-140">Device Id.</span></span>|
|<span data-ttu-id="1e3dd-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1e3dd-141">lastSyncDateTime</span></span>|<span data-ttu-id="1e3dd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e3dd-142">DateTimeOffset</span></span>|<span data-ttu-id="1e3dd-143">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-143">Last sync date and time.</span></span>|
|<span data-ttu-id="1e3dd-144">installState</span><span class="sxs-lookup"><span data-stu-id="1e3dd-144">installState</span></span>|[<span data-ttu-id="1e3dd-145">installState</span><span class="sxs-lookup"><span data-stu-id="1e3dd-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="1e3dd-146">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-146">The install state of the eBook.</span></span> <span data-ttu-id="1e3dd-147">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="1e3dd-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="1e3dd-148">errorCode</span></span>|<span data-ttu-id="1e3dd-149">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-149">String</span></span>|<span data-ttu-id="1e3dd-150">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-150">The error code for install failures.</span></span>|
|<span data-ttu-id="1e3dd-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="1e3dd-151">osVersion</span></span>|<span data-ttu-id="1e3dd-152">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-152">String</span></span>|<span data-ttu-id="1e3dd-153">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-153">OS Version.</span></span>|
|<span data-ttu-id="1e3dd-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="1e3dd-154">osDescription</span></span>|<span data-ttu-id="1e3dd-155">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-155">String</span></span>|<span data-ttu-id="1e3dd-156">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-156">OS Description.</span></span>|
|<span data-ttu-id="1e3dd-157">userName</span><span class="sxs-lookup"><span data-stu-id="1e3dd-157">userName</span></span>|<span data-ttu-id="1e3dd-158">String</span><span class="sxs-lookup"><span data-stu-id="1e3dd-158">String</span></span>|<span data-ttu-id="1e3dd-159">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="1e3dd-160">响应</span><span class="sxs-lookup"><span data-stu-id="1e3dd-160">Response</span></span>
<span data-ttu-id="1e3dd-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e3dd-162">示例</span><span class="sxs-lookup"><span data-stu-id="1e3dd-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e3dd-163">请求</span><span class="sxs-lookup"><span data-stu-id="1e3dd-163">Request</span></span>
<span data-ttu-id="1e3dd-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="1e3dd-165">响应</span><span class="sxs-lookup"><span data-stu-id="1e3dd-165">Response</span></span>
<span data-ttu-id="1e3dd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e3dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```









