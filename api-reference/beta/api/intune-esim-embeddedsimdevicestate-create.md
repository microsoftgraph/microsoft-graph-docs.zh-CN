---
title: 创建 embeddedSIMDeviceState
description: 创建新的 embeddedSIMDeviceState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a501672f84cee4ffd5f0c85be5772827d847019
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995242"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="4631f-103">创建 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="4631f-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="4631f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4631f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4631f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4631f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4631f-106">创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4631f-106">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4631f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4631f-107">Prerequisites</span></span>
<span data-ttu-id="4631f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4631f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4631f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4631f-110">Permission type</span></span>|<span data-ttu-id="4631f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4631f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4631f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4631f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4631f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4631f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4631f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4631f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4631f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4631f-115">Not supported.</span></span>|
|<span data-ttu-id="4631f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4631f-116">Application</span></span>|<span data-ttu-id="4631f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4631f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4631f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4631f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="4631f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4631f-119">Request headers</span></span>
|<span data-ttu-id="4631f-120">标头</span><span class="sxs-lookup"><span data-stu-id="4631f-120">Header</span></span>|<span data-ttu-id="4631f-121">值</span><span class="sxs-lookup"><span data-stu-id="4631f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4631f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4631f-122">Authorization</span></span>|<span data-ttu-id="4631f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4631f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4631f-124">接受</span><span class="sxs-lookup"><span data-stu-id="4631f-124">Accept</span></span>|<span data-ttu-id="4631f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4631f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4631f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4631f-126">Request body</span></span>
<span data-ttu-id="4631f-127">在请求正文中, 提供 embeddedSIMDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4631f-127">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="4631f-128">下表显示创建 embeddedSIMDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4631f-128">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="4631f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4631f-129">Property</span></span>|<span data-ttu-id="4631f-130">类型</span><span class="sxs-lookup"><span data-stu-id="4631f-130">Type</span></span>|<span data-ttu-id="4631f-131">说明</span><span class="sxs-lookup"><span data-stu-id="4631f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4631f-132">id</span><span class="sxs-lookup"><span data-stu-id="4631f-132">id</span></span>|<span data-ttu-id="4631f-133">String</span><span class="sxs-lookup"><span data-stu-id="4631f-133">String</span></span>|<span data-ttu-id="4631f-134">嵌入的 SIM 卡设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4631f-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="4631f-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="4631f-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="4631f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4631f-136">createdDateTime</span></span>|<span data-ttu-id="4631f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4631f-137">DateTimeOffset</span></span>|<span data-ttu-id="4631f-138">嵌入的 SIM 设备状态的创建时间。</span><span class="sxs-lookup"><span data-stu-id="4631f-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="4631f-139">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="4631f-139">Generated service side.</span></span>|
|<span data-ttu-id="4631f-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4631f-140">modifiedDateTime</span></span>|<span data-ttu-id="4631f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4631f-141">DateTimeOffset</span></span>|<span data-ttu-id="4631f-142">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="4631f-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="4631f-143">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="4631f-143">Updated service side.</span></span>|
|<span data-ttu-id="4631f-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4631f-144">lastSyncDateTime</span></span>|<span data-ttu-id="4631f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4631f-145">DateTimeOffset</span></span>|<span data-ttu-id="4631f-146">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="4631f-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="4631f-147">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="4631f-147">Updated service side.</span></span>|
|<span data-ttu-id="4631f-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="4631f-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="4631f-149">String</span><span class="sxs-lookup"><span data-stu-id="4631f-149">String</span></span>|<span data-ttu-id="4631f-150">通用集成电路卡标识符 (UICCID), 用于标识要在其上部署配置文件的硬件。</span><span class="sxs-lookup"><span data-stu-id="4631f-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="4631f-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="4631f-151">deviceName</span></span>|<span data-ttu-id="4631f-152">String</span><span class="sxs-lookup"><span data-stu-id="4631f-152">String</span></span>|<span data-ttu-id="4631f-153">订阅预配到的设备名称, 例如, 桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="4631f-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="4631f-154">userName</span><span class="sxs-lookup"><span data-stu-id="4631f-154">userName</span></span>|<span data-ttu-id="4631f-155">String</span><span class="sxs-lookup"><span data-stu-id="4631f-155">String</span></span>|<span data-ttu-id="4631f-156">订阅预配到的用户名, 例如 joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="4631f-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="4631f-157">state</span><span class="sxs-lookup"><span data-stu-id="4631f-157">state</span></span>|[<span data-ttu-id="4631f-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="4631f-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="4631f-159">应用于设备的配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4631f-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="4631f-160">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="4631f-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="4631f-161">stateDetails</span><span class="sxs-lookup"><span data-stu-id="4631f-161">stateDetails</span></span>|<span data-ttu-id="4631f-162">String</span><span class="sxs-lookup"><span data-stu-id="4631f-162">String</span></span>|<span data-ttu-id="4631f-163">设置状态的字符串说明。</span><span class="sxs-lookup"><span data-stu-id="4631f-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="4631f-164">响应</span><span class="sxs-lookup"><span data-stu-id="4631f-164">Response</span></span>
<span data-ttu-id="4631f-165">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4631f-165">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4631f-166">示例</span><span class="sxs-lookup"><span data-stu-id="4631f-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="4631f-167">请求</span><span class="sxs-lookup"><span data-stu-id="4631f-167">Request</span></span>
<span data-ttu-id="4631f-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4631f-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="4631f-169">响应</span><span class="sxs-lookup"><span data-stu-id="4631f-169">Response</span></span>
<span data-ttu-id="4631f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4631f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





