---
title: 更新 deviceComplianceScriptDeviceState
description: 更新 deviceComplianceScriptDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 107716380bf7ef598b7071fd1299f5a25a3c911c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611900"
---
# <a name="update-devicecompliancescriptdevicestate"></a><span data-ttu-id="88ba1-103">更新 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88ba1-103">Update deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="88ba1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ba1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88ba1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88ba1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88ba1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88ba1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88ba1-107">更新 [deviceComplianceScriptDeviceState 对象](../resources/intune-devices-devicecompliancescriptdevicestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="88ba1-107">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88ba1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88ba1-108">Prerequisites</span></span>
<span data-ttu-id="88ba1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88ba1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88ba1-111">Permission type</span></span>|<span data-ttu-id="88ba1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88ba1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88ba1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88ba1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88ba1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ba1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88ba1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88ba1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88ba1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88ba1-116">Not supported.</span></span>|
|<span data-ttu-id="88ba1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88ba1-117">Application</span></span>|<span data-ttu-id="88ba1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ba1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88ba1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88ba1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="88ba1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88ba1-120">Request headers</span></span>
|<span data-ttu-id="88ba1-121">标头</span><span class="sxs-lookup"><span data-stu-id="88ba1-121">Header</span></span>|<span data-ttu-id="88ba1-122">值</span><span class="sxs-lookup"><span data-stu-id="88ba1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88ba1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88ba1-123">Authorization</span></span>|<span data-ttu-id="88ba1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88ba1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88ba1-125">接受</span><span class="sxs-lookup"><span data-stu-id="88ba1-125">Accept</span></span>|<span data-ttu-id="88ba1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88ba1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88ba1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88ba1-127">Request body</span></span>
<span data-ttu-id="88ba1-128">在请求正文中，提供 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88ba1-128">In the request body, supply a JSON representation for the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

<span data-ttu-id="88ba1-129">下表显示创建 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88ba1-129">The following table shows the properties that are required when you create the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>

|<span data-ttu-id="88ba1-130">属性</span><span class="sxs-lookup"><span data-stu-id="88ba1-130">Property</span></span>|<span data-ttu-id="88ba1-131">类型</span><span class="sxs-lookup"><span data-stu-id="88ba1-131">Type</span></span>|<span data-ttu-id="88ba1-132">说明</span><span class="sxs-lookup"><span data-stu-id="88ba1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ba1-133">id</span><span class="sxs-lookup"><span data-stu-id="88ba1-133">id</span></span>|<span data-ttu-id="88ba1-134">String</span><span class="sxs-lookup"><span data-stu-id="88ba1-134">String</span></span>|<span data-ttu-id="88ba1-135">设备合规性脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="88ba1-135">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="88ba1-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88ba1-136">This property is read-only.</span></span>|
|<span data-ttu-id="88ba1-137">detectionState</span><span class="sxs-lookup"><span data-stu-id="88ba1-137">detectionState</span></span>|[<span data-ttu-id="88ba1-138">runState</span><span class="sxs-lookup"><span data-stu-id="88ba1-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="88ba1-139">最近一次执行设备合规性脚本的检测状态。</span><span class="sxs-lookup"><span data-stu-id="88ba1-139">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="88ba1-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="88ba1-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="88ba1-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="88ba1-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="88ba1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ba1-142">DateTimeOffset</span></span>|<span data-ttu-id="88ba1-143">执行设备合规性脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="88ba1-143">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="88ba1-144">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="88ba1-144">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="88ba1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ba1-145">DateTimeOffset</span></span>|<span data-ttu-id="88ba1-146">下一次执行设备合规性脚本的时间戳</span><span class="sxs-lookup"><span data-stu-id="88ba1-146">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="88ba1-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="88ba1-147">lastSyncDateTime</span></span>|<span data-ttu-id="88ba1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ba1-148">DateTimeOffset</span></span>|<span data-ttu-id="88ba1-149">Intune 管理扩展上次与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="88ba1-149">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="88ba1-150">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="88ba1-150">scriptOutput</span></span>|<span data-ttu-id="88ba1-151">String</span><span class="sxs-lookup"><span data-stu-id="88ba1-151">String</span></span>|<span data-ttu-id="88ba1-152">检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="88ba1-152">Output of the detection script</span></span>|
|<span data-ttu-id="88ba1-153">scriptError</span><span class="sxs-lookup"><span data-stu-id="88ba1-153">scriptError</span></span>|<span data-ttu-id="88ba1-154">String</span><span class="sxs-lookup"><span data-stu-id="88ba1-154">String</span></span>|<span data-ttu-id="88ba1-155">检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="88ba1-155">Error from the detection script</span></span>|



## <a name="response"></a><span data-ttu-id="88ba1-156">响应</span><span class="sxs-lookup"><span data-stu-id="88ba1-156">Response</span></span>
<span data-ttu-id="88ba1-157">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88ba1-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88ba1-158">示例</span><span class="sxs-lookup"><span data-stu-id="88ba1-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="88ba1-159">请求</span><span class="sxs-lookup"><span data-stu-id="88ba1-159">Request</span></span>
<span data-ttu-id="88ba1-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88ba1-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88ba1-161">响应</span><span class="sxs-lookup"><span data-stu-id="88ba1-161">Response</span></span>
<span data-ttu-id="88ba1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88ba1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




