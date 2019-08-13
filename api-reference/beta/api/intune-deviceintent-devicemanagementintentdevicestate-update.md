---
title: 更新 deviceManagementIntentDeviceState
description: 更新 deviceManagementIntentDeviceState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4e23abab9d3bc7b3ca61ba4946b2ed2d4afc625
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343557"
---
# <a name="update-devicemanagementintentdevicestate"></a><span data-ttu-id="c93a4-103">更新 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="c93a4-103">Update deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="c93a4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c93a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c93a4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c93a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c93a4-106">更新[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c93a4-106">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c93a4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c93a4-107">Prerequisites</span></span>
<span data-ttu-id="c93a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c93a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c93a4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c93a4-110">Permission type</span></span>|<span data-ttu-id="c93a4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c93a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c93a4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c93a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c93a4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c93a4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c93a4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c93a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c93a4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c93a4-115">Not supported.</span></span>|
|<span data-ttu-id="c93a4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c93a4-116">Application</span></span>|<span data-ttu-id="c93a4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c93a4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c93a4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c93a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c93a4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c93a4-119">Request headers</span></span>
|<span data-ttu-id="c93a4-120">标头</span><span class="sxs-lookup"><span data-stu-id="c93a4-120">Header</span></span>|<span data-ttu-id="c93a4-121">值</span><span class="sxs-lookup"><span data-stu-id="c93a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c93a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c93a4-122">Authorization</span></span>|<span data-ttu-id="c93a4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c93a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c93a4-124">接受</span><span class="sxs-lookup"><span data-stu-id="c93a4-124">Accept</span></span>|<span data-ttu-id="c93a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c93a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c93a4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c93a4-126">Request body</span></span>
<span data-ttu-id="c93a4-127">在请求正文中, 提供[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c93a4-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

<span data-ttu-id="c93a4-128">下表显示创建[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c93a4-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>

|<span data-ttu-id="c93a4-129">属性</span><span class="sxs-lookup"><span data-stu-id="c93a4-129">Property</span></span>|<span data-ttu-id="c93a4-130">类型</span><span class="sxs-lookup"><span data-stu-id="c93a4-130">Type</span></span>|<span data-ttu-id="c93a4-131">说明</span><span class="sxs-lookup"><span data-stu-id="c93a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c93a4-132">id</span><span class="sxs-lookup"><span data-stu-id="c93a4-132">id</span></span>|<span data-ttu-id="c93a4-133">String</span><span class="sxs-lookup"><span data-stu-id="c93a4-133">String</span></span>|<span data-ttu-id="c93a4-134">ID</span><span class="sxs-lookup"><span data-stu-id="c93a4-134">The ID</span></span>|
|<span data-ttu-id="c93a4-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c93a4-135">userPrincipalName</span></span>|<span data-ttu-id="c93a4-136">String</span><span class="sxs-lookup"><span data-stu-id="c93a4-136">String</span></span>|<span data-ttu-id="c93a4-137">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c93a4-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="c93a4-138">userName</span><span class="sxs-lookup"><span data-stu-id="c93a4-138">userName</span></span>|<span data-ttu-id="c93a4-139">String</span><span class="sxs-lookup"><span data-stu-id="c93a4-139">String</span></span>|<span data-ttu-id="c93a4-140">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="c93a4-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="c93a4-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c93a4-141">deviceDisplayName</span></span>|<span data-ttu-id="c93a4-142">String</span><span class="sxs-lookup"><span data-stu-id="c93a4-142">String</span></span>|<span data-ttu-id="c93a4-143">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="c93a4-143">Device name that is being reported</span></span>|
|<span data-ttu-id="c93a4-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c93a4-144">lastReportedDateTime</span></span>|<span data-ttu-id="c93a4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c93a4-145">DateTimeOffset</span></span>|<span data-ttu-id="c93a4-146">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="c93a4-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="c93a4-147">state</span><span class="sxs-lookup"><span data-stu-id="c93a4-147">state</span></span>|[<span data-ttu-id="c93a4-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c93a4-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c93a4-149">意图的设备状态。</span><span class="sxs-lookup"><span data-stu-id="c93a4-149">Device state for an intent.</span></span> <span data-ttu-id="c93a4-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="c93a4-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c93a4-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="c93a4-151">deviceId</span></span>|<span data-ttu-id="c93a4-152">String</span><span class="sxs-lookup"><span data-stu-id="c93a4-152">String</span></span>|<span data-ttu-id="c93a4-153">报告的设备 id</span><span class="sxs-lookup"><span data-stu-id="c93a4-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="c93a4-154">响应</span><span class="sxs-lookup"><span data-stu-id="c93a4-154">Response</span></span>
<span data-ttu-id="c93a4-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c93a4-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c93a4-156">示例</span><span class="sxs-lookup"><span data-stu-id="c93a4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="c93a4-157">请求</span><span class="sxs-lookup"><span data-stu-id="c93a4-157">Request</span></span>
<span data-ttu-id="c93a4-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c93a4-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="c93a4-159">响应</span><span class="sxs-lookup"><span data-stu-id="c93a4-159">Response</span></span>
<span data-ttu-id="c93a4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c93a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "8db75881-5881-8db7-8158-b78d8158b78d",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```






