---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 940c2e88761aefa5bc18c71b7d785c5ceb0b9647
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131888"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="80216-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="80216-103">Update deviceInstallState</span></span>

<span data-ttu-id="80216-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80216-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80216-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80216-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80216-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80216-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80216-107">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80216-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80216-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="80216-108">Prerequisites</span></span>
<span data-ttu-id="80216-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80216-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80216-111">Permission type</span></span>|<span data-ttu-id="80216-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80216-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80216-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80216-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80216-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80216-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80216-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80216-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80216-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80216-116">Not supported.</span></span>|
|<span data-ttu-id="80216-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80216-117">Application</span></span>|<span data-ttu-id="80216-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80216-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80216-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80216-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="80216-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80216-120">Request headers</span></span>
|<span data-ttu-id="80216-121">标头</span><span class="sxs-lookup"><span data-stu-id="80216-121">Header</span></span>|<span data-ttu-id="80216-122">值</span><span class="sxs-lookup"><span data-stu-id="80216-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80216-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80216-123">Authorization</span></span>|<span data-ttu-id="80216-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80216-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80216-125">接受</span><span class="sxs-lookup"><span data-stu-id="80216-125">Accept</span></span>|<span data-ttu-id="80216-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80216-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80216-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80216-127">Request body</span></span>
<span data-ttu-id="80216-128">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80216-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="80216-129">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80216-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="80216-130">属性</span><span class="sxs-lookup"><span data-stu-id="80216-130">Property</span></span>|<span data-ttu-id="80216-131">类型</span><span class="sxs-lookup"><span data-stu-id="80216-131">Type</span></span>|<span data-ttu-id="80216-132">说明</span><span class="sxs-lookup"><span data-stu-id="80216-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80216-133">id</span><span class="sxs-lookup"><span data-stu-id="80216-133">id</span></span>|<span data-ttu-id="80216-134">String</span><span class="sxs-lookup"><span data-stu-id="80216-134">String</span></span>|<span data-ttu-id="80216-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80216-135">Key of the entity.</span></span>|
|<span data-ttu-id="80216-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="80216-136">deviceName</span></span>|<span data-ttu-id="80216-137">String</span><span class="sxs-lookup"><span data-stu-id="80216-137">String</span></span>|<span data-ttu-id="80216-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="80216-138">Device name.</span></span>|
|<span data-ttu-id="80216-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="80216-139">deviceId</span></span>|<span data-ttu-id="80216-140">String</span><span class="sxs-lookup"><span data-stu-id="80216-140">String</span></span>|<span data-ttu-id="80216-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="80216-141">Device Id.</span></span>|
|<span data-ttu-id="80216-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80216-142">lastSyncDateTime</span></span>|<span data-ttu-id="80216-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80216-143">DateTimeOffset</span></span>|<span data-ttu-id="80216-144">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="80216-144">Last sync date and time.</span></span>|
|<span data-ttu-id="80216-145">installState</span><span class="sxs-lookup"><span data-stu-id="80216-145">installState</span></span>|[<span data-ttu-id="80216-146">installState</span><span class="sxs-lookup"><span data-stu-id="80216-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="80216-147">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="80216-147">The install state of the eBook.</span></span> <span data-ttu-id="80216-148">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="80216-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="80216-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="80216-149">errorCode</span></span>|<span data-ttu-id="80216-150">String</span><span class="sxs-lookup"><span data-stu-id="80216-150">String</span></span>|<span data-ttu-id="80216-151">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="80216-151">The error code for install failures.</span></span>|
|<span data-ttu-id="80216-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="80216-152">osVersion</span></span>|<span data-ttu-id="80216-153">String</span><span class="sxs-lookup"><span data-stu-id="80216-153">String</span></span>|<span data-ttu-id="80216-154">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="80216-154">OS Version.</span></span>|
|<span data-ttu-id="80216-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="80216-155">osDescription</span></span>|<span data-ttu-id="80216-156">String</span><span class="sxs-lookup"><span data-stu-id="80216-156">String</span></span>|<span data-ttu-id="80216-157">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="80216-157">OS Description.</span></span>|
|<span data-ttu-id="80216-158">userName</span><span class="sxs-lookup"><span data-stu-id="80216-158">userName</span></span>|<span data-ttu-id="80216-159">String</span><span class="sxs-lookup"><span data-stu-id="80216-159">String</span></span>|<span data-ttu-id="80216-160">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="80216-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="80216-161">响应</span><span class="sxs-lookup"><span data-stu-id="80216-161">Response</span></span>
<span data-ttu-id="80216-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80216-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80216-163">示例</span><span class="sxs-lookup"><span data-stu-id="80216-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="80216-164">请求</span><span class="sxs-lookup"><span data-stu-id="80216-164">Request</span></span>
<span data-ttu-id="80216-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80216-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80216-166">响应</span><span class="sxs-lookup"><span data-stu-id="80216-166">Response</span></span>
<span data-ttu-id="80216-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80216-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




