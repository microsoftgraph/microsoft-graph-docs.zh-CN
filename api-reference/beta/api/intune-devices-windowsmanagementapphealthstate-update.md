---
title: 更新 windowsManagementAppHealthState
description: 更新 windowsManagementAppHealthState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88bfa7732662a1a3d2d0f7b60835a3a83bde90ad
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126323"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="a30d0-103">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="a30d0-103">Update windowsManagementAppHealthState</span></span>

<span data-ttu-id="a30d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a30d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a30d0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a30d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a30d0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a30d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a30d0-107">更新 [windowsManagementAppHealthState 对象](../resources/intune-devices-windowsmanagementapphealthstate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a30d0-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a30d0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a30d0-108">Prerequisites</span></span>
<span data-ttu-id="a30d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a30d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a30d0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a30d0-111">Permission type</span></span>|<span data-ttu-id="a30d0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a30d0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a30d0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a30d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a30d0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a30d0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a30d0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a30d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a30d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a30d0-116">Not supported.</span></span>|
|<span data-ttu-id="a30d0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a30d0-117">Application</span></span>|<span data-ttu-id="a30d0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a30d0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a30d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a30d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a30d0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a30d0-120">Request headers</span></span>
|<span data-ttu-id="a30d0-121">标头</span><span class="sxs-lookup"><span data-stu-id="a30d0-121">Header</span></span>|<span data-ttu-id="a30d0-122">值</span><span class="sxs-lookup"><span data-stu-id="a30d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a30d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a30d0-123">Authorization</span></span>|<span data-ttu-id="a30d0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a30d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a30d0-125">接受</span><span class="sxs-lookup"><span data-stu-id="a30d0-125">Accept</span></span>|<span data-ttu-id="a30d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a30d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a30d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a30d0-127">Request body</span></span>
<span data-ttu-id="a30d0-128">在请求正文中，提供 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a30d0-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="a30d0-129">下表显示创建 [windowsManagementAppHealthState 时所需的属性](../resources/intune-devices-windowsmanagementapphealthstate.md)。</span><span class="sxs-lookup"><span data-stu-id="a30d0-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="a30d0-130">属性</span><span class="sxs-lookup"><span data-stu-id="a30d0-130">Property</span></span>|<span data-ttu-id="a30d0-131">类型</span><span class="sxs-lookup"><span data-stu-id="a30d0-131">Type</span></span>|<span data-ttu-id="a30d0-132">说明</span><span class="sxs-lookup"><span data-stu-id="a30d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a30d0-133">id</span><span class="sxs-lookup"><span data-stu-id="a30d0-133">id</span></span>|<span data-ttu-id="a30d0-134">String</span><span class="sxs-lookup"><span data-stu-id="a30d0-134">String</span></span>|<span data-ttu-id="a30d0-135">Windows 管理应用运行状况状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a30d0-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="a30d0-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a30d0-136">This property is read-only.</span></span>|
|<span data-ttu-id="a30d0-137">healthState</span><span class="sxs-lookup"><span data-stu-id="a30d0-137">healthState</span></span>|[<span data-ttu-id="a30d0-138">healthState</span><span class="sxs-lookup"><span data-stu-id="a30d0-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="a30d0-139">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="a30d0-139">Windows management app health state.</span></span> <span data-ttu-id="a30d0-140">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="a30d0-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="a30d0-141">installedVersion</span><span class="sxs-lookup"><span data-stu-id="a30d0-141">installedVersion</span></span>|<span data-ttu-id="a30d0-142">String</span><span class="sxs-lookup"><span data-stu-id="a30d0-142">String</span></span>|<span data-ttu-id="a30d0-143">Windows 管理应用安装的版本。</span><span class="sxs-lookup"><span data-stu-id="a30d0-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="a30d0-144">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="a30d0-144">lastCheckInDateTime</span></span>|<span data-ttu-id="a30d0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a30d0-145">DateTimeOffset</span></span>|<span data-ttu-id="a30d0-146">Windows 管理应用上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="a30d0-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="a30d0-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="a30d0-147">deviceName</span></span>|<span data-ttu-id="a30d0-148">String</span><span class="sxs-lookup"><span data-stu-id="a30d0-148">String</span></span>|<span data-ttu-id="a30d0-149">安装 Windows 管理应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="a30d0-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="a30d0-150">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="a30d0-150">deviceOSVersion</span></span>|<span data-ttu-id="a30d0-151">String</span><span class="sxs-lookup"><span data-stu-id="a30d0-151">String</span></span>|<span data-ttu-id="a30d0-152">安装了 Windows 管理应用的设备的 Windows 10 操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a30d0-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="a30d0-153">响应</span><span class="sxs-lookup"><span data-stu-id="a30d0-153">Response</span></span>
<span data-ttu-id="a30d0-154">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a30d0-154">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a30d0-155">示例</span><span class="sxs-lookup"><span data-stu-id="a30d0-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="a30d0-156">请求</span><span class="sxs-lookup"><span data-stu-id="a30d0-156">Request</span></span>
<span data-ttu-id="a30d0-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a30d0-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a30d0-158">响应</span><span class="sxs-lookup"><span data-stu-id="a30d0-158">Response</span></span>
<span data-ttu-id="a30d0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a30d0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




