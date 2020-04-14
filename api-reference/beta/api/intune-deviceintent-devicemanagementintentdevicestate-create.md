---
title: 创建 deviceManagementIntentDeviceState
description: 创建新的 deviceManagementIntentDeviceState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f7e97cfe24e28fcc2cf8c423ab94fa14d707518
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326496"
---
# <a name="create-devicemanagementintentdevicestate"></a><span data-ttu-id="898d5-103">创建 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="898d5-103">Create deviceManagementIntentDeviceState</span></span>

<span data-ttu-id="898d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="898d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="898d5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="898d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="898d5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="898d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="898d5-107">创建新的[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="898d5-107">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="898d5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="898d5-108">Prerequisites</span></span>
<span data-ttu-id="898d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="898d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="898d5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="898d5-111">Permission type</span></span>|<span data-ttu-id="898d5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="898d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="898d5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="898d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="898d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="898d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="898d5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="898d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="898d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="898d5-116">Not supported.</span></span>|
|<span data-ttu-id="898d5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="898d5-117">Application</span></span>|<span data-ttu-id="898d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="898d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="898d5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="898d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="898d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="898d5-120">Request headers</span></span>
|<span data-ttu-id="898d5-121">标头</span><span class="sxs-lookup"><span data-stu-id="898d5-121">Header</span></span>|<span data-ttu-id="898d5-122">值</span><span class="sxs-lookup"><span data-stu-id="898d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="898d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="898d5-123">Authorization</span></span>|<span data-ttu-id="898d5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="898d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="898d5-125">接受</span><span class="sxs-lookup"><span data-stu-id="898d5-125">Accept</span></span>|<span data-ttu-id="898d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="898d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="898d5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="898d5-127">Request body</span></span>
<span data-ttu-id="898d5-128">在请求正文中，提供 deviceManagementIntentDeviceState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="898d5-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceState object.</span></span>

<span data-ttu-id="898d5-129">下表显示创建 deviceManagementIntentDeviceState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="898d5-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceState.</span></span>

|<span data-ttu-id="898d5-130">属性</span><span class="sxs-lookup"><span data-stu-id="898d5-130">Property</span></span>|<span data-ttu-id="898d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="898d5-131">Type</span></span>|<span data-ttu-id="898d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="898d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="898d5-133">id</span><span class="sxs-lookup"><span data-stu-id="898d5-133">id</span></span>|<span data-ttu-id="898d5-134">String</span><span class="sxs-lookup"><span data-stu-id="898d5-134">String</span></span>|<span data-ttu-id="898d5-135">ID</span><span class="sxs-lookup"><span data-stu-id="898d5-135">The ID</span></span>|
|<span data-ttu-id="898d5-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="898d5-136">userPrincipalName</span></span>|<span data-ttu-id="898d5-137">字符串</span><span class="sxs-lookup"><span data-stu-id="898d5-137">String</span></span>|<span data-ttu-id="898d5-138">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="898d5-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="898d5-139">userName</span><span class="sxs-lookup"><span data-stu-id="898d5-139">userName</span></span>|<span data-ttu-id="898d5-140">字符串</span><span class="sxs-lookup"><span data-stu-id="898d5-140">String</span></span>|<span data-ttu-id="898d5-141">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="898d5-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="898d5-142">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="898d5-142">deviceDisplayName</span></span>|<span data-ttu-id="898d5-143">String</span><span class="sxs-lookup"><span data-stu-id="898d5-143">String</span></span>|<span data-ttu-id="898d5-144">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="898d5-144">Device name that is being reported</span></span>|
|<span data-ttu-id="898d5-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="898d5-145">lastReportedDateTime</span></span>|<span data-ttu-id="898d5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="898d5-146">DateTimeOffset</span></span>|<span data-ttu-id="898d5-147">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="898d5-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="898d5-148">state</span><span class="sxs-lookup"><span data-stu-id="898d5-148">state</span></span>|[<span data-ttu-id="898d5-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="898d5-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="898d5-150">意图的设备状态。</span><span class="sxs-lookup"><span data-stu-id="898d5-150">Device state for an intent.</span></span> <span data-ttu-id="898d5-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="898d5-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="898d5-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="898d5-152">deviceId</span></span>|<span data-ttu-id="898d5-153">字符串</span><span class="sxs-lookup"><span data-stu-id="898d5-153">String</span></span>|<span data-ttu-id="898d5-154">报告的设备 id</span><span class="sxs-lookup"><span data-stu-id="898d5-154">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="898d5-155">响应</span><span class="sxs-lookup"><span data-stu-id="898d5-155">Response</span></span>
<span data-ttu-id="898d5-156">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="898d5-156">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="898d5-157">示例</span><span class="sxs-lookup"><span data-stu-id="898d5-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="898d5-158">请求</span><span class="sxs-lookup"><span data-stu-id="898d5-158">Request</span></span>
<span data-ttu-id="898d5-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="898d5-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="898d5-160">响应</span><span class="sxs-lookup"><span data-stu-id="898d5-160">Response</span></span>
<span data-ttu-id="898d5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="898d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



