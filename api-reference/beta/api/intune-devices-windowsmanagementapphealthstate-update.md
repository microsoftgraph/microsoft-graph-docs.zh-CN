---
title: 更新 windowsManagementAppHealthState
description: 更新 windowsManagementAppHealthState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de6314de3699821f15125d75241d3df509d52c64
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160548"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="0f196-103">更新 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="0f196-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="0f196-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f196-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f196-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f196-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f196-106">更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0f196-106">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f196-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f196-107">Prerequisites</span></span>
<span data-ttu-id="0f196-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0f196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f196-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f196-110">Permission type</span></span>|<span data-ttu-id="0f196-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f196-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f196-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f196-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f196-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f196-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f196-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f196-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f196-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f196-115">Not supported.</span></span>|
|<span data-ttu-id="0f196-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f196-116">Application</span></span>|<span data-ttu-id="0f196-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f196-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f196-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f196-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="0f196-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f196-119">Request headers</span></span>
|<span data-ttu-id="0f196-120">标头</span><span class="sxs-lookup"><span data-stu-id="0f196-120">Header</span></span>|<span data-ttu-id="0f196-121">值</span><span class="sxs-lookup"><span data-stu-id="0f196-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f196-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f196-122">Authorization</span></span>|<span data-ttu-id="0f196-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f196-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f196-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0f196-124">Accept</span></span>|<span data-ttu-id="0f196-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f196-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f196-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f196-126">Request body</span></span>
<span data-ttu-id="0f196-127">在请求正文中, 提供[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f196-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="0f196-128">下表显示创建[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f196-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="0f196-129">属性</span><span class="sxs-lookup"><span data-stu-id="0f196-129">Property</span></span>|<span data-ttu-id="0f196-130">类型</span><span class="sxs-lookup"><span data-stu-id="0f196-130">Type</span></span>|<span data-ttu-id="0f196-131">说明</span><span class="sxs-lookup"><span data-stu-id="0f196-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f196-132">id</span><span class="sxs-lookup"><span data-stu-id="0f196-132">id</span></span>|<span data-ttu-id="0f196-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0f196-133">String</span></span>|<span data-ttu-id="0f196-134">Windows management 应用运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0f196-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="0f196-135">healthState</span><span class="sxs-lookup"><span data-stu-id="0f196-135">healthState</span></span>|[<span data-ttu-id="0f196-136">healthState</span><span class="sxs-lookup"><span data-stu-id="0f196-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="0f196-137">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="0f196-137">Windows management app health state.</span></span> <span data-ttu-id="0f196-138">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="0f196-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="0f196-139">installedVersion</span><span class="sxs-lookup"><span data-stu-id="0f196-139">installedVersion</span></span>|<span data-ttu-id="0f196-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0f196-140">String</span></span>|<span data-ttu-id="0f196-141">Windows 管理应用程序已安装版本。</span><span class="sxs-lookup"><span data-stu-id="0f196-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="0f196-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="0f196-142">lastCheckInDateTime</span></span>|<span data-ttu-id="0f196-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f196-143">DateTimeOffset</span></span>|<span data-ttu-id="0f196-144">Windows 管理应用程序上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="0f196-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="0f196-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="0f196-145">deviceName</span></span>|<span data-ttu-id="0f196-146">String</span><span class="sxs-lookup"><span data-stu-id="0f196-146">String</span></span>|<span data-ttu-id="0f196-147">在其上安装 Windows management 应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="0f196-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="0f196-148">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="0f196-148">deviceOSVersion</span></span>|<span data-ttu-id="0f196-149">字符串</span><span class="sxs-lookup"><span data-stu-id="0f196-149">String</span></span>|<span data-ttu-id="0f196-150">windows 10 OS 版本的 windows management app 安装在该设备上。</span><span class="sxs-lookup"><span data-stu-id="0f196-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="0f196-151">响应</span><span class="sxs-lookup"><span data-stu-id="0f196-151">Response</span></span>
<span data-ttu-id="0f196-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f196-152">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f196-153">示例</span><span class="sxs-lookup"><span data-stu-id="0f196-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f196-154">请求</span><span class="sxs-lookup"><span data-stu-id="0f196-154">Request</span></span>
<span data-ttu-id="0f196-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f196-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f196-156">响应</span><span class="sxs-lookup"><span data-stu-id="0f196-156">Response</span></span>
<span data-ttu-id="0f196-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f196-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




