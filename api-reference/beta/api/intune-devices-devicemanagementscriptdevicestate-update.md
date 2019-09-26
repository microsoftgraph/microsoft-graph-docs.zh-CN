---
title: 更新 deviceManagementScriptDeviceState
description: 更新 deviceManagementScriptDeviceState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bfb1dc79bd1162b2b05ddff35c3ea712db3ea97
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188554"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="47627-103">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="47627-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="47627-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47627-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47627-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47627-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47627-106">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47627-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47627-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="47627-107">Prerequisites</span></span>
<span data-ttu-id="47627-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47627-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="47627-110">Permission type</span></span>|<span data-ttu-id="47627-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="47627-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47627-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47627-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47627-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47627-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="47627-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47627-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47627-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="47627-115">Not supported.</span></span>|
|<span data-ttu-id="47627-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="47627-116">Application</span></span>|<span data-ttu-id="47627-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47627-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47627-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47627-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="47627-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="47627-119">Request headers</span></span>
|<span data-ttu-id="47627-120">标头</span><span class="sxs-lookup"><span data-stu-id="47627-120">Header</span></span>|<span data-ttu-id="47627-121">值</span><span class="sxs-lookup"><span data-stu-id="47627-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47627-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47627-122">Authorization</span></span>|<span data-ttu-id="47627-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47627-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47627-124">接受</span><span class="sxs-lookup"><span data-stu-id="47627-124">Accept</span></span>|<span data-ttu-id="47627-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47627-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47627-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="47627-126">Request body</span></span>
<span data-ttu-id="47627-127">在请求正文中，提供[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47627-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="47627-128">下表显示创建[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="47627-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="47627-129">属性</span><span class="sxs-lookup"><span data-stu-id="47627-129">Property</span></span>|<span data-ttu-id="47627-130">类型</span><span class="sxs-lookup"><span data-stu-id="47627-130">Type</span></span>|<span data-ttu-id="47627-131">说明</span><span class="sxs-lookup"><span data-stu-id="47627-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47627-132">id</span><span class="sxs-lookup"><span data-stu-id="47627-132">id</span></span>|<span data-ttu-id="47627-133">String</span><span class="sxs-lookup"><span data-stu-id="47627-133">String</span></span>|<span data-ttu-id="47627-134">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="47627-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="47627-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="47627-135">This property is read-only.</span></span>|
|<span data-ttu-id="47627-136">runState</span><span class="sxs-lookup"><span data-stu-id="47627-136">runState</span></span>|[<span data-ttu-id="47627-137">runState</span><span class="sxs-lookup"><span data-stu-id="47627-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="47627-138">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="47627-138">State of latest run of the device management script.</span></span> <span data-ttu-id="47627-139">可取值为：`unknown`、`success`、`fail`、`error`、`pending`。</span><span class="sxs-lookup"><span data-stu-id="47627-139">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="47627-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="47627-140">resultMessage</span></span>|<span data-ttu-id="47627-141">String</span><span class="sxs-lookup"><span data-stu-id="47627-141">String</span></span>|<span data-ttu-id="47627-142">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="47627-142">Details of execution output.</span></span>|
|<span data-ttu-id="47627-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="47627-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="47627-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47627-144">DateTimeOffset</span></span>|<span data-ttu-id="47627-145">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="47627-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="47627-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="47627-146">errorCode</span></span>|<span data-ttu-id="47627-147">Int32</span><span class="sxs-lookup"><span data-stu-id="47627-147">Int32</span></span>|<span data-ttu-id="47627-148">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="47627-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="47627-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="47627-149">errorDescription</span></span>|<span data-ttu-id="47627-150">String</span><span class="sxs-lookup"><span data-stu-id="47627-150">String</span></span>|<span data-ttu-id="47627-151">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="47627-151">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="47627-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="47627-152">lastSyncDateTime</span></span>|<span data-ttu-id="47627-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47627-153">DateTimeOffset</span></span>|<span data-ttu-id="47627-154">Intune 管理扩展将同步到 Intune 的最新时间。</span><span class="sxs-lookup"><span data-stu-id="47627-154">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="47627-155">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="47627-155">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="47627-156">String</span><span class="sxs-lookup"><span data-stu-id="47627-156">String</span></span>|<span data-ttu-id="47627-157">修复前的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="47627-157">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="47627-158">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="47627-158">remediationScriptError</span></span>|<span data-ttu-id="47627-159">String</span><span class="sxs-lookup"><span data-stu-id="47627-159">String</span></span>|<span data-ttu-id="47627-160">修正脚本的错误输出。</span><span class="sxs-lookup"><span data-stu-id="47627-160">Error output of the remediation script.</span></span>|
|<span data-ttu-id="47627-161">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="47627-161">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="47627-162">String</span><span class="sxs-lookup"><span data-stu-id="47627-162">String</span></span>|<span data-ttu-id="47627-163">修正后的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="47627-163">Detection script output after remediation.</span></span>|



## <a name="response"></a><span data-ttu-id="47627-164">响应</span><span class="sxs-lookup"><span data-stu-id="47627-164">Response</span></span>
<span data-ttu-id="47627-165">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47627-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47627-166">示例</span><span class="sxs-lookup"><span data-stu-id="47627-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="47627-167">请求</span><span class="sxs-lookup"><span data-stu-id="47627-167">Request</span></span>
<span data-ttu-id="47627-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47627-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
}
```

### <a name="response"></a><span data-ttu-id="47627-169">响应</span><span class="sxs-lookup"><span data-stu-id="47627-169">Response</span></span>
<span data-ttu-id="47627-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47627-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
}
```




