---
title: 更新 deviceHealthScriptAssignment
description: 更新 deviceHealthScriptAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 048ac284ab8e5754219b3ef86ce37c0aae01969d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792385"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="1e8ae-103">更新 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="1e8ae-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="1e8ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e8ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e8ae-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e8ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e8ae-107">更新[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e8ae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e8ae-108">Prerequisites</span></span>
<span data-ttu-id="1e8ae-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1e8ae-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1e8ae-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e8ae-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e8ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e8ae-111">Permission type</span></span>|<span data-ttu-id="1e8ae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e8ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e8ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e8ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e8ae-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e8ae-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1e8ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e8ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e8ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-116">Not supported.</span></span>|
|<span data-ttu-id="1e8ae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e8ae-117">Application</span></span>|<span data-ttu-id="1e8ae-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e8ae-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e8ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e8ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1e8ae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e8ae-120">Request headers</span></span>
|<span data-ttu-id="1e8ae-121">标头</span><span class="sxs-lookup"><span data-stu-id="1e8ae-121">Header</span></span>|<span data-ttu-id="1e8ae-122">值</span><span class="sxs-lookup"><span data-stu-id="1e8ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e8ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e8ae-123">Authorization</span></span>|<span data-ttu-id="1e8ae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e8ae-125">接受</span><span class="sxs-lookup"><span data-stu-id="1e8ae-125">Accept</span></span>|<span data-ttu-id="1e8ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e8ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e8ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e8ae-127">Request body</span></span>
<span data-ttu-id="1e8ae-128">在请求正文中，提供[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="1e8ae-129">下表显示创建[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="1e8ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="1e8ae-130">Property</span></span>|<span data-ttu-id="1e8ae-131">类型</span><span class="sxs-lookup"><span data-stu-id="1e8ae-131">Type</span></span>|<span data-ttu-id="1e8ae-132">说明</span><span class="sxs-lookup"><span data-stu-id="1e8ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e8ae-133">id</span><span class="sxs-lookup"><span data-stu-id="1e8ae-133">id</span></span>|<span data-ttu-id="1e8ae-134">String</span><span class="sxs-lookup"><span data-stu-id="1e8ae-134">String</span></span>|<span data-ttu-id="1e8ae-135">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="1e8ae-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-136">This property is read-only.</span></span>|
|<span data-ttu-id="1e8ae-137">target</span><span class="sxs-lookup"><span data-stu-id="1e8ae-137">target</span></span>|[<span data-ttu-id="1e8ae-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1e8ae-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1e8ae-139">将脚本设定为的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="1e8ae-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="1e8ae-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="1e8ae-140">runRemediationScript</span></span>|<span data-ttu-id="1e8ae-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="1e8ae-141">Boolean</span></span>|<span data-ttu-id="1e8ae-142">确定是只运行检测脚本还是运行两个检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="1e8ae-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="1e8ae-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="1e8ae-143">runSchedule</span></span>|[<span data-ttu-id="1e8ae-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="1e8ae-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="1e8ae-145">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="1e8ae-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="1e8ae-146">响应</span><span class="sxs-lookup"><span data-stu-id="1e8ae-146">Response</span></span>
<span data-ttu-id="1e8ae-147">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e8ae-148">示例</span><span class="sxs-lookup"><span data-stu-id="1e8ae-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e8ae-149">请求</span><span class="sxs-lookup"><span data-stu-id="1e8ae-149">Request</span></span>
<span data-ttu-id="1e8ae-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e8ae-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 526

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
    "interval": 8,
    "useUtc": true,
    "time": "11:58:36.2550000"
  }
}
```

### <a name="response"></a><span data-ttu-id="1e8ae-151">响应</span><span class="sxs-lookup"><span data-stu-id="1e8ae-151">Response</span></span>
<span data-ttu-id="1e8ae-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1e8ae-152">Here is an example of the response.</span></span> <span data-ttu-id="1e8ae-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1e8ae-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1e8ae-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1e8ae-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
    "interval": 8,
    "useUtc": true,
    "time": "11:58:36.2550000"
  }
}
```



