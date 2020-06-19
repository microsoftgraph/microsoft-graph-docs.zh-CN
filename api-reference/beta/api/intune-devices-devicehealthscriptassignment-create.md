---
title: 创建 deviceHealthScriptAssignment
description: 创建新的 deviceHealthScriptAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 605b21c3de1a7408224c3544e6f3bbb7d4adf04f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792413"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="d88af-103">创建 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d88af-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="d88af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d88af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d88af-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d88af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d88af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d88af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88af-107">创建新的[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d88af-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d88af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d88af-108">Prerequisites</span></span>
<span data-ttu-id="d88af-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d88af-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d88af-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d88af-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d88af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d88af-111">Permission type</span></span>|<span data-ttu-id="d88af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d88af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d88af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d88af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d88af-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88af-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d88af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d88af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d88af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d88af-116">Not supported.</span></span>|
|<span data-ttu-id="d88af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d88af-117">Application</span></span>|<span data-ttu-id="d88af-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88af-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d88af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d88af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d88af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d88af-120">Request headers</span></span>
|<span data-ttu-id="d88af-121">标头</span><span class="sxs-lookup"><span data-stu-id="d88af-121">Header</span></span>|<span data-ttu-id="d88af-122">值</span><span class="sxs-lookup"><span data-stu-id="d88af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d88af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d88af-123">Authorization</span></span>|<span data-ttu-id="d88af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d88af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d88af-125">接受</span><span class="sxs-lookup"><span data-stu-id="d88af-125">Accept</span></span>|<span data-ttu-id="d88af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d88af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d88af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d88af-127">Request body</span></span>
<span data-ttu-id="d88af-128">在请求正文中，提供 deviceHealthScriptAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d88af-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="d88af-129">下表显示创建 deviceHealthScriptAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d88af-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="d88af-130">属性</span><span class="sxs-lookup"><span data-stu-id="d88af-130">Property</span></span>|<span data-ttu-id="d88af-131">类型</span><span class="sxs-lookup"><span data-stu-id="d88af-131">Type</span></span>|<span data-ttu-id="d88af-132">说明</span><span class="sxs-lookup"><span data-stu-id="d88af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d88af-133">id</span><span class="sxs-lookup"><span data-stu-id="d88af-133">id</span></span>|<span data-ttu-id="d88af-134">String</span><span class="sxs-lookup"><span data-stu-id="d88af-134">String</span></span>|<span data-ttu-id="d88af-135">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="d88af-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="d88af-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d88af-136">This property is read-only.</span></span>|
|<span data-ttu-id="d88af-137">target</span><span class="sxs-lookup"><span data-stu-id="d88af-137">target</span></span>|[<span data-ttu-id="d88af-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d88af-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d88af-139">将脚本设定为的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="d88af-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="d88af-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="d88af-140">runRemediationScript</span></span>|<span data-ttu-id="d88af-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="d88af-141">Boolean</span></span>|<span data-ttu-id="d88af-142">确定是只运行检测脚本还是运行两个检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="d88af-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="d88af-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d88af-143">runSchedule</span></span>|[<span data-ttu-id="d88af-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="d88af-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="d88af-145">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="d88af-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="d88af-146">响应</span><span class="sxs-lookup"><span data-stu-id="d88af-146">Response</span></span>
<span data-ttu-id="d88af-147">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d88af-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d88af-148">示例</span><span class="sxs-lookup"><span data-stu-id="d88af-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d88af-149">请求</span><span class="sxs-lookup"><span data-stu-id="d88af-149">Request</span></span>
<span data-ttu-id="d88af-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d88af-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="d88af-151">响应</span><span class="sxs-lookup"><span data-stu-id="d88af-151">Response</span></span>
<span data-ttu-id="d88af-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d88af-152">Here is an example of the response.</span></span> <span data-ttu-id="d88af-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d88af-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d88af-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d88af-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



