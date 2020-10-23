---
title: 更新 deviceHealthScriptDeviceState
description: 更新 deviceHealthScriptDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5537e1bfa95780545df9e7c53f19c688477f0b78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736525"
---
# <a name="update-devicehealthscriptdevicestate"></a><span data-ttu-id="f1fac-103">更新 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="f1fac-103">Update deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="f1fac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1fac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1fac-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1fac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1fac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1fac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1fac-107">更新 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1fac-107">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1fac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1fac-108">Prerequisites</span></span>
<span data-ttu-id="f1fac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1fac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1fac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1fac-111">Permission type</span></span>|<span data-ttu-id="f1fac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1fac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1fac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1fac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1fac-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1fac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f1fac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1fac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1fac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1fac-116">Not supported.</span></span>|
|<span data-ttu-id="f1fac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1fac-117">Application</span></span>|<span data-ttu-id="f1fac-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1fac-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1fac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1fac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f1fac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1fac-120">Request headers</span></span>
|<span data-ttu-id="f1fac-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1fac-121">Header</span></span>|<span data-ttu-id="f1fac-122">值</span><span class="sxs-lookup"><span data-stu-id="f1fac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1fac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1fac-123">Authorization</span></span>|<span data-ttu-id="f1fac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1fac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1fac-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1fac-125">Accept</span></span>|<span data-ttu-id="f1fac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1fac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1fac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1fac-127">Request body</span></span>
<span data-ttu-id="f1fac-128">在请求正文中，提供 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1fac-128">In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

<span data-ttu-id="f1fac-129">下表显示创建 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1fac-129">The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>

|<span data-ttu-id="f1fac-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1fac-130">Property</span></span>|<span data-ttu-id="f1fac-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1fac-131">Type</span></span>|<span data-ttu-id="f1fac-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1fac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1fac-133">id</span><span class="sxs-lookup"><span data-stu-id="f1fac-133">id</span></span>|<span data-ttu-id="f1fac-134">String</span><span class="sxs-lookup"><span data-stu-id="f1fac-134">String</span></span>|<span data-ttu-id="f1fac-135">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1fac-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="f1fac-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1fac-136">This property is read-only.</span></span>|
|<span data-ttu-id="f1fac-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="f1fac-137">detectionState</span></span>|[<span data-ttu-id="f1fac-138">runState</span><span class="sxs-lookup"><span data-stu-id="f1fac-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f1fac-139">Lastest 设备运行状况脚本执行的检测状态。</span><span class="sxs-lookup"><span data-stu-id="f1fac-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="f1fac-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="f1fac-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="f1fac-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f1fac-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="f1fac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1fac-142">DateTimeOffset</span></span>|<span data-ttu-id="f1fac-143">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="f1fac-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="f1fac-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f1fac-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="f1fac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1fac-145">DateTimeOffset</span></span>|<span data-ttu-id="f1fac-146">应在何时执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="f1fac-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="f1fac-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f1fac-147">lastSyncDateTime</span></span>|<span data-ttu-id="f1fac-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1fac-148">DateTimeOffset</span></span>|<span data-ttu-id="f1fac-149">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="f1fac-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="f1fac-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="f1fac-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="f1fac-151">String</span><span class="sxs-lookup"><span data-stu-id="f1fac-151">String</span></span>|<span data-ttu-id="f1fac-152">修正前的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="f1fac-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="f1fac-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="f1fac-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="f1fac-154">String</span><span class="sxs-lookup"><span data-stu-id="f1fac-154">String</span></span>|<span data-ttu-id="f1fac-155">修正前的检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="f1fac-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="f1fac-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="f1fac-156">remediationScriptError</span></span>|<span data-ttu-id="f1fac-157">String</span><span class="sxs-lookup"><span data-stu-id="f1fac-157">String</span></span>|<span data-ttu-id="f1fac-158">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="f1fac-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="f1fac-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="f1fac-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="f1fac-160">String</span><span class="sxs-lookup"><span data-stu-id="f1fac-160">String</span></span>|<span data-ttu-id="f1fac-161">修正后的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="f1fac-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="f1fac-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="f1fac-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="f1fac-163">String</span><span class="sxs-lookup"><span data-stu-id="f1fac-163">String</span></span>|<span data-ttu-id="f1fac-164">更正后来自检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="f1fac-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="f1fac-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="f1fac-165">remediationState</span></span>|[<span data-ttu-id="f1fac-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="f1fac-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="f1fac-167">来自 lastest 设备运行状况脚本执行的修正状态。</span><span class="sxs-lookup"><span data-stu-id="f1fac-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="f1fac-168">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="f1fac-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="f1fac-169">响应</span><span class="sxs-lookup"><span data-stu-id="f1fac-169">Response</span></span>
<span data-ttu-id="f1fac-170">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1fac-170">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1fac-171">示例</span><span class="sxs-lookup"><span data-stu-id="f1fac-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1fac-172">请求</span><span class="sxs-lookup"><span data-stu-id="f1fac-172">Request</span></span>
<span data-ttu-id="f1fac-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1fac-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1fac-174">响应</span><span class="sxs-lookup"><span data-stu-id="f1fac-174">Response</span></span>
<span data-ttu-id="f1fac-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1fac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





