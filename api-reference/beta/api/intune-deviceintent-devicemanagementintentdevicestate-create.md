---
title: 创建 deviceManagementIntentDeviceState
description: 创建新的 deviceManagementIntentDeviceState 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7954b861e82af8aea21283e742ea632813c8f195
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815266"
---
# <a name="create-devicemanagementintentdevicestate"></a><span data-ttu-id="c6a03-103">创建 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="c6a03-103">Create deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="c6a03-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6a03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6a03-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6a03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6a03-106">创建新的[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6a03-106">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6a03-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6a03-107">Prerequisites</span></span>
<span data-ttu-id="c6a03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6a03-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6a03-110">Permission type</span></span>|<span data-ttu-id="c6a03-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6a03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6a03-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6a03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6a03-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6a03-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6a03-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6a03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6a03-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6a03-115">Not supported.</span></span>|
|<span data-ttu-id="c6a03-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6a03-116">Application</span></span>|<span data-ttu-id="c6a03-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6a03-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6a03-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6a03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c6a03-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6a03-119">Request headers</span></span>
|<span data-ttu-id="c6a03-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6a03-120">Header</span></span>|<span data-ttu-id="c6a03-121">值</span><span class="sxs-lookup"><span data-stu-id="c6a03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6a03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6a03-122">Authorization</span></span>|<span data-ttu-id="c6a03-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6a03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6a03-124">接受</span><span class="sxs-lookup"><span data-stu-id="c6a03-124">Accept</span></span>|<span data-ttu-id="c6a03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6a03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6a03-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6a03-126">Request body</span></span>
<span data-ttu-id="c6a03-127">在请求正文中，提供 deviceManagementIntentDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6a03-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceState object.</span></span>

<span data-ttu-id="c6a03-128">下表显示创建 deviceManagementIntentDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6a03-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceState.</span></span>

|<span data-ttu-id="c6a03-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6a03-129">Property</span></span>|<span data-ttu-id="c6a03-130">类型</span><span class="sxs-lookup"><span data-stu-id="c6a03-130">Type</span></span>|<span data-ttu-id="c6a03-131">说明</span><span class="sxs-lookup"><span data-stu-id="c6a03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6a03-132">id</span><span class="sxs-lookup"><span data-stu-id="c6a03-132">id</span></span>|<span data-ttu-id="c6a03-133">String</span><span class="sxs-lookup"><span data-stu-id="c6a03-133">String</span></span>|<span data-ttu-id="c6a03-134">ID</span><span class="sxs-lookup"><span data-stu-id="c6a03-134">The ID</span></span>|
|<span data-ttu-id="c6a03-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6a03-135">userPrincipalName</span></span>|<span data-ttu-id="c6a03-136">String</span><span class="sxs-lookup"><span data-stu-id="c6a03-136">String</span></span>|<span data-ttu-id="c6a03-137">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c6a03-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="c6a03-138">userName</span><span class="sxs-lookup"><span data-stu-id="c6a03-138">userName</span></span>|<span data-ttu-id="c6a03-139">String</span><span class="sxs-lookup"><span data-stu-id="c6a03-139">String</span></span>|<span data-ttu-id="c6a03-140">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="c6a03-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="c6a03-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6a03-141">deviceDisplayName</span></span>|<span data-ttu-id="c6a03-142">String</span><span class="sxs-lookup"><span data-stu-id="c6a03-142">String</span></span>|<span data-ttu-id="c6a03-143">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="c6a03-143">Device name that is being reported</span></span>|
|<span data-ttu-id="c6a03-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6a03-144">lastReportedDateTime</span></span>|<span data-ttu-id="c6a03-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6a03-145">DateTimeOffset</span></span>|<span data-ttu-id="c6a03-146">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="c6a03-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="c6a03-147">state</span><span class="sxs-lookup"><span data-stu-id="c6a03-147">state</span></span>|[<span data-ttu-id="c6a03-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c6a03-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c6a03-149">意图的设备状态。</span><span class="sxs-lookup"><span data-stu-id="c6a03-149">Device state for an intent.</span></span> <span data-ttu-id="c6a03-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="c6a03-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c6a03-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="c6a03-151">deviceId</span></span>|<span data-ttu-id="c6a03-152">String</span><span class="sxs-lookup"><span data-stu-id="c6a03-152">String</span></span>|<span data-ttu-id="c6a03-153">报告的设备 id</span><span class="sxs-lookup"><span data-stu-id="c6a03-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="c6a03-154">响应</span><span class="sxs-lookup"><span data-stu-id="c6a03-154">Response</span></span>
<span data-ttu-id="c6a03-155">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6a03-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6a03-156">示例</span><span class="sxs-lookup"><span data-stu-id="c6a03-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6a03-157">请求</span><span class="sxs-lookup"><span data-stu-id="c6a03-157">Request</span></span>
<span data-ttu-id="c6a03-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6a03-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="c6a03-159">响应</span><span class="sxs-lookup"><span data-stu-id="c6a03-159">Response</span></span>
<span data-ttu-id="c6a03-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6a03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




