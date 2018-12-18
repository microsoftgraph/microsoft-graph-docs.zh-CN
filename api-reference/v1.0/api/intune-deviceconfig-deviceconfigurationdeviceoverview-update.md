---
title: 更新 deviceConfigurationDeviceOverview
description: 更新 deviceConfigurationDeviceOverview 对象的属性。
author: tfitzmac
ms.openlocfilehash: 5b47dfc9b3a716abcea1d77d093e2cce1d927efe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301139"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="e9bf8-103">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e9bf8-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="e9bf8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9bf8-105">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9bf8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e9bf8-106">Prerequisites</span></span>
<span data-ttu-id="e9bf8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e9bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9bf8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9bf8-109">Permission type</span></span>|<span data-ttu-id="e9bf8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e9bf8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9bf8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9bf8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9bf8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9bf8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9bf8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9bf8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9bf8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-114">Not supported.</span></span>|
|<span data-ttu-id="e9bf8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9bf8-115">Application</span></span>|<span data-ttu-id="e9bf8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9bf8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9bf8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="e9bf8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9bf8-118">Request headers</span></span>
|<span data-ttu-id="e9bf8-119">标头</span><span class="sxs-lookup"><span data-stu-id="e9bf8-119">Header</span></span>|<span data-ttu-id="e9bf8-120">值</span><span class="sxs-lookup"><span data-stu-id="e9bf8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9bf8-121">授权</span><span class="sxs-lookup"><span data-stu-id="e9bf8-121">Authorization</span></span>|<span data-ttu-id="e9bf8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9bf8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e9bf8-123">Accept</span></span>|<span data-ttu-id="e9bf8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e9bf8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9bf8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9bf8-125">Request body</span></span>
<span data-ttu-id="e9bf8-126">在请求正文中，提供 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="e9bf8-127">下表显示创建 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="e9bf8-128">属性</span><span class="sxs-lookup"><span data-stu-id="e9bf8-128">Property</span></span>|<span data-ttu-id="e9bf8-129">类型</span><span class="sxs-lookup"><span data-stu-id="e9bf8-129">Type</span></span>|<span data-ttu-id="e9bf8-130">说明</span><span class="sxs-lookup"><span data-stu-id="e9bf8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9bf8-131">id</span><span class="sxs-lookup"><span data-stu-id="e9bf8-131">id</span></span>|<span data-ttu-id="e9bf8-132">String</span><span class="sxs-lookup"><span data-stu-id="e9bf8-132">String</span></span>|<span data-ttu-id="e9bf8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-133">Key of the entity.</span></span>|
|<span data-ttu-id="e9bf8-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e9bf8-134">pendingCount</span></span>|<span data-ttu-id="e9bf8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bf8-135">Int32</span></span>|<span data-ttu-id="e9bf8-136">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="e9bf8-136">Number of pending devices</span></span>|
|<span data-ttu-id="e9bf8-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e9bf8-137">notApplicableCount</span></span>|<span data-ttu-id="e9bf8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bf8-138">Int32</span></span>|<span data-ttu-id="e9bf8-139">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="e9bf8-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="e9bf8-140">successCount</span><span class="sxs-lookup"><span data-stu-id="e9bf8-140">successCount</span></span>|<span data-ttu-id="e9bf8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bf8-141">Int32</span></span>|<span data-ttu-id="e9bf8-142">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="e9bf8-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="e9bf8-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="e9bf8-143">errorCount</span></span>|<span data-ttu-id="e9bf8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bf8-144">Int32</span></span>|<span data-ttu-id="e9bf8-145">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="e9bf8-145">Number of error devices</span></span>|
|<span data-ttu-id="e9bf8-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="e9bf8-146">failedCount</span></span>|<span data-ttu-id="e9bf8-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bf8-147">Int32</span></span>|<span data-ttu-id="e9bf8-148">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="e9bf8-148">Number of failed devices</span></span>|
|<span data-ttu-id="e9bf8-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e9bf8-149">lastUpdateDateTime</span></span>|<span data-ttu-id="e9bf8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9bf8-150">DateTimeOffset</span></span>|<span data-ttu-id="e9bf8-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="e9bf8-151">Last update time</span></span>|
|<span data-ttu-id="e9bf8-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e9bf8-152">configurationVersion</span></span>|<span data-ttu-id="e9bf8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bf8-153">Int32</span></span>|<span data-ttu-id="e9bf8-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="e9bf8-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="e9bf8-155">响应</span><span class="sxs-lookup"><span data-stu-id="e9bf8-155">Response</span></span>
<span data-ttu-id="e9bf8-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9bf8-157">示例</span><span class="sxs-lookup"><span data-stu-id="e9bf8-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9bf8-158">请求</span><span class="sxs-lookup"><span data-stu-id="e9bf8-158">Request</span></span>
<span data-ttu-id="e9bf8-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9bf8-160">响应</span><span class="sxs-lookup"><span data-stu-id="e9bf8-160">Response</span></span>
<span data-ttu-id="e9bf8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9bf8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



