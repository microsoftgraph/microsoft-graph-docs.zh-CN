---
title: 创建 deviceManagementScriptDeviceState
description: 创建新的 deviceManagementScriptDeviceState 对象。
author: tfitzmac
ms.openlocfilehash: 2b809c82e077bc75c354d3b8b1c09548eaacad64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304849"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="69426-103">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="69426-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="69426-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69426-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69426-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69426-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69426-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69426-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69426-107">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69426-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69426-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69426-108">Prerequisites</span></span>
<span data-ttu-id="69426-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="69426-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69426-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69426-111">Permission type</span></span>|<span data-ttu-id="69426-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69426-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69426-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69426-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69426-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69426-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69426-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69426-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69426-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69426-116">Not supported.</span></span>|
|<span data-ttu-id="69426-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69426-117">Application</span></span>|<span data-ttu-id="69426-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69426-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69426-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69426-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="69426-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69426-120">Request headers</span></span>
|<span data-ttu-id="69426-121">标头</span><span class="sxs-lookup"><span data-stu-id="69426-121">Header</span></span>|<span data-ttu-id="69426-122">值</span><span class="sxs-lookup"><span data-stu-id="69426-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69426-123">授权</span><span class="sxs-lookup"><span data-stu-id="69426-123">Authorization</span></span>|<span data-ttu-id="69426-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69426-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69426-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69426-125">Accept</span></span>|<span data-ttu-id="69426-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69426-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69426-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69426-127">Request body</span></span>
<span data-ttu-id="69426-128">在请求正文中，提供 deviceManagementScriptDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69426-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="69426-129">下表显示时创建 deviceManagementScriptDeviceState 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69426-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="69426-130">属性</span><span class="sxs-lookup"><span data-stu-id="69426-130">Property</span></span>|<span data-ttu-id="69426-131">类型</span><span class="sxs-lookup"><span data-stu-id="69426-131">Type</span></span>|<span data-ttu-id="69426-132">说明</span><span class="sxs-lookup"><span data-stu-id="69426-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69426-133">id</span><span class="sxs-lookup"><span data-stu-id="69426-133">id</span></span>|<span data-ttu-id="69426-134">字符串</span><span class="sxs-lookup"><span data-stu-id="69426-134">String</span></span>|<span data-ttu-id="69426-135">设备管理脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="69426-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="69426-136">runState</span><span class="sxs-lookup"><span data-stu-id="69426-136">runState</span></span>|[<span data-ttu-id="69426-137">runState</span><span class="sxs-lookup"><span data-stu-id="69426-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="69426-138">设备管理脚本的最新运行状态。</span><span class="sxs-lookup"><span data-stu-id="69426-138">State of latest run of the device management script.</span></span> <span data-ttu-id="69426-139">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="69426-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="69426-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="69426-140">resultMessage</span></span>|<span data-ttu-id="69426-141">字符串</span><span class="sxs-lookup"><span data-stu-id="69426-141">String</span></span>|<span data-ttu-id="69426-142">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="69426-142">Details of execution output.</span></span>|
|<span data-ttu-id="69426-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="69426-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="69426-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69426-144">DateTimeOffset</span></span>|<span data-ttu-id="69426-145">最新时间设备管理脚本执行。</span><span class="sxs-lookup"><span data-stu-id="69426-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="69426-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="69426-146">errorCode</span></span>|<span data-ttu-id="69426-147">Int32</span><span class="sxs-lookup"><span data-stu-id="69426-147">Int32</span></span>|<span data-ttu-id="69426-148">错误代码对应的设备管理脚本错误执行。</span><span class="sxs-lookup"><span data-stu-id="69426-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="69426-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="69426-149">errorDescription</span></span>|<span data-ttu-id="69426-150">String</span><span class="sxs-lookup"><span data-stu-id="69426-150">String</span></span>|<span data-ttu-id="69426-151">设备管理脚本错误执行所对应的错误描述。</span><span class="sxs-lookup"><span data-stu-id="69426-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="69426-152">响应</span><span class="sxs-lookup"><span data-stu-id="69426-152">Response</span></span>
<span data-ttu-id="69426-153">如果成功，此方法返回`201 Created`响应代码和响应正文中的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69426-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69426-154">示例</span><span class="sxs-lookup"><span data-stu-id="69426-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="69426-155">请求</span><span class="sxs-lookup"><span data-stu-id="69426-155">Request</span></span>
<span data-ttu-id="69426-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69426-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69426-157">响应</span><span class="sxs-lookup"><span data-stu-id="69426-157">Response</span></span>
<span data-ttu-id="69426-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69426-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





