---
title: 更新 embeddedSIMDeviceState
description: 更新 embeddedSIMDeviceState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cad82e5e211120d79e011647063762ae6a69ec60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858651"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="97baf-103">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="97baf-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="97baf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97baf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97baf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97baf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97baf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97baf-107">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97baf-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97baf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="97baf-108">Prerequisites</span></span>
<span data-ttu-id="97baf-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="97baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97baf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="97baf-111">Permission type</span></span>|<span data-ttu-id="97baf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="97baf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97baf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97baf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97baf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97baf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97baf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97baf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97baf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="97baf-116">Not supported.</span></span>|
|<span data-ttu-id="97baf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="97baf-117">Application</span></span>|<span data-ttu-id="97baf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="97baf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97baf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97baf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="97baf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="97baf-120">Request headers</span></span>
|<span data-ttu-id="97baf-121">标头</span><span class="sxs-lookup"><span data-stu-id="97baf-121">Header</span></span>|<span data-ttu-id="97baf-122">值</span><span class="sxs-lookup"><span data-stu-id="97baf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97baf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97baf-123">Authorization</span></span>|<span data-ttu-id="97baf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="97baf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97baf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97baf-125">Accept</span></span>|<span data-ttu-id="97baf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97baf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97baf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="97baf-127">Request body</span></span>
<span data-ttu-id="97baf-128">在请求正文中，提供[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97baf-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="97baf-129">下表显示时创建[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="97baf-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="97baf-130">属性</span><span class="sxs-lookup"><span data-stu-id="97baf-130">Property</span></span>|<span data-ttu-id="97baf-131">类型</span><span class="sxs-lookup"><span data-stu-id="97baf-131">Type</span></span>|<span data-ttu-id="97baf-132">说明</span><span class="sxs-lookup"><span data-stu-id="97baf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97baf-133">id</span><span class="sxs-lookup"><span data-stu-id="97baf-133">id</span></span>|<span data-ttu-id="97baf-134">字符串</span><span class="sxs-lookup"><span data-stu-id="97baf-134">String</span></span>|<span data-ttu-id="97baf-135">嵌入 SIM 设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="97baf-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="97baf-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="97baf-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="97baf-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97baf-137">createdDateTime</span></span>|<span data-ttu-id="97baf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97baf-138">DateTimeOffset</span></span>|<span data-ttu-id="97baf-139">创建嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="97baf-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="97baf-140">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="97baf-140">Generated service side.</span></span>|
|<span data-ttu-id="97baf-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97baf-141">modifiedDateTime</span></span>|<span data-ttu-id="97baf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97baf-142">DateTimeOffset</span></span>|<span data-ttu-id="97baf-143">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="97baf-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="97baf-144">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="97baf-144">Updated service side.</span></span>|
|<span data-ttu-id="97baf-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="97baf-145">lastSyncDateTime</span></span>|<span data-ttu-id="97baf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97baf-146">DateTimeOffset</span></span>|<span data-ttu-id="97baf-147">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="97baf-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="97baf-148">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="97baf-148">Updated service side.</span></span>|
|<span data-ttu-id="97baf-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="97baf-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="97baf-150">字符串</span><span class="sxs-lookup"><span data-stu-id="97baf-150">String</span></span>|<span data-ttu-id="97baf-151">通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。</span><span class="sxs-lookup"><span data-stu-id="97baf-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="97baf-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="97baf-152">deviceName</span></span>|<span data-ttu-id="97baf-153">String</span><span class="sxs-lookup"><span data-stu-id="97baf-153">String</span></span>|<span data-ttu-id="97baf-154">订阅已的设备名称设置如桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="97baf-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="97baf-155">userName</span><span class="sxs-lookup"><span data-stu-id="97baf-155">userName</span></span>|<span data-ttu-id="97baf-156">String</span><span class="sxs-lookup"><span data-stu-id="97baf-156">String</span></span>|<span data-ttu-id="97baf-157">订阅已设置到例如 joe@contoso.com 用户名</span><span class="sxs-lookup"><span data-stu-id="97baf-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="97baf-158">state</span><span class="sxs-lookup"><span data-stu-id="97baf-158">state</span></span>|[<span data-ttu-id="97baf-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="97baf-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="97baf-160">应用于该设备配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="97baf-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="97baf-161">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="97baf-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="97baf-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="97baf-162">stateDetails</span></span>|<span data-ttu-id="97baf-163">字符串</span><span class="sxs-lookup"><span data-stu-id="97baf-163">String</span></span>|<span data-ttu-id="97baf-164">字符串设置状态的说明。</span><span class="sxs-lookup"><span data-stu-id="97baf-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="97baf-165">响应</span><span class="sxs-lookup"><span data-stu-id="97baf-165">Response</span></span>
<span data-ttu-id="97baf-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97baf-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97baf-167">示例</span><span class="sxs-lookup"><span data-stu-id="97baf-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="97baf-168">请求</span><span class="sxs-lookup"><span data-stu-id="97baf-168">Request</span></span>
<span data-ttu-id="97baf-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97baf-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 300

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="97baf-170">响应</span><span class="sxs-lookup"><span data-stu-id="97baf-170">Response</span></span>
<span data-ttu-id="97baf-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97baf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





