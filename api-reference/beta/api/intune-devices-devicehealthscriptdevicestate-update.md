---
title: 更新 deviceHealthScriptDeviceState
description: 更新 deviceHealthScriptDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: daa79b87391aeec8265f8f6499e4addf8c3393cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235131"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="df9aa-103">更新 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="df9aa-103">Update deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="df9aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df9aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df9aa-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df9aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df9aa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df9aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df9aa-107">更新 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df9aa-107">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df9aa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df9aa-108">Prerequisites</span></span>
<span data-ttu-id="df9aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df9aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df9aa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df9aa-111">Permission type</span></span>|<span data-ttu-id="df9aa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df9aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df9aa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df9aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df9aa-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df9aa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="df9aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df9aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df9aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df9aa-116">Not supported.</span></span>|
|<span data-ttu-id="df9aa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df9aa-117">Application</span></span>|<span data-ttu-id="df9aa-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="df9aa-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df9aa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df9aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="df9aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df9aa-120">Request headers</span></span>
|<span data-ttu-id="df9aa-121">标头</span><span class="sxs-lookup"><span data-stu-id="df9aa-121">Header</span></span>|<span data-ttu-id="df9aa-122">值</span><span class="sxs-lookup"><span data-stu-id="df9aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df9aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df9aa-123">Authorization</span></span>|<span data-ttu-id="df9aa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df9aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df9aa-125">接受</span><span class="sxs-lookup"><span data-stu-id="df9aa-125">Accept</span></span>|<span data-ttu-id="df9aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df9aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df9aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df9aa-127">Request body</span></span>
<span data-ttu-id="df9aa-128">在请求正文中，提供 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df9aa-128">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="df9aa-129">下表显示创建 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df9aa-129">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="df9aa-130">属性</span><span class="sxs-lookup"><span data-stu-id="df9aa-130">Property</span></span>|<span data-ttu-id="df9aa-131">类型</span><span class="sxs-lookup"><span data-stu-id="df9aa-131">Type</span></span>|<span data-ttu-id="df9aa-132">说明</span><span class="sxs-lookup"><span data-stu-id="df9aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df9aa-133">id</span><span class="sxs-lookup"><span data-stu-id="df9aa-133">id</span></span>|<span data-ttu-id="df9aa-134">String</span><span class="sxs-lookup"><span data-stu-id="df9aa-134">String</span></span>|<span data-ttu-id="df9aa-135">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="df9aa-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="df9aa-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="df9aa-136">This property is read-only.</span></span>|
|<span data-ttu-id="df9aa-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="df9aa-137">detectionState</span></span>|[<span data-ttu-id="df9aa-138">runState</span><span class="sxs-lookup"><span data-stu-id="df9aa-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="df9aa-139">Lastest 设备运行状况脚本执行的检测状态。</span><span class="sxs-lookup"><span data-stu-id="df9aa-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="df9aa-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="df9aa-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="df9aa-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="df9aa-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="df9aa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df9aa-142">DateTimeOffset</span></span>|<span data-ttu-id="df9aa-143">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="df9aa-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="df9aa-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="df9aa-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="df9aa-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df9aa-145">DateTimeOffset</span></span>|<span data-ttu-id="df9aa-146">应在何时执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="df9aa-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="df9aa-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="df9aa-147">lastSyncDateTime</span></span>|<span data-ttu-id="df9aa-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df9aa-148">DateTimeOffset</span></span>|<span data-ttu-id="df9aa-149">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="df9aa-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="df9aa-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="df9aa-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="df9aa-151">String</span><span class="sxs-lookup"><span data-stu-id="df9aa-151">String</span></span>|<span data-ttu-id="df9aa-152">修正前的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="df9aa-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="df9aa-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="df9aa-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="df9aa-154">String</span><span class="sxs-lookup"><span data-stu-id="df9aa-154">String</span></span>|<span data-ttu-id="df9aa-155">修正前的检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="df9aa-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="df9aa-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="df9aa-156">remediationScriptError</span></span>|<span data-ttu-id="df9aa-157">String</span><span class="sxs-lookup"><span data-stu-id="df9aa-157">String</span></span>|<span data-ttu-id="df9aa-158">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="df9aa-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="df9aa-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="df9aa-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="df9aa-160">String</span><span class="sxs-lookup"><span data-stu-id="df9aa-160">String</span></span>|<span data-ttu-id="df9aa-161">修正后的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="df9aa-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="df9aa-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="df9aa-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="df9aa-163">String</span><span class="sxs-lookup"><span data-stu-id="df9aa-163">String</span></span>|<span data-ttu-id="df9aa-164">更正后来自检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="df9aa-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="df9aa-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="df9aa-165">remediationState</span></span>|[<span data-ttu-id="df9aa-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="df9aa-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="df9aa-167">来自 lastest 设备运行状况脚本执行的修正状态。</span><span class="sxs-lookup"><span data-stu-id="df9aa-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="df9aa-168">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="df9aa-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="df9aa-169">响应</span><span class="sxs-lookup"><span data-stu-id="df9aa-169">Response</span></span>
<span data-ttu-id="df9aa-170">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df9aa-170">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df9aa-171">示例</span><span class="sxs-lookup"><span data-stu-id="df9aa-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="df9aa-172">请求</span><span class="sxs-lookup"><span data-stu-id="df9aa-172">Request</span></span>
<span data-ttu-id="df9aa-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df9aa-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
Content-type: application/json
Content-length: 762

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
  "remediationState": "skipped"
}
```

### <a name="response"></a><span data-ttu-id="df9aa-174">响应</span><span class="sxs-lookup"><span data-stu-id="df9aa-174">Response</span></span>
<span data-ttu-id="df9aa-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df9aa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 811

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
  "remediationState": "skipped"
}
```




