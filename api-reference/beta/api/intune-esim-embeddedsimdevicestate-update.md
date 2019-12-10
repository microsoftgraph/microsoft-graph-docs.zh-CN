---
title: 更新 embeddedSIMDeviceState
description: 更新 embeddedSIMDeviceState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bf7a48ccef44f8bcb2c9cb8d7753afe339b17d8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943521"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="11dd8-103">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="11dd8-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="11dd8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11dd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11dd8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11dd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11dd8-106">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="11dd8-106">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11dd8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="11dd8-107">Prerequisites</span></span>
<span data-ttu-id="11dd8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11dd8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11dd8-110">Permission type</span></span>|<span data-ttu-id="11dd8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11dd8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11dd8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11dd8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11dd8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dd8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11dd8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11dd8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11dd8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11dd8-115">Not supported.</span></span>|
|<span data-ttu-id="11dd8-116">Application</span><span class="sxs-lookup"><span data-stu-id="11dd8-116">Application</span></span>|<span data-ttu-id="11dd8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dd8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11dd8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11dd8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="11dd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="11dd8-119">Request headers</span></span>
|<span data-ttu-id="11dd8-120">标头</span><span class="sxs-lookup"><span data-stu-id="11dd8-120">Header</span></span>|<span data-ttu-id="11dd8-121">值</span><span class="sxs-lookup"><span data-stu-id="11dd8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11dd8-122">授权</span><span class="sxs-lookup"><span data-stu-id="11dd8-122">Authorization</span></span>|<span data-ttu-id="11dd8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="11dd8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11dd8-124">接受</span><span class="sxs-lookup"><span data-stu-id="11dd8-124">Accept</span></span>|<span data-ttu-id="11dd8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11dd8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11dd8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="11dd8-126">Request body</span></span>
<span data-ttu-id="11dd8-127">在请求正文中，提供[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11dd8-127">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="11dd8-128">下表显示创建[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="11dd8-128">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="11dd8-129">属性</span><span class="sxs-lookup"><span data-stu-id="11dd8-129">Property</span></span>|<span data-ttu-id="11dd8-130">类型</span><span class="sxs-lookup"><span data-stu-id="11dd8-130">Type</span></span>|<span data-ttu-id="11dd8-131">说明</span><span class="sxs-lookup"><span data-stu-id="11dd8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11dd8-132">id</span><span class="sxs-lookup"><span data-stu-id="11dd8-132">id</span></span>|<span data-ttu-id="11dd8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="11dd8-133">String</span></span>|<span data-ttu-id="11dd8-134">嵌入的 SIM 卡设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="11dd8-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="11dd8-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="11dd8-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="11dd8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11dd8-136">createdDateTime</span></span>|<span data-ttu-id="11dd8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dd8-137">DateTimeOffset</span></span>|<span data-ttu-id="11dd8-138">嵌入的 SIM 设备状态的创建时间。</span><span class="sxs-lookup"><span data-stu-id="11dd8-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="11dd8-139">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="11dd8-139">Generated service side.</span></span>|
|<span data-ttu-id="11dd8-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11dd8-140">modifiedDateTime</span></span>|<span data-ttu-id="11dd8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dd8-141">DateTimeOffset</span></span>|<span data-ttu-id="11dd8-142">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="11dd8-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="11dd8-143">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="11dd8-143">Updated service side.</span></span>|
|<span data-ttu-id="11dd8-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="11dd8-144">lastSyncDateTime</span></span>|<span data-ttu-id="11dd8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dd8-145">DateTimeOffset</span></span>|<span data-ttu-id="11dd8-146">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="11dd8-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="11dd8-147">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="11dd8-147">Updated service side.</span></span>|
|<span data-ttu-id="11dd8-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="11dd8-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="11dd8-149">字符串</span><span class="sxs-lookup"><span data-stu-id="11dd8-149">String</span></span>|<span data-ttu-id="11dd8-150">通用集成电路卡标识符（UICCID），用于标识要在其上部署配置文件的硬件。</span><span class="sxs-lookup"><span data-stu-id="11dd8-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="11dd8-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="11dd8-151">deviceName</span></span>|<span data-ttu-id="11dd8-152">字符串</span><span class="sxs-lookup"><span data-stu-id="11dd8-152">String</span></span>|<span data-ttu-id="11dd8-153">订阅预配到的设备名称，例如，桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="11dd8-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="11dd8-154">userName</span><span class="sxs-lookup"><span data-stu-id="11dd8-154">userName</span></span>|<span data-ttu-id="11dd8-155">String</span><span class="sxs-lookup"><span data-stu-id="11dd8-155">String</span></span>|<span data-ttu-id="11dd8-156">订阅预配到的用户名，例如 joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="11dd8-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="11dd8-157">state</span><span class="sxs-lookup"><span data-stu-id="11dd8-157">state</span></span>|[<span data-ttu-id="11dd8-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="11dd8-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="11dd8-159">应用于设备的配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="11dd8-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="11dd8-160">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="11dd8-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="11dd8-161">stateDetails</span><span class="sxs-lookup"><span data-stu-id="11dd8-161">stateDetails</span></span>|<span data-ttu-id="11dd8-162">字符串</span><span class="sxs-lookup"><span data-stu-id="11dd8-162">String</span></span>|<span data-ttu-id="11dd8-163">设置状态的字符串说明。</span><span class="sxs-lookup"><span data-stu-id="11dd8-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="11dd8-164">响应</span><span class="sxs-lookup"><span data-stu-id="11dd8-164">Response</span></span>
<span data-ttu-id="11dd8-165">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11dd8-165">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11dd8-166">示例</span><span class="sxs-lookup"><span data-stu-id="11dd8-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="11dd8-167">请求</span><span class="sxs-lookup"><span data-stu-id="11dd8-167">Request</span></span>
<span data-ttu-id="11dd8-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11dd8-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11dd8-169">响应</span><span class="sxs-lookup"><span data-stu-id="11dd8-169">Response</span></span>
<span data-ttu-id="11dd8-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="11dd8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





