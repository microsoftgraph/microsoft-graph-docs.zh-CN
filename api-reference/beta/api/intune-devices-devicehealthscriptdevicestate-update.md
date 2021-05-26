---
title: 更新 deviceHealthScriptDeviceState
description: 更新 deviceHealthScriptDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9185740611f90b5a58a789d1ce1bcce888928fb0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665096"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="9f58f-103">更新 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="9f58f-103">Update deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="9f58f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f58f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f58f-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f58f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f58f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f58f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f58f-107">更新 [deviceHealthScriptDeviceState 对象](../resources/intune-devices-devicehealthscriptdevicestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9f58f-107">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f58f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f58f-108">Prerequisites</span></span>
<span data-ttu-id="9f58f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f58f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f58f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f58f-111">Permission type</span></span>|<span data-ttu-id="9f58f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f58f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f58f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f58f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f58f-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f58f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f58f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f58f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f58f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f58f-116">Not supported.</span></span>|
|<span data-ttu-id="9f58f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f58f-117">Application</span></span>|<span data-ttu-id="9f58f-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f58f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f58f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f58f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9f58f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f58f-120">Request headers</span></span>
|<span data-ttu-id="9f58f-121">标头</span><span class="sxs-lookup"><span data-stu-id="9f58f-121">Header</span></span>|<span data-ttu-id="9f58f-122">值</span><span class="sxs-lookup"><span data-stu-id="9f58f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f58f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f58f-123">Authorization</span></span>|<span data-ttu-id="9f58f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f58f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f58f-125">接受</span><span class="sxs-lookup"><span data-stu-id="9f58f-125">Accept</span></span>|<span data-ttu-id="9f58f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f58f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f58f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f58f-127">Request body</span></span>
<span data-ttu-id="9f58f-128">在请求正文中，提供 [deviceHealthScriptDeviceState 对象的](../resources/intune-devices-devicehealthscriptdevicestate.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f58f-128">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="9f58f-129">下表显示创建 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f58f-129">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="9f58f-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f58f-130">Property</span></span>|<span data-ttu-id="9f58f-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f58f-131">Type</span></span>|<span data-ttu-id="9f58f-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f58f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f58f-133">id</span><span class="sxs-lookup"><span data-stu-id="9f58f-133">id</span></span>|<span data-ttu-id="9f58f-134">String</span><span class="sxs-lookup"><span data-stu-id="9f58f-134">String</span></span>|<span data-ttu-id="9f58f-135">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f58f-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="9f58f-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9f58f-136">This property is read-only.</span></span>|
|<span data-ttu-id="9f58f-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="9f58f-137">detectionState</span></span>|[<span data-ttu-id="9f58f-138">runState</span><span class="sxs-lookup"><span data-stu-id="9f58f-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="9f58f-139">最近一次执行设备运行状况脚本的检测状态。</span><span class="sxs-lookup"><span data-stu-id="9f58f-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="9f58f-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="9f58f-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="9f58f-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9f58f-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="9f58f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f58f-142">DateTimeOffset</span></span>|<span data-ttu-id="9f58f-143">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="9f58f-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="9f58f-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9f58f-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="9f58f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f58f-145">DateTimeOffset</span></span>|<span data-ttu-id="9f58f-146">预计执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="9f58f-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="9f58f-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9f58f-147">lastSyncDateTime</span></span>|<span data-ttu-id="9f58f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f58f-148">DateTimeOffset</span></span>|<span data-ttu-id="9f58f-149">Intune 管理扩展上次与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="9f58f-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="9f58f-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="9f58f-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="9f58f-151">String</span><span class="sxs-lookup"><span data-stu-id="9f58f-151">String</span></span>|<span data-ttu-id="9f58f-152">修正前检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="9f58f-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="9f58f-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="9f58f-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="9f58f-154">String</span><span class="sxs-lookup"><span data-stu-id="9f58f-154">String</span></span>|<span data-ttu-id="9f58f-155">修正前检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="9f58f-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="9f58f-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="9f58f-156">remediationScriptError</span></span>|<span data-ttu-id="9f58f-157">String</span><span class="sxs-lookup"><span data-stu-id="9f58f-157">String</span></span>|<span data-ttu-id="9f58f-158">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="9f58f-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="9f58f-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="9f58f-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="9f58f-160">String</span><span class="sxs-lookup"><span data-stu-id="9f58f-160">String</span></span>|<span data-ttu-id="9f58f-161">修正后检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="9f58f-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="9f58f-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="9f58f-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="9f58f-163">String</span><span class="sxs-lookup"><span data-stu-id="9f58f-163">String</span></span>|<span data-ttu-id="9f58f-164">修正后检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="9f58f-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="9f58f-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="9f58f-165">remediationState</span></span>|[<span data-ttu-id="9f58f-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="9f58f-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="9f58f-167">自上次设备运行状况脚本执行以来的修正状态。</span><span class="sxs-lookup"><span data-stu-id="9f58f-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="9f58f-168">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="9f58f-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|
|<span data-ttu-id="9f58f-169">assignmentFilterIds</span><span class="sxs-lookup"><span data-stu-id="9f58f-169">assignmentFilterIds</span></span>|<span data-ttu-id="9f58f-170">String collection</span><span class="sxs-lookup"><span data-stu-id="9f58f-170">String collection</span></span>|<span data-ttu-id="9f58f-171">用于运行状况脚本适用性评估的分配筛选器 ID 的列表</span><span class="sxs-lookup"><span data-stu-id="9f58f-171">A list of the assignment filter ids used for health script applicability evaluation</span></span>|



## <a name="response"></a><span data-ttu-id="9f58f-172">响应</span><span class="sxs-lookup"><span data-stu-id="9f58f-172">Response</span></span>
<span data-ttu-id="9f58f-173">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f58f-173">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f58f-174">示例</span><span class="sxs-lookup"><span data-stu-id="9f58f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f58f-175">请求</span><span class="sxs-lookup"><span data-stu-id="9f58f-175">Request</span></span>
<span data-ttu-id="9f58f-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f58f-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped",
  "assignmentFilterIds": [
    "Assignment Filter Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9f58f-177">响应</span><span class="sxs-lookup"><span data-stu-id="9f58f-177">Response</span></span>
<span data-ttu-id="9f58f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f58f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped",
  "assignmentFilterIds": [
    "Assignment Filter Ids value"
  ]
}
```




