---
title: 更新 embeddedSIMDeviceState
description: 更新 embeddedSIMDeviceState 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f29da78f3a0a614ce5e2bdb79ab7e88e5018a403
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408703"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="bc91f-103">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="bc91f-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="bc91f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bc91f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc91f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc91f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc91f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc91f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc91f-107">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc91f-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc91f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc91f-108">Prerequisites</span></span>
<span data-ttu-id="bc91f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bc91f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc91f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc91f-111">Permission type</span></span>|<span data-ttu-id="bc91f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc91f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc91f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc91f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc91f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc91f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc91f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc91f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc91f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc91f-116">Not supported.</span></span>|
|<span data-ttu-id="bc91f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc91f-117">Application</span></span>|<span data-ttu-id="bc91f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc91f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc91f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc91f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="bc91f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc91f-120">Request headers</span></span>
|<span data-ttu-id="bc91f-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc91f-121">Header</span></span>|<span data-ttu-id="bc91f-122">值</span><span class="sxs-lookup"><span data-stu-id="bc91f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc91f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc91f-123">Authorization</span></span>|<span data-ttu-id="bc91f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc91f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc91f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc91f-125">Accept</span></span>|<span data-ttu-id="bc91f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc91f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc91f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc91f-127">Request body</span></span>
<span data-ttu-id="bc91f-128">在请求正文中，提供[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc91f-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="bc91f-129">下表显示时创建[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc91f-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="bc91f-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc91f-130">Property</span></span>|<span data-ttu-id="bc91f-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc91f-131">Type</span></span>|<span data-ttu-id="bc91f-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc91f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc91f-133">id</span><span class="sxs-lookup"><span data-stu-id="bc91f-133">id</span></span>|<span data-ttu-id="bc91f-134">String</span><span class="sxs-lookup"><span data-stu-id="bc91f-134">String</span></span>|<span data-ttu-id="bc91f-135">嵌入 SIM 设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bc91f-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="bc91f-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="bc91f-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="bc91f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc91f-137">createdDateTime</span></span>|<span data-ttu-id="bc91f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc91f-138">DateTimeOffset</span></span>|<span data-ttu-id="bc91f-139">创建嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="bc91f-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="bc91f-140">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="bc91f-140">Generated service side.</span></span>|
|<span data-ttu-id="bc91f-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc91f-141">modifiedDateTime</span></span>|<span data-ttu-id="bc91f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc91f-142">DateTimeOffset</span></span>|<span data-ttu-id="bc91f-143">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="bc91f-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="bc91f-144">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="bc91f-144">Updated service side.</span></span>|
|<span data-ttu-id="bc91f-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bc91f-145">lastSyncDateTime</span></span>|<span data-ttu-id="bc91f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc91f-146">DateTimeOffset</span></span>|<span data-ttu-id="bc91f-147">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="bc91f-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="bc91f-148">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="bc91f-148">Updated service side.</span></span>|
|<span data-ttu-id="bc91f-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc91f-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="bc91f-150">String</span><span class="sxs-lookup"><span data-stu-id="bc91f-150">String</span></span>|<span data-ttu-id="bc91f-151">通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。</span><span class="sxs-lookup"><span data-stu-id="bc91f-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="bc91f-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="bc91f-152">deviceName</span></span>|<span data-ttu-id="bc91f-153">String</span><span class="sxs-lookup"><span data-stu-id="bc91f-153">String</span></span>|<span data-ttu-id="bc91f-154">订阅已的设备名称设置如桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="bc91f-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="bc91f-155">userName</span><span class="sxs-lookup"><span data-stu-id="bc91f-155">userName</span></span>|<span data-ttu-id="bc91f-156">String</span><span class="sxs-lookup"><span data-stu-id="bc91f-156">String</span></span>|<span data-ttu-id="bc91f-157">订阅已设置到例如 joe@contoso.com 用户名</span><span class="sxs-lookup"><span data-stu-id="bc91f-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="bc91f-158">state</span><span class="sxs-lookup"><span data-stu-id="bc91f-158">state</span></span>|[<span data-ttu-id="bc91f-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="bc91f-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="bc91f-160">应用于该设备配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="bc91f-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="bc91f-161">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="bc91f-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="bc91f-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="bc91f-162">stateDetails</span></span>|<span data-ttu-id="bc91f-163">String</span><span class="sxs-lookup"><span data-stu-id="bc91f-163">String</span></span>|<span data-ttu-id="bc91f-164">字符串设置状态的说明。</span><span class="sxs-lookup"><span data-stu-id="bc91f-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="bc91f-165">响应</span><span class="sxs-lookup"><span data-stu-id="bc91f-165">Response</span></span>
<span data-ttu-id="bc91f-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bc91f-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc91f-167">示例</span><span class="sxs-lookup"><span data-stu-id="bc91f-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc91f-168">请求</span><span class="sxs-lookup"><span data-stu-id="bc91f-168">Request</span></span>
<span data-ttu-id="bc91f-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc91f-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="bc91f-170">响应</span><span class="sxs-lookup"><span data-stu-id="bc91f-170">Response</span></span>
<span data-ttu-id="bc91f-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc91f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```




