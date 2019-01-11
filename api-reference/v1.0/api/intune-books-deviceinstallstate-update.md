---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0962abe32198d684a158547a3af390cccfab22d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855641"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="9e337-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9e337-103">Update deviceInstallState</span></span>

> <span data-ttu-id="9e337-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e337-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e337-105">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e337-105">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e337-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e337-106">Prerequisites</span></span>
<span data-ttu-id="9e337-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9e337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e337-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e337-109">Permission type</span></span>|<span data-ttu-id="9e337-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e337-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e337-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e337-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e337-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e337-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9e337-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e337-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e337-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e337-114">Not supported.</span></span>|
|<span data-ttu-id="9e337-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e337-115">Application</span></span>|<span data-ttu-id="9e337-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e337-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e337-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e337-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9e337-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e337-118">Request headers</span></span>
|<span data-ttu-id="9e337-119">标头</span><span class="sxs-lookup"><span data-stu-id="9e337-119">Header</span></span>|<span data-ttu-id="9e337-120">值</span><span class="sxs-lookup"><span data-stu-id="9e337-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e337-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e337-121">Authorization</span></span>|<span data-ttu-id="9e337-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e337-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e337-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9e337-123">Accept</span></span>|<span data-ttu-id="9e337-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e337-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e337-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e337-125">Request body</span></span>
<span data-ttu-id="9e337-126">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e337-126">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="9e337-127">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e337-127">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="9e337-128">属性</span><span class="sxs-lookup"><span data-stu-id="9e337-128">Property</span></span>|<span data-ttu-id="9e337-129">类型</span><span class="sxs-lookup"><span data-stu-id="9e337-129">Type</span></span>|<span data-ttu-id="9e337-130">说明</span><span class="sxs-lookup"><span data-stu-id="9e337-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e337-131">id</span><span class="sxs-lookup"><span data-stu-id="9e337-131">id</span></span>|<span data-ttu-id="9e337-132">String</span><span class="sxs-lookup"><span data-stu-id="9e337-132">String</span></span>|<span data-ttu-id="9e337-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e337-133">Key of the entity.</span></span>|
|<span data-ttu-id="9e337-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="9e337-134">deviceName</span></span>|<span data-ttu-id="9e337-135">String</span><span class="sxs-lookup"><span data-stu-id="9e337-135">String</span></span>|<span data-ttu-id="9e337-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="9e337-136">Device name.</span></span>|
|<span data-ttu-id="9e337-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="9e337-137">deviceId</span></span>|<span data-ttu-id="9e337-138">String</span><span class="sxs-lookup"><span data-stu-id="9e337-138">String</span></span>|<span data-ttu-id="9e337-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="9e337-139">Device Id.</span></span>|
|<span data-ttu-id="9e337-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9e337-140">lastSyncDateTime</span></span>|<span data-ttu-id="9e337-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e337-141">DateTimeOffset</span></span>|<span data-ttu-id="9e337-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9e337-142">Last sync date and time.</span></span>|
|<span data-ttu-id="9e337-143">installState</span><span class="sxs-lookup"><span data-stu-id="9e337-143">installState</span></span>|[<span data-ttu-id="9e337-144">installState</span><span class="sxs-lookup"><span data-stu-id="9e337-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="9e337-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9e337-145">The install state of the eBook.</span></span> <span data-ttu-id="9e337-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9e337-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="9e337-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="9e337-147">errorCode</span></span>|<span data-ttu-id="9e337-148">String</span><span class="sxs-lookup"><span data-stu-id="9e337-148">String</span></span>|<span data-ttu-id="9e337-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9e337-149">The error code for install failures.</span></span>|
|<span data-ttu-id="9e337-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="9e337-150">osVersion</span></span>|<span data-ttu-id="9e337-151">String</span><span class="sxs-lookup"><span data-stu-id="9e337-151">String</span></span>|<span data-ttu-id="9e337-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9e337-152">OS Version.</span></span>|
|<span data-ttu-id="9e337-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="9e337-153">osDescription</span></span>|<span data-ttu-id="9e337-154">String</span><span class="sxs-lookup"><span data-stu-id="9e337-154">String</span></span>|<span data-ttu-id="9e337-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="9e337-155">OS Description.</span></span>|
|<span data-ttu-id="9e337-156">userName</span><span class="sxs-lookup"><span data-stu-id="9e337-156">userName</span></span>|<span data-ttu-id="9e337-157">String</span><span class="sxs-lookup"><span data-stu-id="9e337-157">String</span></span>|<span data-ttu-id="9e337-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="9e337-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="9e337-159">响应</span><span class="sxs-lookup"><span data-stu-id="9e337-159">Response</span></span>
<span data-ttu-id="9e337-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e337-160">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e337-161">示例</span><span class="sxs-lookup"><span data-stu-id="9e337-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e337-162">请求</span><span class="sxs-lookup"><span data-stu-id="9e337-162">Request</span></span>
<span data-ttu-id="9e337-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e337-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e337-164">响应</span><span class="sxs-lookup"><span data-stu-id="9e337-164">Response</span></span>
<span data-ttu-id="9e337-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e337-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



