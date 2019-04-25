---
title: 创建 windowsManagementAppHealthState
description: 创建新的 windowsManagementAppHealthState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c275825fb5222fcb1a77ed2bd8abce6d76c75594
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534372"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="2c221-103">创建 windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="2c221-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="2c221-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c221-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c221-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c221-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c221-106">创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c221-106">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c221-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c221-107">Prerequisites</span></span>
<span data-ttu-id="2c221-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c221-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c221-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c221-110">Permission type</span></span>|<span data-ttu-id="2c221-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c221-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c221-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c221-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c221-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c221-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2c221-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c221-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c221-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c221-115">Not supported.</span></span>|
|<span data-ttu-id="2c221-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c221-116">Application</span></span>|<span data-ttu-id="2c221-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c221-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c221-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c221-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="2c221-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c221-119">Request headers</span></span>
|<span data-ttu-id="2c221-120">标头</span><span class="sxs-lookup"><span data-stu-id="2c221-120">Header</span></span>|<span data-ttu-id="2c221-121">值</span><span class="sxs-lookup"><span data-stu-id="2c221-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c221-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c221-122">Authorization</span></span>|<span data-ttu-id="2c221-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c221-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c221-124">接受</span><span class="sxs-lookup"><span data-stu-id="2c221-124">Accept</span></span>|<span data-ttu-id="2c221-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c221-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c221-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c221-126">Request body</span></span>
<span data-ttu-id="2c221-127">在请求正文中, 提供 windowsManagementAppHealthState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c221-127">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="2c221-128">下表显示创建 windowsManagementAppHealthState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c221-128">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="2c221-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c221-129">Property</span></span>|<span data-ttu-id="2c221-130">类型</span><span class="sxs-lookup"><span data-stu-id="2c221-130">Type</span></span>|<span data-ttu-id="2c221-131">说明</span><span class="sxs-lookup"><span data-stu-id="2c221-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c221-132">id</span><span class="sxs-lookup"><span data-stu-id="2c221-132">id</span></span>|<span data-ttu-id="2c221-133">String</span><span class="sxs-lookup"><span data-stu-id="2c221-133">String</span></span>|<span data-ttu-id="2c221-134">Windows management 应用运行状况状态的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="2c221-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="2c221-135">healthState</span><span class="sxs-lookup"><span data-stu-id="2c221-135">healthState</span></span>|[<span data-ttu-id="2c221-136">healthState</span><span class="sxs-lookup"><span data-stu-id="2c221-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="2c221-137">Windows 管理应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="2c221-137">Windows management app health state.</span></span> <span data-ttu-id="2c221-138">可取值为：`unknown`、`healthy`、`unhealthy`。</span><span class="sxs-lookup"><span data-stu-id="2c221-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="2c221-139">installedVersion</span><span class="sxs-lookup"><span data-stu-id="2c221-139">installedVersion</span></span>|<span data-ttu-id="2c221-140">String</span><span class="sxs-lookup"><span data-stu-id="2c221-140">String</span></span>|<span data-ttu-id="2c221-141">Windows 管理应用程序已安装版本。</span><span class="sxs-lookup"><span data-stu-id="2c221-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="2c221-142">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="2c221-142">lastCheckInDateTime</span></span>|<span data-ttu-id="2c221-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c221-143">DateTimeOffset</span></span>|<span data-ttu-id="2c221-144">Windows 管理应用程序上次签入时间。</span><span class="sxs-lookup"><span data-stu-id="2c221-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="2c221-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="2c221-145">deviceName</span></span>|<span data-ttu-id="2c221-146">String</span><span class="sxs-lookup"><span data-stu-id="2c221-146">String</span></span>|<span data-ttu-id="2c221-147">在其上安装 Windows management 应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="2c221-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="2c221-148">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="2c221-148">deviceOSVersion</span></span>|<span data-ttu-id="2c221-149">String</span><span class="sxs-lookup"><span data-stu-id="2c221-149">String</span></span>|<span data-ttu-id="2c221-150">windows 10 OS 版本的 windows management app 安装在该设备上。</span><span class="sxs-lookup"><span data-stu-id="2c221-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="2c221-151">响应</span><span class="sxs-lookup"><span data-stu-id="2c221-151">Response</span></span>
<span data-ttu-id="2c221-152">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c221-152">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c221-153">示例</span><span class="sxs-lookup"><span data-stu-id="2c221-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c221-154">请求</span><span class="sxs-lookup"><span data-stu-id="2c221-154">Request</span></span>
<span data-ttu-id="2c221-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c221-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c221-156">响应</span><span class="sxs-lookup"><span data-stu-id="2c221-156">Response</span></span>
<span data-ttu-id="2c221-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c221-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





