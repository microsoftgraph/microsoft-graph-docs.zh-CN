---
title: 创建 deviceManagementScriptDeviceState
description: 创建新的 deviceManagementScriptDeviceState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfd0b21906cd7692e32b93475efdb8b861ed44b3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530613"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="2deaa-103">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2deaa-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="2deaa-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2deaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2deaa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2deaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2deaa-106">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2deaa-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2deaa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2deaa-107">Prerequisites</span></span>
<span data-ttu-id="2deaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2deaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2deaa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2deaa-110">Permission type</span></span>|<span data-ttu-id="2deaa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2deaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2deaa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2deaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2deaa-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2deaa-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2deaa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2deaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2deaa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2deaa-115">Not supported.</span></span>|
|<span data-ttu-id="2deaa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2deaa-116">Application</span></span>|<span data-ttu-id="2deaa-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2deaa-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2deaa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2deaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="2deaa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2deaa-119">Request headers</span></span>
|<span data-ttu-id="2deaa-120">标头</span><span class="sxs-lookup"><span data-stu-id="2deaa-120">Header</span></span>|<span data-ttu-id="2deaa-121">值</span><span class="sxs-lookup"><span data-stu-id="2deaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2deaa-122">授权</span><span class="sxs-lookup"><span data-stu-id="2deaa-122">Authorization</span></span>|<span data-ttu-id="2deaa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2deaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2deaa-124">接受</span><span class="sxs-lookup"><span data-stu-id="2deaa-124">Accept</span></span>|<span data-ttu-id="2deaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2deaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2deaa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2deaa-126">Request body</span></span>
<span data-ttu-id="2deaa-127">在请求正文中，提供 deviceManagementScriptDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2deaa-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="2deaa-128">下表显示创建 deviceManagementScriptDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2deaa-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="2deaa-129">属性</span><span class="sxs-lookup"><span data-stu-id="2deaa-129">Property</span></span>|<span data-ttu-id="2deaa-130">类型</span><span class="sxs-lookup"><span data-stu-id="2deaa-130">Type</span></span>|<span data-ttu-id="2deaa-131">说明</span><span class="sxs-lookup"><span data-stu-id="2deaa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2deaa-132">id</span><span class="sxs-lookup"><span data-stu-id="2deaa-132">id</span></span>|<span data-ttu-id="2deaa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2deaa-133">String</span></span>|<span data-ttu-id="2deaa-134">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="2deaa-134">Key of the device management script device state entity.</span></span> <span data-ttu-id="2deaa-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2deaa-135">This property is read-only.</span></span>|
|<span data-ttu-id="2deaa-136">runState</span><span class="sxs-lookup"><span data-stu-id="2deaa-136">runState</span></span>|[<span data-ttu-id="2deaa-137">runState</span><span class="sxs-lookup"><span data-stu-id="2deaa-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="2deaa-138">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="2deaa-138">State of latest run of the device management script.</span></span> <span data-ttu-id="2deaa-139">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="2deaa-139">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="2deaa-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="2deaa-140">resultMessage</span></span>|<span data-ttu-id="2deaa-141">字符串</span><span class="sxs-lookup"><span data-stu-id="2deaa-141">String</span></span>|<span data-ttu-id="2deaa-142">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2deaa-142">Details of execution output.</span></span>|
|<span data-ttu-id="2deaa-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2deaa-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="2deaa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2deaa-144">DateTimeOffset</span></span>|<span data-ttu-id="2deaa-145">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="2deaa-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="2deaa-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="2deaa-146">errorCode</span></span>|<span data-ttu-id="2deaa-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2deaa-147">Int32</span></span>|<span data-ttu-id="2deaa-148">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="2deaa-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="2deaa-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="2deaa-149">errorDescription</span></span>|<span data-ttu-id="2deaa-150">String</span><span class="sxs-lookup"><span data-stu-id="2deaa-150">String</span></span>|<span data-ttu-id="2deaa-151">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="2deaa-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="2deaa-152">响应</span><span class="sxs-lookup"><span data-stu-id="2deaa-152">Response</span></span>
<span data-ttu-id="2deaa-153">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2deaa-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2deaa-154">示例</span><span class="sxs-lookup"><span data-stu-id="2deaa-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="2deaa-155">请求</span><span class="sxs-lookup"><span data-stu-id="2deaa-155">Request</span></span>
<span data-ttu-id="2deaa-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2deaa-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="2deaa-157">响应</span><span class="sxs-lookup"><span data-stu-id="2deaa-157">Response</span></span>
<span data-ttu-id="2deaa-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2deaa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






