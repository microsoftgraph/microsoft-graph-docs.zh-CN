---
title: 更新 deviceManagementScriptDeviceState
description: 更新 deviceManagementScriptDeviceState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9014ae76127e37965b7f57d90bb39f4bdfa354fa
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611844"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="64d54-103">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="64d54-103">Update deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="64d54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64d54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64d54-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64d54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64d54-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64d54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64d54-107">更新 [deviceManagementScriptDeviceState 对象](../resources/intune-devices-devicemanagementscriptdevicestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="64d54-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64d54-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64d54-108">Prerequisites</span></span>
<span data-ttu-id="64d54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64d54-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="64d54-111">Permission type</span></span>|<span data-ttu-id="64d54-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64d54-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64d54-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64d54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64d54-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d54-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="64d54-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64d54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64d54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64d54-116">Not supported.</span></span>|
|<span data-ttu-id="64d54-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="64d54-117">Application</span></span>|<span data-ttu-id="64d54-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d54-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64d54-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64d54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="64d54-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64d54-120">Request headers</span></span>
|<span data-ttu-id="64d54-121">标头</span><span class="sxs-lookup"><span data-stu-id="64d54-121">Header</span></span>|<span data-ttu-id="64d54-122">值</span><span class="sxs-lookup"><span data-stu-id="64d54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64d54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64d54-123">Authorization</span></span>|<span data-ttu-id="64d54-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64d54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64d54-125">接受</span><span class="sxs-lookup"><span data-stu-id="64d54-125">Accept</span></span>|<span data-ttu-id="64d54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64d54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64d54-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64d54-127">Request body</span></span>
<span data-ttu-id="64d54-128">在请求正文中，提供 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64d54-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="64d54-129">下表显示创建 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="64d54-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="64d54-130">属性</span><span class="sxs-lookup"><span data-stu-id="64d54-130">Property</span></span>|<span data-ttu-id="64d54-131">类型</span><span class="sxs-lookup"><span data-stu-id="64d54-131">Type</span></span>|<span data-ttu-id="64d54-132">说明</span><span class="sxs-lookup"><span data-stu-id="64d54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64d54-133">id</span><span class="sxs-lookup"><span data-stu-id="64d54-133">id</span></span>|<span data-ttu-id="64d54-134">String</span><span class="sxs-lookup"><span data-stu-id="64d54-134">String</span></span>|<span data-ttu-id="64d54-135">设备管理脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="64d54-135">Key of the device management script device state entity.</span></span> <span data-ttu-id="64d54-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="64d54-136">This property is read-only.</span></span>|
|<span data-ttu-id="64d54-137">runState</span><span class="sxs-lookup"><span data-stu-id="64d54-137">runState</span></span>|[<span data-ttu-id="64d54-138">runState</span><span class="sxs-lookup"><span data-stu-id="64d54-138">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="64d54-139">设备管理脚本的最新运行状态。</span><span class="sxs-lookup"><span data-stu-id="64d54-139">State of latest run of the device management script.</span></span> <span data-ttu-id="64d54-140">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="64d54-140">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="64d54-141">resultMessage</span><span class="sxs-lookup"><span data-stu-id="64d54-141">resultMessage</span></span>|<span data-ttu-id="64d54-142">String</span><span class="sxs-lookup"><span data-stu-id="64d54-142">String</span></span>|<span data-ttu-id="64d54-143">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="64d54-143">Details of execution output.</span></span>|
|<span data-ttu-id="64d54-144">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="64d54-144">lastStateUpdateDateTime</span></span>|<span data-ttu-id="64d54-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64d54-145">DateTimeOffset</span></span>|<span data-ttu-id="64d54-146">设备管理脚本执行的最新时间。</span><span class="sxs-lookup"><span data-stu-id="64d54-146">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="64d54-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="64d54-147">errorCode</span></span>|<span data-ttu-id="64d54-148">Int32</span><span class="sxs-lookup"><span data-stu-id="64d54-148">Int32</span></span>|<span data-ttu-id="64d54-149">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="64d54-149">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="64d54-150">errorDescription</span><span class="sxs-lookup"><span data-stu-id="64d54-150">errorDescription</span></span>|<span data-ttu-id="64d54-151">String</span><span class="sxs-lookup"><span data-stu-id="64d54-151">String</span></span>|<span data-ttu-id="64d54-152">与设备管理脚本的错误执行相对应的错误描述。</span><span class="sxs-lookup"><span data-stu-id="64d54-152">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="64d54-153">响应</span><span class="sxs-lookup"><span data-stu-id="64d54-153">Response</span></span>
<span data-ttu-id="64d54-154">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64d54-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64d54-155">示例</span><span class="sxs-lookup"><span data-stu-id="64d54-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="64d54-156">请求</span><span class="sxs-lookup"><span data-stu-id="64d54-156">Request</span></span>
<span data-ttu-id="64d54-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64d54-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="64d54-158">响应</span><span class="sxs-lookup"><span data-stu-id="64d54-158">Response</span></span>
<span data-ttu-id="64d54-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64d54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```




