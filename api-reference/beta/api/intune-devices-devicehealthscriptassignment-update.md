---
title: 更新 deviceHealthScriptAssignment
description: 更新 deviceHealthScriptAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93909516b037e7545716156920dfec7a089cebca
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610002"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="fc095-103">更新 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="fc095-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="fc095-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc095-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc095-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc095-107">更新 [deviceHealthScriptAssignment 对象](../resources/intune-devices-devicehealthscriptassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="fc095-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc095-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc095-108">Prerequisites</span></span>
<span data-ttu-id="fc095-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc095-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc095-111">Permission type</span></span>|<span data-ttu-id="fc095-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc095-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc095-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc095-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc095-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc095-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc095-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc095-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc095-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc095-116">Not supported.</span></span>|
|<span data-ttu-id="fc095-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc095-117">Application</span></span>|<span data-ttu-id="fc095-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc095-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc095-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc095-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fc095-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc095-120">Request headers</span></span>
|<span data-ttu-id="fc095-121">标头</span><span class="sxs-lookup"><span data-stu-id="fc095-121">Header</span></span>|<span data-ttu-id="fc095-122">值</span><span class="sxs-lookup"><span data-stu-id="fc095-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc095-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc095-123">Authorization</span></span>|<span data-ttu-id="fc095-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc095-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc095-125">接受</span><span class="sxs-lookup"><span data-stu-id="fc095-125">Accept</span></span>|<span data-ttu-id="fc095-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc095-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc095-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc095-127">Request body</span></span>
<span data-ttu-id="fc095-128">在请求正文中，提供 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc095-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="fc095-129">下表显示创建 [deviceHealthScriptAssignment 时所需的属性](../resources/intune-devices-devicehealthscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="fc095-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="fc095-130">属性</span><span class="sxs-lookup"><span data-stu-id="fc095-130">Property</span></span>|<span data-ttu-id="fc095-131">类型</span><span class="sxs-lookup"><span data-stu-id="fc095-131">Type</span></span>|<span data-ttu-id="fc095-132">说明</span><span class="sxs-lookup"><span data-stu-id="fc095-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc095-133">id</span><span class="sxs-lookup"><span data-stu-id="fc095-133">id</span></span>|<span data-ttu-id="fc095-134">String</span><span class="sxs-lookup"><span data-stu-id="fc095-134">String</span></span>|<span data-ttu-id="fc095-135">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc095-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="fc095-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fc095-136">This property is read-only.</span></span>|
|<span data-ttu-id="fc095-137">target</span><span class="sxs-lookup"><span data-stu-id="fc095-137">target</span></span>|[<span data-ttu-id="fc095-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fc095-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fc095-139">我们将脚本定向到的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="fc095-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="fc095-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="fc095-140">runRemediationScript</span></span>|<span data-ttu-id="fc095-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc095-141">Boolean</span></span>|<span data-ttu-id="fc095-142">确定是仅运行检测脚本还是同时运行检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="fc095-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="fc095-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="fc095-143">runSchedule</span></span>|[<span data-ttu-id="fc095-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="fc095-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="fc095-145">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="fc095-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="fc095-146">响应</span><span class="sxs-lookup"><span data-stu-id="fc095-146">Response</span></span>
<span data-ttu-id="fc095-147">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc095-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc095-148">示例</span><span class="sxs-lookup"><span data-stu-id="fc095-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc095-149">请求</span><span class="sxs-lookup"><span data-stu-id="fc095-149">Request</span></span>
<span data-ttu-id="fc095-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc095-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 590

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
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

### <a name="response"></a><span data-ttu-id="fc095-151">响应</span><span class="sxs-lookup"><span data-stu-id="fc095-151">Response</span></span>
<span data-ttu-id="fc095-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc095-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
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




