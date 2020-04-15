---
title: 更新 deviceConfigurationDeviceOverview
description: 更新 deviceConfigurationDeviceOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30277770a143e0a0ebc6212d8944beda517bc5e1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407559"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="5af20-103">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5af20-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="5af20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5af20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5af20-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5af20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5af20-106">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5af20-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5af20-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5af20-107">Prerequisites</span></span>
<span data-ttu-id="5af20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5af20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5af20-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5af20-110">Permission type</span></span>|<span data-ttu-id="5af20-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5af20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5af20-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5af20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5af20-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5af20-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5af20-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5af20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5af20-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5af20-115">Not supported.</span></span>|
|<span data-ttu-id="5af20-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5af20-116">Application</span></span>|<span data-ttu-id="5af20-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5af20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5af20-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5af20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="5af20-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5af20-119">Request headers</span></span>
|<span data-ttu-id="5af20-120">标头</span><span class="sxs-lookup"><span data-stu-id="5af20-120">Header</span></span>|<span data-ttu-id="5af20-121">值</span><span class="sxs-lookup"><span data-stu-id="5af20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5af20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5af20-122">Authorization</span></span>|<span data-ttu-id="5af20-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5af20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5af20-124">接受</span><span class="sxs-lookup"><span data-stu-id="5af20-124">Accept</span></span>|<span data-ttu-id="5af20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5af20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af20-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5af20-126">Request body</span></span>
<span data-ttu-id="5af20-127">在请求正文中，提供 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5af20-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="5af20-128">下表显示创建 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5af20-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="5af20-129">属性</span><span class="sxs-lookup"><span data-stu-id="5af20-129">Property</span></span>|<span data-ttu-id="5af20-130">类型</span><span class="sxs-lookup"><span data-stu-id="5af20-130">Type</span></span>|<span data-ttu-id="5af20-131">说明</span><span class="sxs-lookup"><span data-stu-id="5af20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af20-132">id</span><span class="sxs-lookup"><span data-stu-id="5af20-132">id</span></span>|<span data-ttu-id="5af20-133">String</span><span class="sxs-lookup"><span data-stu-id="5af20-133">String</span></span>|<span data-ttu-id="5af20-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5af20-134">Key of the entity.</span></span>|
|<span data-ttu-id="5af20-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="5af20-135">pendingCount</span></span>|<span data-ttu-id="5af20-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5af20-136">Int32</span></span>|<span data-ttu-id="5af20-137">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="5af20-137">Number of pending devices</span></span>|
|<span data-ttu-id="5af20-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5af20-138">notApplicableCount</span></span>|<span data-ttu-id="5af20-139">Int32</span><span class="sxs-lookup"><span data-stu-id="5af20-139">Int32</span></span>|<span data-ttu-id="5af20-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="5af20-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="5af20-141">successCount</span><span class="sxs-lookup"><span data-stu-id="5af20-141">successCount</span></span>|<span data-ttu-id="5af20-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5af20-142">Int32</span></span>|<span data-ttu-id="5af20-143">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="5af20-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="5af20-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="5af20-144">errorCount</span></span>|<span data-ttu-id="5af20-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5af20-145">Int32</span></span>|<span data-ttu-id="5af20-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="5af20-146">Number of error devices</span></span>|
|<span data-ttu-id="5af20-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="5af20-147">failedCount</span></span>|<span data-ttu-id="5af20-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5af20-148">Int32</span></span>|<span data-ttu-id="5af20-149">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="5af20-149">Number of failed devices</span></span>|
|<span data-ttu-id="5af20-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5af20-150">lastUpdateDateTime</span></span>|<span data-ttu-id="5af20-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5af20-151">DateTimeOffset</span></span>|<span data-ttu-id="5af20-152">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="5af20-152">Last update time</span></span>|
|<span data-ttu-id="5af20-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="5af20-153">configurationVersion</span></span>|<span data-ttu-id="5af20-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5af20-154">Int32</span></span>|<span data-ttu-id="5af20-155">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="5af20-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="5af20-156">响应</span><span class="sxs-lookup"><span data-stu-id="5af20-156">Response</span></span>
<span data-ttu-id="5af20-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5af20-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5af20-158">示例</span><span class="sxs-lookup"><span data-stu-id="5af20-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5af20-159">请求</span><span class="sxs-lookup"><span data-stu-id="5af20-159">Request</span></span>
<span data-ttu-id="5af20-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5af20-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="5af20-161">响应</span><span class="sxs-lookup"><span data-stu-id="5af20-161">Response</span></span>
<span data-ttu-id="5af20-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5af20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```






