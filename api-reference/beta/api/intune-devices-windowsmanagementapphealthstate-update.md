---
title: 更新 windowsManagementAppHealthState
description: 更新 windowsManagementAppHealthState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4f956dc8ef3a1c4d65629d451396e274ae45f00
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944214"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="4b83f-103">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="4b83f-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="4b83f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b83f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b83f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b83f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b83f-106">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4b83f-106">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b83f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b83f-107">Prerequisites</span></span>
<span data-ttu-id="4b83f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b83f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b83f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b83f-110">Permission type</span></span>|<span data-ttu-id="4b83f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b83f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b83f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b83f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b83f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b83f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4b83f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b83f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b83f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b83f-115">Not supported.</span></span>|
|<span data-ttu-id="4b83f-116">Application</span><span class="sxs-lookup"><span data-stu-id="4b83f-116">Application</span></span>|<span data-ttu-id="4b83f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b83f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b83f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b83f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="4b83f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b83f-119">Request headers</span></span>
|<span data-ttu-id="4b83f-120">标头</span><span class="sxs-lookup"><span data-stu-id="4b83f-120">Header</span></span>|<span data-ttu-id="4b83f-121">值</span><span class="sxs-lookup"><span data-stu-id="4b83f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b83f-122">授权</span><span class="sxs-lookup"><span data-stu-id="4b83f-122">Authorization</span></span>|<span data-ttu-id="4b83f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b83f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b83f-124">接受</span><span class="sxs-lookup"><span data-stu-id="4b83f-124">Accept</span></span>|<span data-ttu-id="4b83f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b83f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b83f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b83f-126">Request body</span></span>
<span data-ttu-id="4b83f-127">在请求正文中，提供[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b83f-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="4b83f-128">下表显示创建[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4b83f-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="4b83f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4b83f-129">Property</span></span>|<span data-ttu-id="4b83f-130">类型</span><span class="sxs-lookup"><span data-stu-id="4b83f-130">Type</span></span>|<span data-ttu-id="4b83f-131">说明</span><span class="sxs-lookup"><span data-stu-id="4b83f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b83f-132">id</span><span class="sxs-lookup"><span data-stu-id="4b83f-132">id</span></span>|<span data-ttu-id="4b83f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4b83f-133">String</span></span>|<span data-ttu-id="4b83f-134">Windows 管理应用运行状况状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4b83f-134">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="4b83f-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4b83f-135">This property is read-only.</span></span>|
|<span data-ttu-id="4b83f-136">healthState</span><span class="sxs-lookup"><span data-stu-id="4b83f-136">healthState</span></span>|[<span data-ttu-id="4b83f-137">healthState</span><span class="sxs-lookup"><span data-stu-id="4b83f-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="4b83f-138">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="4b83f-138">Windows management app health state.</span></span> <span data-ttu-id="4b83f-139">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="4b83f-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="4b83f-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="4b83f-140">installedVersion</span></span>|<span data-ttu-id="4b83f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="4b83f-141">String</span></span>|<span data-ttu-id="4b83f-142">Windows 管理应用程序已安装版本。</span><span class="sxs-lookup"><span data-stu-id="4b83f-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="4b83f-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="4b83f-143">lastCheckInDateTime</span></span>|<span data-ttu-id="4b83f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b83f-144">DateTimeOffset</span></span>|<span data-ttu-id="4b83f-145">Windows 管理应用程序上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="4b83f-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="4b83f-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="4b83f-146">deviceName</span></span>|<span data-ttu-id="4b83f-147">String</span><span class="sxs-lookup"><span data-stu-id="4b83f-147">String</span></span>|<span data-ttu-id="4b83f-148">在其上安装 Windows management 应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="4b83f-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="4b83f-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="4b83f-149">deviceOSVersion</span></span>|<span data-ttu-id="4b83f-150">字符串</span><span class="sxs-lookup"><span data-stu-id="4b83f-150">String</span></span>|<span data-ttu-id="4b83f-151">Windows 10 OS 版本的 Windows management app 安装在该设备上。</span><span class="sxs-lookup"><span data-stu-id="4b83f-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="4b83f-152">响应</span><span class="sxs-lookup"><span data-stu-id="4b83f-152">Response</span></span>
<span data-ttu-id="4b83f-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4b83f-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b83f-154">示例</span><span class="sxs-lookup"><span data-stu-id="4b83f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b83f-155">请求</span><span class="sxs-lookup"><span data-stu-id="4b83f-155">Request</span></span>
<span data-ttu-id="4b83f-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b83f-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="4b83f-157">响应</span><span class="sxs-lookup"><span data-stu-id="4b83f-157">Response</span></span>
<span data-ttu-id="4b83f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b83f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```





