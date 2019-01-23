---
title: 创建 windowsManagementAppHealthState
description: 创建新的 windowsManagementAppHealthState 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c3463e05c58d3b501955f3b04c49cbf112d8a63f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416522"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="969ae-103">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="969ae-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="969ae-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="969ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="969ae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="969ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="969ae-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="969ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="969ae-107">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="969ae-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="969ae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="969ae-108">Prerequisites</span></span>
<span data-ttu-id="969ae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="969ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="969ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="969ae-111">Permission type</span></span>|<span data-ttu-id="969ae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="969ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="969ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="969ae-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969ae-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="969ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="969ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="969ae-116">Not supported.</span></span>|
|<span data-ttu-id="969ae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="969ae-117">Application</span></span>|<span data-ttu-id="969ae-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="969ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="969ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="969ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="969ae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="969ae-120">Request headers</span></span>
|<span data-ttu-id="969ae-121">标头</span><span class="sxs-lookup"><span data-stu-id="969ae-121">Header</span></span>|<span data-ttu-id="969ae-122">值</span><span class="sxs-lookup"><span data-stu-id="969ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="969ae-123">Authorization</span></span>|<span data-ttu-id="969ae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="969ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="969ae-125">Accept</span></span>|<span data-ttu-id="969ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="969ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="969ae-127">Request body</span></span>
<span data-ttu-id="969ae-128">在请求正文中，提供 windowsManagementAppHealthState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="969ae-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="969ae-129">下表显示时创建 windowsManagementAppHealthState 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="969ae-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="969ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="969ae-130">Property</span></span>|<span data-ttu-id="969ae-131">类型</span><span class="sxs-lookup"><span data-stu-id="969ae-131">Type</span></span>|<span data-ttu-id="969ae-132">说明</span><span class="sxs-lookup"><span data-stu-id="969ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="969ae-133">id</span><span class="sxs-lookup"><span data-stu-id="969ae-133">id</span></span>|<span data-ttu-id="969ae-134">String</span><span class="sxs-lookup"><span data-stu-id="969ae-134">String</span></span>|<span data-ttu-id="969ae-135">Windows 管理应用程序的运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="969ae-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="969ae-136">healthState</span><span class="sxs-lookup"><span data-stu-id="969ae-136">healthState</span></span>|[<span data-ttu-id="969ae-137">healthState</span><span class="sxs-lookup"><span data-stu-id="969ae-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="969ae-138">Windows 管理应用程序的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="969ae-138">Windows management app health state.</span></span> <span data-ttu-id="969ae-139">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="969ae-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="969ae-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="969ae-140">installedVersion</span></span>|<span data-ttu-id="969ae-141">String</span><span class="sxs-lookup"><span data-stu-id="969ae-141">String</span></span>|<span data-ttu-id="969ae-142">Windows 管理应用程序安装的版本。</span><span class="sxs-lookup"><span data-stu-id="969ae-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="969ae-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="969ae-143">lastCheckInDateTime</span></span>|<span data-ttu-id="969ae-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969ae-144">DateTimeOffset</span></span>|<span data-ttu-id="969ae-145">Windows 管理应用程序上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="969ae-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="969ae-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="969ae-146">deviceName</span></span>|<span data-ttu-id="969ae-147">String</span><span class="sxs-lookup"><span data-stu-id="969ae-147">String</span></span>|<span data-ttu-id="969ae-148">设备的 Windows 安装管理应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="969ae-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="969ae-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="969ae-149">deviceOSVersion</span></span>|<span data-ttu-id="969ae-150">String</span><span class="sxs-lookup"><span data-stu-id="969ae-150">String</span></span>|<span data-ttu-id="969ae-151">Windows 10 OS 版本的 Windows 安装管理应用程序的设备。</span><span class="sxs-lookup"><span data-stu-id="969ae-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="969ae-152">响应</span><span class="sxs-lookup"><span data-stu-id="969ae-152">Response</span></span>
<span data-ttu-id="969ae-153">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="969ae-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969ae-154">示例</span><span class="sxs-lookup"><span data-stu-id="969ae-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="969ae-155">请求</span><span class="sxs-lookup"><span data-stu-id="969ae-155">Request</span></span>
<span data-ttu-id="969ae-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="969ae-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
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

### <a name="response"></a><span data-ttu-id="969ae-157">响应</span><span class="sxs-lookup"><span data-stu-id="969ae-157">Response</span></span>
<span data-ttu-id="969ae-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="969ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




