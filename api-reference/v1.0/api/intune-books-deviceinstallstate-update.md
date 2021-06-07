---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37acda13b5f55518f065fac79810a01cc1548655
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758713"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="6eb53-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6eb53-103">Update deviceInstallState</span></span>

<span data-ttu-id="6eb53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eb53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6eb53-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6eb53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eb53-106">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6eb53-106">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6eb53-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6eb53-107">Prerequisites</span></span>
<span data-ttu-id="6eb53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6eb53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb53-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eb53-110">Permission type</span></span>|<span data-ttu-id="6eb53-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6eb53-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eb53-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6eb53-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eb53-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6eb53-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eb53-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb53-115">Not supported.</span></span>|
|<span data-ttu-id="6eb53-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6eb53-116">Application</span></span>|<span data-ttu-id="6eb53-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eb53-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eb53-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eb53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6eb53-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eb53-119">Request headers</span></span>
|<span data-ttu-id="6eb53-120">标头</span><span class="sxs-lookup"><span data-stu-id="6eb53-120">Header</span></span>|<span data-ttu-id="6eb53-121">值</span><span class="sxs-lookup"><span data-stu-id="6eb53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eb53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eb53-122">Authorization</span></span>|<span data-ttu-id="6eb53-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6eb53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eb53-124">接受</span><span class="sxs-lookup"><span data-stu-id="6eb53-124">Accept</span></span>|<span data-ttu-id="6eb53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eb53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6eb53-126">Request body</span></span>
<span data-ttu-id="6eb53-127">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6eb53-127">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="6eb53-128">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6eb53-128">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="6eb53-129">属性</span><span class="sxs-lookup"><span data-stu-id="6eb53-129">Property</span></span>|<span data-ttu-id="6eb53-130">类型</span><span class="sxs-lookup"><span data-stu-id="6eb53-130">Type</span></span>|<span data-ttu-id="6eb53-131">说明</span><span class="sxs-lookup"><span data-stu-id="6eb53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eb53-132">id</span><span class="sxs-lookup"><span data-stu-id="6eb53-132">id</span></span>|<span data-ttu-id="6eb53-133">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-133">String</span></span>|<span data-ttu-id="6eb53-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6eb53-134">Key of the entity.</span></span>|
|<span data-ttu-id="6eb53-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="6eb53-135">deviceName</span></span>|<span data-ttu-id="6eb53-136">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-136">String</span></span>|<span data-ttu-id="6eb53-137">设备名称。</span><span class="sxs-lookup"><span data-stu-id="6eb53-137">Device name.</span></span>|
|<span data-ttu-id="6eb53-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="6eb53-138">deviceId</span></span>|<span data-ttu-id="6eb53-139">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-139">String</span></span>|<span data-ttu-id="6eb53-140">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="6eb53-140">Device Id.</span></span>|
|<span data-ttu-id="6eb53-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6eb53-141">lastSyncDateTime</span></span>|<span data-ttu-id="6eb53-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eb53-142">DateTimeOffset</span></span>|<span data-ttu-id="6eb53-143">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6eb53-143">Last sync date and time.</span></span>|
|<span data-ttu-id="6eb53-144">installState</span><span class="sxs-lookup"><span data-stu-id="6eb53-144">installState</span></span>|[<span data-ttu-id="6eb53-145">installState</span><span class="sxs-lookup"><span data-stu-id="6eb53-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="6eb53-146">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="6eb53-146">The install state of the eBook.</span></span> <span data-ttu-id="6eb53-147">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="6eb53-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="6eb53-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="6eb53-148">errorCode</span></span>|<span data-ttu-id="6eb53-149">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-149">String</span></span>|<span data-ttu-id="6eb53-150">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="6eb53-150">The error code for install failures.</span></span>|
|<span data-ttu-id="6eb53-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="6eb53-151">osVersion</span></span>|<span data-ttu-id="6eb53-152">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-152">String</span></span>|<span data-ttu-id="6eb53-153">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6eb53-153">OS Version.</span></span>|
|<span data-ttu-id="6eb53-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="6eb53-154">osDescription</span></span>|<span data-ttu-id="6eb53-155">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-155">String</span></span>|<span data-ttu-id="6eb53-156">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="6eb53-156">OS Description.</span></span>|
|<span data-ttu-id="6eb53-157">userName</span><span class="sxs-lookup"><span data-stu-id="6eb53-157">userName</span></span>|<span data-ttu-id="6eb53-158">String</span><span class="sxs-lookup"><span data-stu-id="6eb53-158">String</span></span>|<span data-ttu-id="6eb53-159">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="6eb53-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="6eb53-160">响应</span><span class="sxs-lookup"><span data-stu-id="6eb53-160">Response</span></span>
<span data-ttu-id="6eb53-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6eb53-161">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eb53-162">示例</span><span class="sxs-lookup"><span data-stu-id="6eb53-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6eb53-163">请求</span><span class="sxs-lookup"><span data-stu-id="6eb53-163">Request</span></span>
<span data-ttu-id="6eb53-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6eb53-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6eb53-165">响应</span><span class="sxs-lookup"><span data-stu-id="6eb53-165">Response</span></span>
<span data-ttu-id="6eb53-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6eb53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




