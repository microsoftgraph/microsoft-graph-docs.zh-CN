---
title: 创建 deviceHealthScriptAssignment
description: 创建新的 deviceHealthScriptAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8678ca5cc5201599158af71f7be2731a5a96232c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161283"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="89d2e-103">创建 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="89d2e-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="89d2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89d2e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89d2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89d2e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89d2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d2e-107">创建新的 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89d2e-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89d2e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="89d2e-108">Prerequisites</span></span>
<span data-ttu-id="89d2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89d2e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89d2e-111">Permission type</span></span>|<span data-ttu-id="89d2e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89d2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89d2e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89d2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89d2e-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d2e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89d2e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89d2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89d2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89d2e-116">Not supported.</span></span>|
|<span data-ttu-id="89d2e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89d2e-117">Application</span></span>|<span data-ttu-id="89d2e-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d2e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89d2e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89d2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="89d2e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89d2e-120">Request headers</span></span>
|<span data-ttu-id="89d2e-121">标头</span><span class="sxs-lookup"><span data-stu-id="89d2e-121">Header</span></span>|<span data-ttu-id="89d2e-122">值</span><span class="sxs-lookup"><span data-stu-id="89d2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89d2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89d2e-123">Authorization</span></span>|<span data-ttu-id="89d2e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89d2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89d2e-125">接受</span><span class="sxs-lookup"><span data-stu-id="89d2e-125">Accept</span></span>|<span data-ttu-id="89d2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89d2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d2e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89d2e-127">Request body</span></span>
<span data-ttu-id="89d2e-128">在请求正文中，提供 deviceHealthScriptAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d2e-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="89d2e-129">下表显示创建 deviceHealthScriptAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89d2e-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="89d2e-130">属性</span><span class="sxs-lookup"><span data-stu-id="89d2e-130">Property</span></span>|<span data-ttu-id="89d2e-131">类型</span><span class="sxs-lookup"><span data-stu-id="89d2e-131">Type</span></span>|<span data-ttu-id="89d2e-132">说明</span><span class="sxs-lookup"><span data-stu-id="89d2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d2e-133">id</span><span class="sxs-lookup"><span data-stu-id="89d2e-133">id</span></span>|<span data-ttu-id="89d2e-134">String</span><span class="sxs-lookup"><span data-stu-id="89d2e-134">String</span></span>|<span data-ttu-id="89d2e-135">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="89d2e-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="89d2e-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="89d2e-136">This property is read-only.</span></span>|
|<span data-ttu-id="89d2e-137">target</span><span class="sxs-lookup"><span data-stu-id="89d2e-137">target</span></span>|[<span data-ttu-id="89d2e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="89d2e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="89d2e-139">我们将脚本定向到的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="89d2e-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="89d2e-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="89d2e-140">runRemediationScript</span></span>|<span data-ttu-id="89d2e-141">布尔</span><span class="sxs-lookup"><span data-stu-id="89d2e-141">Boolean</span></span>|<span data-ttu-id="89d2e-142">确定是仅运行检测脚本还是同时运行检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="89d2e-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="89d2e-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="89d2e-143">runSchedule</span></span>|[<span data-ttu-id="89d2e-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="89d2e-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="89d2e-145">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="89d2e-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="89d2e-146">响应</span><span class="sxs-lookup"><span data-stu-id="89d2e-146">Response</span></span>
<span data-ttu-id="89d2e-147">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89d2e-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89d2e-148">示例</span><span class="sxs-lookup"><span data-stu-id="89d2e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="89d2e-149">请求</span><span class="sxs-lookup"><span data-stu-id="89d2e-149">Request</span></span>
<span data-ttu-id="89d2e-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89d2e-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="89d2e-151">响应</span><span class="sxs-lookup"><span data-stu-id="89d2e-151">Response</span></span>
<span data-ttu-id="89d2e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89d2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




