---
title: 更新 deviceInstallState
description: 更新 deviceInstallState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 826a78585d206126c036322fe9784c32178a5583
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259498"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="b18bc-103">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="b18bc-103">Update deviceInstallState</span></span>

> <span data-ttu-id="b18bc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b18bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b18bc-105">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b18bc-105">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b18bc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b18bc-106">Prerequisites</span></span>
<span data-ttu-id="b18bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b18bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b18bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b18bc-109">Permission type</span></span>|<span data-ttu-id="b18bc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b18bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b18bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b18bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b18bc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b18bc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b18bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b18bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b18bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b18bc-114">Not supported.</span></span>|
|<span data-ttu-id="b18bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b18bc-115">Application</span></span>|<span data-ttu-id="b18bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b18bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b18bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b18bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b18bc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b18bc-118">Request headers</span></span>
|<span data-ttu-id="b18bc-119">标头</span><span class="sxs-lookup"><span data-stu-id="b18bc-119">Header</span></span>|<span data-ttu-id="b18bc-120">值</span><span class="sxs-lookup"><span data-stu-id="b18bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b18bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b18bc-121">Authorization</span></span>|<span data-ttu-id="b18bc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b18bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b18bc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b18bc-123">Accept</span></span>|<span data-ttu-id="b18bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b18bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b18bc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b18bc-125">Request body</span></span>
<span data-ttu-id="b18bc-126">在请求正文中，提供 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b18bc-126">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="b18bc-127">下表显示创建 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b18bc-127">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="b18bc-128">属性</span><span class="sxs-lookup"><span data-stu-id="b18bc-128">Property</span></span>|<span data-ttu-id="b18bc-129">类型</span><span class="sxs-lookup"><span data-stu-id="b18bc-129">Type</span></span>|<span data-ttu-id="b18bc-130">说明</span><span class="sxs-lookup"><span data-stu-id="b18bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b18bc-131">id</span><span class="sxs-lookup"><span data-stu-id="b18bc-131">id</span></span>|<span data-ttu-id="b18bc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b18bc-132">String</span></span>|<span data-ttu-id="b18bc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b18bc-133">Key of the entity.</span></span>|
|<span data-ttu-id="b18bc-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="b18bc-134">deviceName</span></span>|<span data-ttu-id="b18bc-135">String</span><span class="sxs-lookup"><span data-stu-id="b18bc-135">String</span></span>|<span data-ttu-id="b18bc-136">设备名称。</span><span class="sxs-lookup"><span data-stu-id="b18bc-136">Device name.</span></span>|
|<span data-ttu-id="b18bc-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="b18bc-137">deviceId</span></span>|<span data-ttu-id="b18bc-138">String</span><span class="sxs-lookup"><span data-stu-id="b18bc-138">String</span></span>|<span data-ttu-id="b18bc-139">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="b18bc-139">Device Id.</span></span>|
|<span data-ttu-id="b18bc-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b18bc-140">lastSyncDateTime</span></span>|<span data-ttu-id="b18bc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18bc-141">DateTimeOffset</span></span>|<span data-ttu-id="b18bc-142">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b18bc-142">Last sync date and time.</span></span>|
|<span data-ttu-id="b18bc-143">installState</span><span class="sxs-lookup"><span data-stu-id="b18bc-143">installState</span></span>|[<span data-ttu-id="b18bc-144">installState</span><span class="sxs-lookup"><span data-stu-id="b18bc-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="b18bc-145">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="b18bc-145">The install state of the eBook.</span></span> <span data-ttu-id="b18bc-146">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="b18bc-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="b18bc-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="b18bc-147">errorCode</span></span>|<span data-ttu-id="b18bc-148">String</span><span class="sxs-lookup"><span data-stu-id="b18bc-148">String</span></span>|<span data-ttu-id="b18bc-149">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="b18bc-149">The error code for install failures.</span></span>|
|<span data-ttu-id="b18bc-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="b18bc-150">osVersion</span></span>|<span data-ttu-id="b18bc-151">String</span><span class="sxs-lookup"><span data-stu-id="b18bc-151">String</span></span>|<span data-ttu-id="b18bc-152">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b18bc-152">OS Version.</span></span>|
|<span data-ttu-id="b18bc-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="b18bc-153">osDescription</span></span>|<span data-ttu-id="b18bc-154">String</span><span class="sxs-lookup"><span data-stu-id="b18bc-154">String</span></span>|<span data-ttu-id="b18bc-155">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="b18bc-155">OS Description.</span></span>|
|<span data-ttu-id="b18bc-156">userName</span><span class="sxs-lookup"><span data-stu-id="b18bc-156">userName</span></span>|<span data-ttu-id="b18bc-157">String</span><span class="sxs-lookup"><span data-stu-id="b18bc-157">String</span></span>|<span data-ttu-id="b18bc-158">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="b18bc-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="b18bc-159">响应</span><span class="sxs-lookup"><span data-stu-id="b18bc-159">Response</span></span>
<span data-ttu-id="b18bc-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b18bc-160">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b18bc-161">示例</span><span class="sxs-lookup"><span data-stu-id="b18bc-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="b18bc-162">请求</span><span class="sxs-lookup"><span data-stu-id="b18bc-162">Request</span></span>
<span data-ttu-id="b18bc-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b18bc-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b18bc-164">响应</span><span class="sxs-lookup"><span data-stu-id="b18bc-164">Response</span></span>
<span data-ttu-id="b18bc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b18bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



