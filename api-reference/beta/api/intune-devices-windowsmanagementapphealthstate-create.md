---
title: 创建 windowsManagementAppHealthState
description: 创建新的 windowsManagementAppHealthState 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ba082150ea5b032a4621bfea33b7d85f5ad2a16
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126380"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="76774-103">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="76774-103">Create windowsManagementAppHealthState</span></span>

<span data-ttu-id="76774-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76774-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76774-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76774-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76774-107">创建新的 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76774-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76774-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="76774-108">Prerequisites</span></span>
<span data-ttu-id="76774-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76774-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76774-111">Permission type</span></span>|<span data-ttu-id="76774-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76774-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76774-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76774-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76774-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76774-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="76774-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76774-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76774-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76774-116">Not supported.</span></span>|
|<span data-ttu-id="76774-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="76774-117">Application</span></span>|<span data-ttu-id="76774-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76774-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76774-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76774-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="76774-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="76774-120">Request headers</span></span>
|<span data-ttu-id="76774-121">标头</span><span class="sxs-lookup"><span data-stu-id="76774-121">Header</span></span>|<span data-ttu-id="76774-122">值</span><span class="sxs-lookup"><span data-stu-id="76774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76774-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76774-123">Authorization</span></span>|<span data-ttu-id="76774-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76774-125">接受</span><span class="sxs-lookup"><span data-stu-id="76774-125">Accept</span></span>|<span data-ttu-id="76774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76774-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="76774-127">Request body</span></span>
<span data-ttu-id="76774-128">在请求正文中，提供 windowsManagementAppHealthState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76774-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="76774-129">下表显示创建 windowsManagementAppHealthState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="76774-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="76774-130">属性</span><span class="sxs-lookup"><span data-stu-id="76774-130">Property</span></span>|<span data-ttu-id="76774-131">类型</span><span class="sxs-lookup"><span data-stu-id="76774-131">Type</span></span>|<span data-ttu-id="76774-132">说明</span><span class="sxs-lookup"><span data-stu-id="76774-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76774-133">id</span><span class="sxs-lookup"><span data-stu-id="76774-133">id</span></span>|<span data-ttu-id="76774-134">String</span><span class="sxs-lookup"><span data-stu-id="76774-134">String</span></span>|<span data-ttu-id="76774-135">Windows 管理应用运行状况状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="76774-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="76774-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="76774-136">This property is read-only.</span></span>|
|<span data-ttu-id="76774-137">healthState</span><span class="sxs-lookup"><span data-stu-id="76774-137">healthState</span></span>|[<span data-ttu-id="76774-138">healthState</span><span class="sxs-lookup"><span data-stu-id="76774-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="76774-139">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="76774-139">Windows management app health state.</span></span> <span data-ttu-id="76774-140">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="76774-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="76774-141">installedVersion</span><span class="sxs-lookup"><span data-stu-id="76774-141">installedVersion</span></span>|<span data-ttu-id="76774-142">String</span><span class="sxs-lookup"><span data-stu-id="76774-142">String</span></span>|<span data-ttu-id="76774-143">Windows 管理应用安装的版本。</span><span class="sxs-lookup"><span data-stu-id="76774-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="76774-144">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="76774-144">lastCheckInDateTime</span></span>|<span data-ttu-id="76774-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76774-145">DateTimeOffset</span></span>|<span data-ttu-id="76774-146">Windows 管理应用上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="76774-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="76774-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="76774-147">deviceName</span></span>|<span data-ttu-id="76774-148">String</span><span class="sxs-lookup"><span data-stu-id="76774-148">String</span></span>|<span data-ttu-id="76774-149">安装 Windows 管理应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="76774-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="76774-150">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="76774-150">deviceOSVersion</span></span>|<span data-ttu-id="76774-151">String</span><span class="sxs-lookup"><span data-stu-id="76774-151">String</span></span>|<span data-ttu-id="76774-152">安装了 Windows 管理应用的设备的 Windows 10 操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="76774-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="76774-153">响应</span><span class="sxs-lookup"><span data-stu-id="76774-153">Response</span></span>
<span data-ttu-id="76774-154">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76774-154">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76774-155">示例</span><span class="sxs-lookup"><span data-stu-id="76774-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="76774-156">请求</span><span class="sxs-lookup"><span data-stu-id="76774-156">Request</span></span>
<span data-ttu-id="76774-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76774-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76774-158">响应</span><span class="sxs-lookup"><span data-stu-id="76774-158">Response</span></span>
<span data-ttu-id="76774-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76774-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




