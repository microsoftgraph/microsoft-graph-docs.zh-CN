---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5da7df5df6966cabf5b2435057a09399c00f8152
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015864"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="9faac-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9faac-103">Update deviceInstallState</span></span>

> <span data-ttu-id="9faac-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9faac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9faac-105">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9faac-105">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9faac-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9faac-106">Prerequisites</span></span>
<span data-ttu-id="9faac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9faac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9faac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9faac-109">Permission type</span></span>|<span data-ttu-id="9faac-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9faac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9faac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9faac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9faac-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9faac-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9faac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9faac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9faac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9faac-114">Not supported.</span></span>|
|<span data-ttu-id="9faac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9faac-115">Application</span></span>|<span data-ttu-id="9faac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9faac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9faac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9faac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9faac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9faac-118">Request headers</span></span>
|<span data-ttu-id="9faac-119">标头</span><span class="sxs-lookup"><span data-stu-id="9faac-119">Header</span></span>|<span data-ttu-id="9faac-120">值</span><span class="sxs-lookup"><span data-stu-id="9faac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9faac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9faac-121">Authorization</span></span>|<span data-ttu-id="9faac-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9faac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9faac-123">接受</span><span class="sxs-lookup"><span data-stu-id="9faac-123">Accept</span></span>|<span data-ttu-id="9faac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9faac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9faac-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9faac-125">Request body</span></span>
<span data-ttu-id="9faac-126">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9faac-126">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="9faac-127">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9faac-127">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="9faac-128">属性</span><span class="sxs-lookup"><span data-stu-id="9faac-128">Property</span></span>|<span data-ttu-id="9faac-129">类型</span><span class="sxs-lookup"><span data-stu-id="9faac-129">Type</span></span>|<span data-ttu-id="9faac-130">说明</span><span class="sxs-lookup"><span data-stu-id="9faac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9faac-131">id</span><span class="sxs-lookup"><span data-stu-id="9faac-131">id</span></span>|<span data-ttu-id="9faac-132">String</span><span class="sxs-lookup"><span data-stu-id="9faac-132">String</span></span>|<span data-ttu-id="9faac-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9faac-133">Key of the entity.</span></span>|
|<span data-ttu-id="9faac-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="9faac-134">deviceName</span></span>|<span data-ttu-id="9faac-135">String</span><span class="sxs-lookup"><span data-stu-id="9faac-135">String</span></span>|<span data-ttu-id="9faac-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="9faac-136">Device name.</span></span>|
|<span data-ttu-id="9faac-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="9faac-137">deviceId</span></span>|<span data-ttu-id="9faac-138">String</span><span class="sxs-lookup"><span data-stu-id="9faac-138">String</span></span>|<span data-ttu-id="9faac-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="9faac-139">Device Id.</span></span>|
|<span data-ttu-id="9faac-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9faac-140">lastSyncDateTime</span></span>|<span data-ttu-id="9faac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9faac-141">DateTimeOffset</span></span>|<span data-ttu-id="9faac-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9faac-142">Last sync date and time.</span></span>|
|<span data-ttu-id="9faac-143">installState</span><span class="sxs-lookup"><span data-stu-id="9faac-143">installState</span></span>|[<span data-ttu-id="9faac-144">installState</span><span class="sxs-lookup"><span data-stu-id="9faac-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="9faac-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9faac-145">The install state of the eBook.</span></span> <span data-ttu-id="9faac-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9faac-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="9faac-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="9faac-147">errorCode</span></span>|<span data-ttu-id="9faac-148">String</span><span class="sxs-lookup"><span data-stu-id="9faac-148">String</span></span>|<span data-ttu-id="9faac-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9faac-149">The error code for install failures.</span></span>|
|<span data-ttu-id="9faac-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="9faac-150">osVersion</span></span>|<span data-ttu-id="9faac-151">String</span><span class="sxs-lookup"><span data-stu-id="9faac-151">String</span></span>|<span data-ttu-id="9faac-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9faac-152">OS Version.</span></span>|
|<span data-ttu-id="9faac-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="9faac-153">osDescription</span></span>|<span data-ttu-id="9faac-154">String</span><span class="sxs-lookup"><span data-stu-id="9faac-154">String</span></span>|<span data-ttu-id="9faac-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="9faac-155">OS Description.</span></span>|
|<span data-ttu-id="9faac-156">userName</span><span class="sxs-lookup"><span data-stu-id="9faac-156">userName</span></span>|<span data-ttu-id="9faac-157">String</span><span class="sxs-lookup"><span data-stu-id="9faac-157">String</span></span>|<span data-ttu-id="9faac-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="9faac-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="9faac-159">响应</span><span class="sxs-lookup"><span data-stu-id="9faac-159">Response</span></span>
<span data-ttu-id="9faac-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9faac-160">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9faac-161">示例</span><span class="sxs-lookup"><span data-stu-id="9faac-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="9faac-162">请求</span><span class="sxs-lookup"><span data-stu-id="9faac-162">Request</span></span>
<span data-ttu-id="9faac-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9faac-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
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

### <a name="response"></a><span data-ttu-id="9faac-164">响应</span><span class="sxs-lookup"><span data-stu-id="9faac-164">Response</span></span>
<span data-ttu-id="9faac-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9faac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



