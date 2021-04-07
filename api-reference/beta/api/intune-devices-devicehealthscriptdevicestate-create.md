---
title: 创建 deviceHealthScriptDeviceState
description: 创建新的 deviceHealthScriptDeviceState 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e82e2fd9821f05cfb0690367fce3de03b02cd7c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51609764"
---
# <a name="create-devicehealthscriptdevicestate"></a><span data-ttu-id="60b6e-103">创建 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="60b6e-103">Create deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="60b6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60b6e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60b6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60b6e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60b6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60b6e-107">创建新的 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60b6e-107">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60b6e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60b6e-108">Prerequisites</span></span>
<span data-ttu-id="60b6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60b6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b6e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60b6e-111">Permission type</span></span>|<span data-ttu-id="60b6e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60b6e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60b6e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60b6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60b6e-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b6e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60b6e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60b6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60b6e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60b6e-116">Not supported.</span></span>|
|<span data-ttu-id="60b6e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60b6e-117">Application</span></span>|<span data-ttu-id="60b6e-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b6e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b6e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60b6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="60b6e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60b6e-120">Request headers</span></span>
|<span data-ttu-id="60b6e-121">标头</span><span class="sxs-lookup"><span data-stu-id="60b6e-121">Header</span></span>|<span data-ttu-id="60b6e-122">值</span><span class="sxs-lookup"><span data-stu-id="60b6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60b6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b6e-123">Authorization</span></span>|<span data-ttu-id="60b6e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60b6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60b6e-125">接受</span><span class="sxs-lookup"><span data-stu-id="60b6e-125">Accept</span></span>|<span data-ttu-id="60b6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60b6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b6e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60b6e-127">Request body</span></span>
<span data-ttu-id="60b6e-128">在请求正文中，提供 deviceHealthScriptDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60b6e-128">In the request body, supply a JSON representation for the deviceHealthScriptDeviceState object.</span></span>

<span data-ttu-id="60b6e-129">下表显示创建 deviceHealthScriptDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60b6e-129">The following table shows the properties that are required when you create the deviceHealthScriptDeviceState.</span></span>

|<span data-ttu-id="60b6e-130">属性</span><span class="sxs-lookup"><span data-stu-id="60b6e-130">Property</span></span>|<span data-ttu-id="60b6e-131">类型</span><span class="sxs-lookup"><span data-stu-id="60b6e-131">Type</span></span>|<span data-ttu-id="60b6e-132">说明</span><span class="sxs-lookup"><span data-stu-id="60b6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60b6e-133">id</span><span class="sxs-lookup"><span data-stu-id="60b6e-133">id</span></span>|<span data-ttu-id="60b6e-134">String</span><span class="sxs-lookup"><span data-stu-id="60b6e-134">String</span></span>|<span data-ttu-id="60b6e-135">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="60b6e-135">Key of the device health script device state entity.</span></span> <span data-ttu-id="60b6e-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="60b6e-136">This property is read-only.</span></span>|
|<span data-ttu-id="60b6e-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="60b6e-137">detectionState</span></span>|[<span data-ttu-id="60b6e-138">runState</span><span class="sxs-lookup"><span data-stu-id="60b6e-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="60b6e-139">最近一次执行设备运行状况脚本的检测状态。</span><span class="sxs-lookup"><span data-stu-id="60b6e-139">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="60b6e-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="60b6e-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="60b6e-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="60b6e-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="60b6e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b6e-142">DateTimeOffset</span></span>|<span data-ttu-id="60b6e-143">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="60b6e-143">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="60b6e-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="60b6e-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="60b6e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b6e-145">DateTimeOffset</span></span>|<span data-ttu-id="60b6e-146">预计执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="60b6e-146">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="60b6e-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="60b6e-147">lastSyncDateTime</span></span>|<span data-ttu-id="60b6e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b6e-148">DateTimeOffset</span></span>|<span data-ttu-id="60b6e-149">Intune 管理扩展上次与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="60b6e-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="60b6e-150">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="60b6e-150">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="60b6e-151">String</span><span class="sxs-lookup"><span data-stu-id="60b6e-151">String</span></span>|<span data-ttu-id="60b6e-152">修正前检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="60b6e-152">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="60b6e-153">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="60b6e-153">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="60b6e-154">String</span><span class="sxs-lookup"><span data-stu-id="60b6e-154">String</span></span>|<span data-ttu-id="60b6e-155">修正前检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="60b6e-155">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="60b6e-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="60b6e-156">remediationScriptError</span></span>|<span data-ttu-id="60b6e-157">String</span><span class="sxs-lookup"><span data-stu-id="60b6e-157">String</span></span>|<span data-ttu-id="60b6e-158">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="60b6e-158">Error output of the remediation script</span></span>|
|<span data-ttu-id="60b6e-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="60b6e-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="60b6e-160">String</span><span class="sxs-lookup"><span data-stu-id="60b6e-160">String</span></span>|<span data-ttu-id="60b6e-161">修正后检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="60b6e-161">Detection script output after remediation</span></span>|
|<span data-ttu-id="60b6e-162">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="60b6e-162">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="60b6e-163">String</span><span class="sxs-lookup"><span data-stu-id="60b6e-163">String</span></span>|<span data-ttu-id="60b6e-164">修正后检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="60b6e-164">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="60b6e-165">remediationState</span><span class="sxs-lookup"><span data-stu-id="60b6e-165">remediationState</span></span>|[<span data-ttu-id="60b6e-166">remediationState</span><span class="sxs-lookup"><span data-stu-id="60b6e-166">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="60b6e-167">自上次设备运行状况脚本执行以来的修正状态。</span><span class="sxs-lookup"><span data-stu-id="60b6e-167">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="60b6e-168">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="60b6e-168">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|



## <a name="response"></a><span data-ttu-id="60b6e-169">响应</span><span class="sxs-lookup"><span data-stu-id="60b6e-169">Response</span></span>
<span data-ttu-id="60b6e-170">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60b6e-170">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b6e-171">示例</span><span class="sxs-lookup"><span data-stu-id="60b6e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="60b6e-172">请求</span><span class="sxs-lookup"><span data-stu-id="60b6e-172">Request</span></span>
<span data-ttu-id="60b6e-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60b6e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60b6e-174">响应</span><span class="sxs-lookup"><span data-stu-id="60b6e-174">Response</span></span>
<span data-ttu-id="60b6e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60b6e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




