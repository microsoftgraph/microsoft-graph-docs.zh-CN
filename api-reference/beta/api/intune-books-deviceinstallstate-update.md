---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c74be38f35071a0bf2d619a88fe1cd47802c917d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48716878"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="6e225-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="6e225-103">Update deviceInstallState</span></span>

<span data-ttu-id="6e225-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e225-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e225-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e225-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e225-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e225-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e225-107">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e225-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e225-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e225-108">Prerequisites</span></span>
<span data-ttu-id="6e225-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e225-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e225-111">Permission type</span></span>|<span data-ttu-id="6e225-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e225-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e225-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e225-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e225-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e225-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6e225-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e225-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e225-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e225-116">Not supported.</span></span>|
|<span data-ttu-id="6e225-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e225-117">Application</span></span>|<span data-ttu-id="6e225-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e225-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e225-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e225-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6e225-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e225-120">Request headers</span></span>
|<span data-ttu-id="6e225-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e225-121">Header</span></span>|<span data-ttu-id="6e225-122">值</span><span class="sxs-lookup"><span data-stu-id="6e225-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e225-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e225-123">Authorization</span></span>|<span data-ttu-id="6e225-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e225-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e225-125">接受</span><span class="sxs-lookup"><span data-stu-id="6e225-125">Accept</span></span>|<span data-ttu-id="6e225-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e225-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e225-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e225-127">Request body</span></span>
<span data-ttu-id="6e225-128">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e225-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="6e225-129">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e225-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="6e225-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e225-130">Property</span></span>|<span data-ttu-id="6e225-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e225-131">Type</span></span>|<span data-ttu-id="6e225-132">说明</span><span class="sxs-lookup"><span data-stu-id="6e225-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e225-133">id</span><span class="sxs-lookup"><span data-stu-id="6e225-133">id</span></span>|<span data-ttu-id="6e225-134">String</span><span class="sxs-lookup"><span data-stu-id="6e225-134">String</span></span>|<span data-ttu-id="6e225-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6e225-135">Key of the entity.</span></span>|
|<span data-ttu-id="6e225-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="6e225-136">deviceName</span></span>|<span data-ttu-id="6e225-137">String</span><span class="sxs-lookup"><span data-stu-id="6e225-137">String</span></span>|<span data-ttu-id="6e225-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="6e225-138">Device name.</span></span>|
|<span data-ttu-id="6e225-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="6e225-139">deviceId</span></span>|<span data-ttu-id="6e225-140">String</span><span class="sxs-lookup"><span data-stu-id="6e225-140">String</span></span>|<span data-ttu-id="6e225-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="6e225-141">Device Id.</span></span>|
|<span data-ttu-id="6e225-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6e225-142">lastSyncDateTime</span></span>|<span data-ttu-id="6e225-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e225-143">DateTimeOffset</span></span>|<span data-ttu-id="6e225-144">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6e225-144">Last sync date and time.</span></span>|
|<span data-ttu-id="6e225-145">installState</span><span class="sxs-lookup"><span data-stu-id="6e225-145">installState</span></span>|[<span data-ttu-id="6e225-146">installState</span><span class="sxs-lookup"><span data-stu-id="6e225-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="6e225-147">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="6e225-147">The install state of the eBook.</span></span> <span data-ttu-id="6e225-148">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="6e225-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="6e225-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="6e225-149">errorCode</span></span>|<span data-ttu-id="6e225-150">String</span><span class="sxs-lookup"><span data-stu-id="6e225-150">String</span></span>|<span data-ttu-id="6e225-151">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="6e225-151">The error code for install failures.</span></span>|
|<span data-ttu-id="6e225-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="6e225-152">osVersion</span></span>|<span data-ttu-id="6e225-153">String</span><span class="sxs-lookup"><span data-stu-id="6e225-153">String</span></span>|<span data-ttu-id="6e225-154">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6e225-154">OS Version.</span></span>|
|<span data-ttu-id="6e225-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="6e225-155">osDescription</span></span>|<span data-ttu-id="6e225-156">String</span><span class="sxs-lookup"><span data-stu-id="6e225-156">String</span></span>|<span data-ttu-id="6e225-157">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="6e225-157">OS Description.</span></span>|
|<span data-ttu-id="6e225-158">userName</span><span class="sxs-lookup"><span data-stu-id="6e225-158">userName</span></span>|<span data-ttu-id="6e225-159">String</span><span class="sxs-lookup"><span data-stu-id="6e225-159">String</span></span>|<span data-ttu-id="6e225-160">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="6e225-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="6e225-161">响应</span><span class="sxs-lookup"><span data-stu-id="6e225-161">Response</span></span>
<span data-ttu-id="6e225-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e225-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e225-163">示例</span><span class="sxs-lookup"><span data-stu-id="6e225-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e225-164">请求</span><span class="sxs-lookup"><span data-stu-id="6e225-164">Request</span></span>
<span data-ttu-id="6e225-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e225-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
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

### <a name="response"></a><span data-ttu-id="6e225-166">响应</span><span class="sxs-lookup"><span data-stu-id="6e225-166">Response</span></span>
<span data-ttu-id="6e225-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e225-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





