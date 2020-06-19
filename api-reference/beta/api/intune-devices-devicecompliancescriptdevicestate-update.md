---
title: 更新 deviceComplianceScriptDeviceState
description: 更新 deviceComplianceScriptDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2506199946b3b80c983c84486cb3b6de4a209494
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792441"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="f5a70-103">更新 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="f5a70-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="f5a70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5a70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5a70-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5a70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5a70-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5a70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5a70-107">更新[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f5a70-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5a70-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5a70-108">Prerequisites</span></span>
<span data-ttu-id="f5a70-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f5a70-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f5a70-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5a70-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5a70-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5a70-111">Permission type</span></span>|<span data-ttu-id="f5a70-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5a70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5a70-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5a70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5a70-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5a70-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f5a70-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5a70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5a70-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5a70-116">Not supported.</span></span>|
|<span data-ttu-id="f5a70-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5a70-117">Application</span></span>|<span data-ttu-id="f5a70-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5a70-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5a70-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5a70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f5a70-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5a70-120">Request headers</span></span>
|<span data-ttu-id="f5a70-121">标头</span><span class="sxs-lookup"><span data-stu-id="f5a70-121">Header</span></span>|<span data-ttu-id="f5a70-122">值</span><span class="sxs-lookup"><span data-stu-id="f5a70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5a70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5a70-123">Authorization</span></span>|<span data-ttu-id="f5a70-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5a70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5a70-125">接受</span><span class="sxs-lookup"><span data-stu-id="f5a70-125">Accept</span></span>|<span data-ttu-id="f5a70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5a70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5a70-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5a70-127">Request body</span></span>
<span data-ttu-id="f5a70-128">在请求正文中，提供[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5a70-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="f5a70-129">下表显示创建[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5a70-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="f5a70-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5a70-130">Property</span></span>|<span data-ttu-id="f5a70-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5a70-131">Type</span></span>|<span data-ttu-id="f5a70-132">说明</span><span class="sxs-lookup"><span data-stu-id="f5a70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5a70-133">id</span><span class="sxs-lookup"><span data-stu-id="f5a70-133">id</span></span>|<span data-ttu-id="f5a70-134">String</span><span class="sxs-lookup"><span data-stu-id="f5a70-134">String</span></span>|<span data-ttu-id="f5a70-135">设备合规性脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5a70-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="f5a70-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f5a70-136">This property is read-only.</span></span>|
|<span data-ttu-id="f5a70-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="f5a70-137">detectionState</span></span>|[<span data-ttu-id="f5a70-138">runState</span><span class="sxs-lookup"><span data-stu-id="f5a70-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f5a70-139">Lastest 设备合规性脚本执行中的检测状态。</span><span class="sxs-lookup"><span data-stu-id="f5a70-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="f5a70-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="f5a70-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="f5a70-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f5a70-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="f5a70-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5a70-142">DateTimeOffset</span></span>|<span data-ttu-id="f5a70-143">执行设备符合性脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="f5a70-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="f5a70-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f5a70-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="f5a70-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5a70-145">DateTimeOffset</span></span>|<span data-ttu-id="f5a70-146">预期何时执行设备符合性脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="f5a70-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="f5a70-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f5a70-147">lastSyncDateTime</span></span>|<span data-ttu-id="f5a70-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5a70-148">DateTimeOffset</span></span>|<span data-ttu-id="f5a70-149">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="f5a70-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="f5a70-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="f5a70-150">scriptOutput</span></span>|<span data-ttu-id="f5a70-151">String</span><span class="sxs-lookup"><span data-stu-id="f5a70-151">String</span></span>|<span data-ttu-id="f5a70-152">检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="f5a70-152">Output of the detection script</span></span>|
|<span data-ttu-id="f5a70-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="f5a70-153">scriptError</span></span>|<span data-ttu-id="f5a70-154">String</span><span class="sxs-lookup"><span data-stu-id="f5a70-154">String</span></span>|<span data-ttu-id="f5a70-155">检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="f5a70-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="f5a70-156">响应</span><span class="sxs-lookup"><span data-stu-id="f5a70-156">Response</span></span>
<span data-ttu-id="f5a70-157">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f5a70-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5a70-158">示例</span><span class="sxs-lookup"><span data-stu-id="f5a70-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5a70-159">请求</span><span class="sxs-lookup"><span data-stu-id="f5a70-159">Request</span></span>
<span data-ttu-id="f5a70-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5a70-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```

### <a name="response"></a><span data-ttu-id="f5a70-161">响应</span><span class="sxs-lookup"><span data-stu-id="f5a70-161">Response</span></span>
<span data-ttu-id="f5a70-162">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f5a70-162">Here is an example of the response.</span></span> <span data-ttu-id="f5a70-163">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f5a70-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f5a70-164">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f5a70-164">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 436

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "7bd39c86-9c86-7bd3-869c-d37b869cd37b",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "scriptOutput": "Script Output value",
  "scriptError": "Script Error value"
}
```



