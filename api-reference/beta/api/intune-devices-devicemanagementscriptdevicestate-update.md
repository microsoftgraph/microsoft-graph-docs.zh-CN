---
title: 更新 deviceManagementScriptDeviceState
description: 更新 deviceManagementScriptDeviceState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65da8583b854c2cd912e877729bbe3ec7735c92a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170607"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="cb6af-103">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="cb6af-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="cb6af-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb6af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb6af-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb6af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb6af-106">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb6af-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb6af-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb6af-107">Prerequisites</span></span>
<span data-ttu-id="cb6af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cb6af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cb6af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb6af-110">Permission type</span></span>|<span data-ttu-id="cb6af-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb6af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb6af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb6af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb6af-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6af-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb6af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb6af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb6af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb6af-115">Not supported.</span></span>|
|<span data-ttu-id="cb6af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb6af-116">Application</span></span>|<span data-ttu-id="cb6af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb6af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb6af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb6af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cb6af-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb6af-119">Request headers</span></span>
|<span data-ttu-id="cb6af-120">标头</span><span class="sxs-lookup"><span data-stu-id="cb6af-120">Header</span></span>|<span data-ttu-id="cb6af-121">值</span><span class="sxs-lookup"><span data-stu-id="cb6af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb6af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb6af-122">Authorization</span></span>|<span data-ttu-id="cb6af-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb6af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb6af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cb6af-124">Accept</span></span>|<span data-ttu-id="cb6af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb6af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb6af-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb6af-126">Request body</span></span>
<span data-ttu-id="cb6af-127">在请求正文中, 提供[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb6af-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="cb6af-128">下表显示创建[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb6af-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="cb6af-129">属性</span><span class="sxs-lookup"><span data-stu-id="cb6af-129">Property</span></span>|<span data-ttu-id="cb6af-130">类型</span><span class="sxs-lookup"><span data-stu-id="cb6af-130">Type</span></span>|<span data-ttu-id="cb6af-131">说明</span><span class="sxs-lookup"><span data-stu-id="cb6af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6af-132">id</span><span class="sxs-lookup"><span data-stu-id="cb6af-132">id</span></span>|<span data-ttu-id="cb6af-133">String</span><span class="sxs-lookup"><span data-stu-id="cb6af-133">String</span></span>|<span data-ttu-id="cb6af-134">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="cb6af-134">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="cb6af-135">runState</span><span class="sxs-lookup"><span data-stu-id="cb6af-135">runState</span></span>|[<span data-ttu-id="cb6af-136">runState</span><span class="sxs-lookup"><span data-stu-id="cb6af-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="cb6af-137">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="cb6af-137">State of latest run of the device management script.</span></span> <span data-ttu-id="cb6af-138">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="cb6af-138">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="cb6af-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="cb6af-139">resultMessage</span></span>|<span data-ttu-id="cb6af-140">String</span><span class="sxs-lookup"><span data-stu-id="cb6af-140">String</span></span>|<span data-ttu-id="cb6af-141">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cb6af-141">Details of execution output.</span></span>|
|<span data-ttu-id="cb6af-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cb6af-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="cb6af-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb6af-143">DateTimeOffset</span></span>|<span data-ttu-id="cb6af-144">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="cb6af-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="cb6af-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="cb6af-145">errorCode</span></span>|<span data-ttu-id="cb6af-146">Int32</span><span class="sxs-lookup"><span data-stu-id="cb6af-146">Int32</span></span>|<span data-ttu-id="cb6af-147">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="cb6af-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="cb6af-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="cb6af-148">errorDescription</span></span>|<span data-ttu-id="cb6af-149">String</span><span class="sxs-lookup"><span data-stu-id="cb6af-149">String</span></span>|<span data-ttu-id="cb6af-150">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="cb6af-150">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="cb6af-151">响应</span><span class="sxs-lookup"><span data-stu-id="cb6af-151">Response</span></span>
<span data-ttu-id="cb6af-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb6af-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb6af-153">示例</span><span class="sxs-lookup"><span data-stu-id="cb6af-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb6af-154">请求</span><span class="sxs-lookup"><span data-stu-id="cb6af-154">Request</span></span>
<span data-ttu-id="cb6af-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb6af-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="cb6af-156">响应</span><span class="sxs-lookup"><span data-stu-id="cb6af-156">Response</span></span>
<span data-ttu-id="cb6af-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb6af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




