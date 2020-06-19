---
title: 创建 deviceComplianceScriptDeviceState
description: 创建新的 deviceComplianceScriptDeviceState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51da464896ff0a9acdcb395deb04f5117ef02db8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792469"
---
# <a name="create-devicecompliancescriptdevicestate"></a><span data-ttu-id="e98c3-103">创建 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="e98c3-103">Create deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="e98c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e98c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e98c3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e98c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e98c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e98c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e98c3-107">创建新的[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e98c3-107">Create a new [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e98c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e98c3-108">Prerequisites</span></span>
<span data-ttu-id="e98c3-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e98c3-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e98c3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e98c3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e98c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e98c3-111">Permission type</span></span>|<span data-ttu-id="e98c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e98c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e98c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e98c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e98c3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e98c3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e98c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e98c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e98c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e98c3-116">Not supported.</span></span>|
|<span data-ttu-id="e98c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e98c3-117">Application</span></span>|<span data-ttu-id="e98c3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e98c3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e98c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e98c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="e98c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e98c3-120">Request headers</span></span>
|<span data-ttu-id="e98c3-121">标头</span><span class="sxs-lookup"><span data-stu-id="e98c3-121">Header</span></span>|<span data-ttu-id="e98c3-122">值</span><span class="sxs-lookup"><span data-stu-id="e98c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e98c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e98c3-123">Authorization</span></span>|<span data-ttu-id="e98c3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e98c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e98c3-125">接受</span><span class="sxs-lookup"><span data-stu-id="e98c3-125">Accept</span></span>|<span data-ttu-id="e98c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e98c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e98c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e98c3-127">Request body</span></span>
<span data-ttu-id="e98c3-128">在请求正文中，提供 deviceComplianceScriptDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e98c3-128">In the request body, supply a JSON representation for the deviceComplianceScriptDeviceState object.</span></span>

<span data-ttu-id="e98c3-129">下表显示创建 deviceComplianceScriptDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e98c3-129">The following table shows the properties that are required when you create the deviceComplianceScriptDeviceState.</span></span>

|<span data-ttu-id="e98c3-130">属性</span><span class="sxs-lookup"><span data-stu-id="e98c3-130">Property</span></span>|<span data-ttu-id="e98c3-131">类型</span><span class="sxs-lookup"><span data-stu-id="e98c3-131">Type</span></span>|<span data-ttu-id="e98c3-132">说明</span><span class="sxs-lookup"><span data-stu-id="e98c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e98c3-133">id</span><span class="sxs-lookup"><span data-stu-id="e98c3-133">id</span></span>|<span data-ttu-id="e98c3-134">String</span><span class="sxs-lookup"><span data-stu-id="e98c3-134">String</span></span>|<span data-ttu-id="e98c3-135">设备合规性脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="e98c3-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="e98c3-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e98c3-136">This property is read-only.</span></span>|
|<span data-ttu-id="e98c3-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="e98c3-137">detectionState</span></span>|[<span data-ttu-id="e98c3-138">runState</span><span class="sxs-lookup"><span data-stu-id="e98c3-138">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e98c3-139">Lastest 设备合规性脚本执行中的检测状态。</span><span class="sxs-lookup"><span data-stu-id="e98c3-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="e98c3-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e98c3-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="e98c3-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e98c3-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="e98c3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e98c3-142">DateTimeOffset</span></span>|<span data-ttu-id="e98c3-143">执行设备符合性脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="e98c3-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="e98c3-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e98c3-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="e98c3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e98c3-145">DateTimeOffset</span></span>|<span data-ttu-id="e98c3-146">预期何时执行设备符合性脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="e98c3-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="e98c3-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e98c3-147">lastSyncDateTime</span></span>|<span data-ttu-id="e98c3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e98c3-148">DateTimeOffset</span></span>|<span data-ttu-id="e98c3-149">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="e98c3-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="e98c3-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="e98c3-150">scriptOutput</span></span>|<span data-ttu-id="e98c3-151">String</span><span class="sxs-lookup"><span data-stu-id="e98c3-151">String</span></span>|<span data-ttu-id="e98c3-152">检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="e98c3-152">Output of the detection script</span></span>|
|<span data-ttu-id="e98c3-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="e98c3-153">scriptError</span></span>|<span data-ttu-id="e98c3-154">String</span><span class="sxs-lookup"><span data-stu-id="e98c3-154">String</span></span>|<span data-ttu-id="e98c3-155">检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="e98c3-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="e98c3-156">响应</span><span class="sxs-lookup"><span data-stu-id="e98c3-156">Response</span></span>
<span data-ttu-id="e98c3-157">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e98c3-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e98c3-158">示例</span><span class="sxs-lookup"><span data-stu-id="e98c3-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e98c3-159">请求</span><span class="sxs-lookup"><span data-stu-id="e98c3-159">Request</span></span>
<span data-ttu-id="e98c3-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e98c3-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="e98c3-161">响应</span><span class="sxs-lookup"><span data-stu-id="e98c3-161">Response</span></span>
<span data-ttu-id="e98c3-162">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e98c3-162">Here is an example of the response.</span></span> <span data-ttu-id="e98c3-163">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e98c3-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e98c3-164">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e98c3-164">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



