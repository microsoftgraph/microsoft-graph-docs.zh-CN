---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d73f1cc881d918f385bfdc8d98cf9a1451a554e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394787"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="e0266-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="e0266-103">Update deviceInstallState</span></span>

> <span data-ttu-id="e0266-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e0266-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0266-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0266-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0266-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0266-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0266-107">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0266-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0266-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0266-108">Prerequisites</span></span>
<span data-ttu-id="e0266-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e0266-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e0266-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0266-111">Permission type</span></span>|<span data-ttu-id="e0266-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0266-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0266-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0266-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0266-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0266-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0266-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0266-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0266-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0266-116">Not supported.</span></span>|
|<span data-ttu-id="e0266-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0266-117">Application</span></span>|<span data-ttu-id="e0266-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0266-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0266-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0266-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e0266-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0266-120">Request headers</span></span>
|<span data-ttu-id="e0266-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0266-121">Header</span></span>|<span data-ttu-id="e0266-122">值</span><span class="sxs-lookup"><span data-stu-id="e0266-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0266-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0266-123">Authorization</span></span>|<span data-ttu-id="e0266-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0266-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0266-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0266-125">Accept</span></span>|<span data-ttu-id="e0266-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0266-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0266-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0266-127">Request body</span></span>
<span data-ttu-id="e0266-128">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0266-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="e0266-129">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0266-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="e0266-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0266-130">Property</span></span>|<span data-ttu-id="e0266-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0266-131">Type</span></span>|<span data-ttu-id="e0266-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0266-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0266-133">id</span><span class="sxs-lookup"><span data-stu-id="e0266-133">id</span></span>|<span data-ttu-id="e0266-134">String</span><span class="sxs-lookup"><span data-stu-id="e0266-134">String</span></span>|<span data-ttu-id="e0266-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0266-135">Key of the entity.</span></span>|
|<span data-ttu-id="e0266-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="e0266-136">deviceName</span></span>|<span data-ttu-id="e0266-137">String</span><span class="sxs-lookup"><span data-stu-id="e0266-137">String</span></span>|<span data-ttu-id="e0266-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="e0266-138">Device name.</span></span>|
|<span data-ttu-id="e0266-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="e0266-139">deviceId</span></span>|<span data-ttu-id="e0266-140">String</span><span class="sxs-lookup"><span data-stu-id="e0266-140">String</span></span>|<span data-ttu-id="e0266-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="e0266-141">Device Id.</span></span>|
|<span data-ttu-id="e0266-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e0266-142">lastSyncDateTime</span></span>|<span data-ttu-id="e0266-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0266-143">DateTimeOffset</span></span>|<span data-ttu-id="e0266-144">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0266-144">Last sync date and time.</span></span>|
|<span data-ttu-id="e0266-145">installState</span><span class="sxs-lookup"><span data-stu-id="e0266-145">installState</span></span>|[<span data-ttu-id="e0266-146">installState</span><span class="sxs-lookup"><span data-stu-id="e0266-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="e0266-147">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e0266-147">The install state of the eBook.</span></span> <span data-ttu-id="e0266-148">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="e0266-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="e0266-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="e0266-149">errorCode</span></span>|<span data-ttu-id="e0266-150">String</span><span class="sxs-lookup"><span data-stu-id="e0266-150">String</span></span>|<span data-ttu-id="e0266-151">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="e0266-151">The error code for install failures.</span></span>|
|<span data-ttu-id="e0266-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="e0266-152">osVersion</span></span>|<span data-ttu-id="e0266-153">String</span><span class="sxs-lookup"><span data-stu-id="e0266-153">String</span></span>|<span data-ttu-id="e0266-154">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e0266-154">OS Version.</span></span>|
|<span data-ttu-id="e0266-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="e0266-155">osDescription</span></span>|<span data-ttu-id="e0266-156">String</span><span class="sxs-lookup"><span data-stu-id="e0266-156">String</span></span>|<span data-ttu-id="e0266-157">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="e0266-157">OS Description.</span></span>|
|<span data-ttu-id="e0266-158">userName</span><span class="sxs-lookup"><span data-stu-id="e0266-158">userName</span></span>|<span data-ttu-id="e0266-159">String</span><span class="sxs-lookup"><span data-stu-id="e0266-159">String</span></span>|<span data-ttu-id="e0266-160">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="e0266-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="e0266-161">响应</span><span class="sxs-lookup"><span data-stu-id="e0266-161">Response</span></span>
<span data-ttu-id="e0266-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0266-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0266-163">示例</span><span class="sxs-lookup"><span data-stu-id="e0266-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0266-164">请求</span><span class="sxs-lookup"><span data-stu-id="e0266-164">Request</span></span>
<span data-ttu-id="e0266-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0266-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0266-166">响应</span><span class="sxs-lookup"><span data-stu-id="e0266-166">Response</span></span>
<span data-ttu-id="e0266-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0266-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




