---
title: 创建 deviceManagementScriptDeviceState
description: 创建新的 deviceManagementScriptDeviceState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f613c6bb7d8a9fa25a9ef6007701433a1c2f799
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188561"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="ca994-103">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="ca994-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="ca994-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca994-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca994-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca994-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca994-106">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca994-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca994-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca994-107">Prerequisites</span></span>
<span data-ttu-id="ca994-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca994-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca994-110">Permission type</span></span>|<span data-ttu-id="ca994-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca994-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca994-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca994-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca994-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca994-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ca994-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca994-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca994-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca994-115">Not supported.</span></span>|
|<span data-ttu-id="ca994-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca994-116">Application</span></span>|<span data-ttu-id="ca994-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca994-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca994-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca994-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="ca994-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca994-119">Request headers</span></span>
|<span data-ttu-id="ca994-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca994-120">Header</span></span>|<span data-ttu-id="ca994-121">值</span><span class="sxs-lookup"><span data-stu-id="ca994-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca994-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca994-122">Authorization</span></span>|<span data-ttu-id="ca994-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca994-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca994-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca994-124">Accept</span></span>|<span data-ttu-id="ca994-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca994-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca994-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca994-126">Request body</span></span>
<span data-ttu-id="ca994-127">在请求正文中，提供 deviceManagementScriptDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca994-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="ca994-128">下表显示创建 deviceManagementScriptDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca994-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="ca994-129">属性</span><span class="sxs-lookup"><span data-stu-id="ca994-129">Property</span></span>|<span data-ttu-id="ca994-130">类型</span><span class="sxs-lookup"><span data-stu-id="ca994-130">Type</span></span>|<span data-ttu-id="ca994-131">说明</span><span class="sxs-lookup"><span data-stu-id="ca994-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca994-132">id</span><span class="sxs-lookup"><span data-stu-id="ca994-132">id</span></span>|<span data-ttu-id="ca994-133">String</span><span class="sxs-lookup"><span data-stu-id="ca994-133">String</span></span>|<span data-ttu-id="ca994-134">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="ca994-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="ca994-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ca994-135">This property is read-only.</span></span>|
|<span data-ttu-id="ca994-136">runState</span><span class="sxs-lookup"><span data-stu-id="ca994-136">runState</span></span>|[<span data-ttu-id="ca994-137">runState</span><span class="sxs-lookup"><span data-stu-id="ca994-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="ca994-138">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="ca994-138">State of latest run of the device management script.</span></span> <span data-ttu-id="ca994-139">可取值为：`unknown`、`success`、`fail`、`error`、`pending`。</span><span class="sxs-lookup"><span data-stu-id="ca994-139">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="ca994-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="ca994-140">resultMessage</span></span>|<span data-ttu-id="ca994-141">String</span><span class="sxs-lookup"><span data-stu-id="ca994-141">String</span></span>|<span data-ttu-id="ca994-142">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ca994-142">Details of execution output.</span></span>|
|<span data-ttu-id="ca994-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ca994-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="ca994-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca994-144">DateTimeOffset</span></span>|<span data-ttu-id="ca994-145">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="ca994-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="ca994-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="ca994-146">errorCode</span></span>|<span data-ttu-id="ca994-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ca994-147">Int32</span></span>|<span data-ttu-id="ca994-148">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ca994-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="ca994-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="ca994-149">errorDescription</span></span>|<span data-ttu-id="ca994-150">String</span><span class="sxs-lookup"><span data-stu-id="ca994-150">String</span></span>|<span data-ttu-id="ca994-151">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="ca994-151">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="ca994-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ca994-152">lastSyncDateTime</span></span>|<span data-ttu-id="ca994-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca994-153">DateTimeOffset</span></span>|<span data-ttu-id="ca994-154">Intune 管理扩展将同步到 Intune 的最新时间。</span><span class="sxs-lookup"><span data-stu-id="ca994-154">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="ca994-155">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="ca994-155">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="ca994-156">String</span><span class="sxs-lookup"><span data-stu-id="ca994-156">String</span></span>|<span data-ttu-id="ca994-157">修复前的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="ca994-157">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="ca994-158">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="ca994-158">remediationScriptError</span></span>|<span data-ttu-id="ca994-159">String</span><span class="sxs-lookup"><span data-stu-id="ca994-159">String</span></span>|<span data-ttu-id="ca994-160">修正脚本的错误输出。</span><span class="sxs-lookup"><span data-stu-id="ca994-160">Error output of the remediation script.</span></span>|
|<span data-ttu-id="ca994-161">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="ca994-161">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="ca994-162">String</span><span class="sxs-lookup"><span data-stu-id="ca994-162">String</span></span>|<span data-ttu-id="ca994-163">修正后的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="ca994-163">Detection script output after remediation.</span></span>|



## <a name="response"></a><span data-ttu-id="ca994-164">响应</span><span class="sxs-lookup"><span data-stu-id="ca994-164">Response</span></span>
<span data-ttu-id="ca994-165">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca994-165">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca994-166">示例</span><span class="sxs-lookup"><span data-stu-id="ca994-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca994-167">请求</span><span class="sxs-lookup"><span data-stu-id="ca994-167">Request</span></span>
<span data-ttu-id="ca994-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca994-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="ca994-169">响应</span><span class="sxs-lookup"><span data-stu-id="ca994-169">Response</span></span>
<span data-ttu-id="ca994-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca994-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




