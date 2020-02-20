---
title: 创建 deviceHealthScriptDeviceState
description: 创建新的 deviceHealthScriptDeviceState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 13924843321c3eced7a05022177b2f07edf27d23
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162139"
---
# <a name="create-devicehealthscriptdevicestate"></a><span data-ttu-id="4e8e8-103">创建 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4e8e8-103">Create deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="4e8e8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e8e8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e8e8-106">创建新的[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-106">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e8e8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4e8e8-107">Prerequisites</span></span>
<span data-ttu-id="4e8e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e8e8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e8e8-110">Permission type</span></span>|<span data-ttu-id="4e8e8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4e8e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e8e8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e8e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e8e8-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e8e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e8e8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e8e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e8e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-115">Not supported.</span></span>|
|<span data-ttu-id="4e8e8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e8e8-116">Application</span></span>|<span data-ttu-id="4e8e8-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e8e8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e8e8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e8e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="4e8e8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e8e8-119">Request headers</span></span>
|<span data-ttu-id="4e8e8-120">标头</span><span class="sxs-lookup"><span data-stu-id="4e8e8-120">Header</span></span>|<span data-ttu-id="4e8e8-121">值</span><span class="sxs-lookup"><span data-stu-id="4e8e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e8e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e8e8-122">Authorization</span></span>|<span data-ttu-id="4e8e8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e8e8-124">接受</span><span class="sxs-lookup"><span data-stu-id="4e8e8-124">Accept</span></span>|<span data-ttu-id="4e8e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e8e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e8e8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e8e8-126">Request body</span></span>
<span data-ttu-id="4e8e8-127">在请求正文中，提供 deviceHealthScriptDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-127">In the request body, supply a JSON representation for the deviceHealthScriptDeviceState object.</span></span>

<span data-ttu-id="4e8e8-128">下表显示创建 deviceHealthScriptDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-128">The following table shows the properties that are required when you create the deviceHealthScriptDeviceState.</span></span>

|<span data-ttu-id="4e8e8-129">属性</span><span class="sxs-lookup"><span data-stu-id="4e8e8-129">Property</span></span>|<span data-ttu-id="4e8e8-130">类型</span><span class="sxs-lookup"><span data-stu-id="4e8e8-130">Type</span></span>|<span data-ttu-id="4e8e8-131">说明</span><span class="sxs-lookup"><span data-stu-id="4e8e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e8e8-132">id</span><span class="sxs-lookup"><span data-stu-id="4e8e8-132">id</span></span>|<span data-ttu-id="4e8e8-133">String</span><span class="sxs-lookup"><span data-stu-id="4e8e8-133">String</span></span>|<span data-ttu-id="4e8e8-134">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-134">Key of the device health script device state entity.</span></span> <span data-ttu-id="4e8e8-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-135">This property is read-only.</span></span>|
|<span data-ttu-id="4e8e8-136">detectionState</span><span class="sxs-lookup"><span data-stu-id="4e8e8-136">detectionState</span></span>|[<span data-ttu-id="4e8e8-137">runState</span><span class="sxs-lookup"><span data-stu-id="4e8e8-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4e8e8-138">Lastest 设备运行状况脚本执行的检测状态。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-138">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="4e8e8-139">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="4e8e8-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8e8-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="4e8e8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8e8-141">DateTimeOffset</span></span>|<span data-ttu-id="4e8e8-142">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="4e8e8-142">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="4e8e8-143">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8e8-143">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="4e8e8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8e8-144">DateTimeOffset</span></span>|<span data-ttu-id="4e8e8-145">应在何时执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="4e8e8-145">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="4e8e8-146">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8e8-146">lastSyncDateTime</span></span>|<span data-ttu-id="4e8e8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8e8-147">DateTimeOffset</span></span>|<span data-ttu-id="4e8e8-148">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="4e8e8-148">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="4e8e8-149">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="4e8e8-149">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="4e8e8-150">String</span><span class="sxs-lookup"><span data-stu-id="4e8e8-150">String</span></span>|<span data-ttu-id="4e8e8-151">修正前的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="4e8e8-151">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="4e8e8-152">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="4e8e8-152">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="4e8e8-153">String</span><span class="sxs-lookup"><span data-stu-id="4e8e8-153">String</span></span>|<span data-ttu-id="4e8e8-154">修正前的检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="4e8e8-154">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="4e8e8-155">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="4e8e8-155">remediationScriptError</span></span>|<span data-ttu-id="4e8e8-156">String</span><span class="sxs-lookup"><span data-stu-id="4e8e8-156">String</span></span>|<span data-ttu-id="4e8e8-157">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="4e8e8-157">Error output of the remediation script</span></span>|
|<span data-ttu-id="4e8e8-158">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="4e8e8-158">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="4e8e8-159">String</span><span class="sxs-lookup"><span data-stu-id="4e8e8-159">String</span></span>|<span data-ttu-id="4e8e8-160">修正后的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="4e8e8-160">Detection script output after remediation</span></span>|
|<span data-ttu-id="4e8e8-161">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="4e8e8-161">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="4e8e8-162">String</span><span class="sxs-lookup"><span data-stu-id="4e8e8-162">String</span></span>|<span data-ttu-id="4e8e8-163">更正后来自检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="4e8e8-163">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="4e8e8-164">remediationState</span><span class="sxs-lookup"><span data-stu-id="4e8e8-164">remediationState</span></span>|[<span data-ttu-id="4e8e8-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="4e8e8-165">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="4e8e8-166">来自 lastest 设备运行状况脚本执行的修正状态。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-166">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="4e8e8-167">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-167">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="4e8e8-168">响应</span><span class="sxs-lookup"><span data-stu-id="4e8e8-168">Response</span></span>
<span data-ttu-id="4e8e8-169">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-169">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e8e8-170">示例</span><span class="sxs-lookup"><span data-stu-id="4e8e8-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e8e8-171">请求</span><span class="sxs-lookup"><span data-stu-id="4e8e8-171">Request</span></span>
<span data-ttu-id="4e8e8-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="4e8e8-173">响应</span><span class="sxs-lookup"><span data-stu-id="4e8e8-173">Response</span></span>
<span data-ttu-id="4e8e8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e8e8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





