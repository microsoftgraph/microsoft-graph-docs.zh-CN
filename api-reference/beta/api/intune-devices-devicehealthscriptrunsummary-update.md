---
title: 更新 deviceHealthScriptRunSummary
description: 更新 deviceHealthScriptRunSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14a05cb7e2c8bb0df57fefedec6331d73e9846fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469466"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="e25b9-103">更新 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e25b9-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="e25b9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e25b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e25b9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e25b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e25b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e25b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e25b9-107">更新[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e25b9-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e25b9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e25b9-108">Prerequisites</span></span>
<span data-ttu-id="e25b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e25b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e25b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e25b9-111">Permission type</span></span>|<span data-ttu-id="e25b9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e25b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e25b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e25b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e25b9-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e25b9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e25b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e25b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e25b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e25b9-116">Not supported.</span></span>|
|<span data-ttu-id="e25b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e25b9-117">Application</span></span>|<span data-ttu-id="e25b9-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e25b9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e25b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e25b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="e25b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e25b9-120">Request headers</span></span>
|<span data-ttu-id="e25b9-121">标头</span><span class="sxs-lookup"><span data-stu-id="e25b9-121">Header</span></span>|<span data-ttu-id="e25b9-122">值</span><span class="sxs-lookup"><span data-stu-id="e25b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e25b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e25b9-123">Authorization</span></span>|<span data-ttu-id="e25b9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e25b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e25b9-125">接受</span><span class="sxs-lookup"><span data-stu-id="e25b9-125">Accept</span></span>|<span data-ttu-id="e25b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e25b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e25b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e25b9-127">Request body</span></span>
<span data-ttu-id="e25b9-128">在请求正文中，提供[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e25b9-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="e25b9-129">下表显示创建[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e25b9-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="e25b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="e25b9-130">Property</span></span>|<span data-ttu-id="e25b9-131">类型</span><span class="sxs-lookup"><span data-stu-id="e25b9-131">Type</span></span>|<span data-ttu-id="e25b9-132">说明</span><span class="sxs-lookup"><span data-stu-id="e25b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e25b9-133">id</span><span class="sxs-lookup"><span data-stu-id="e25b9-133">id</span></span>|<span data-ttu-id="e25b9-134">String</span><span class="sxs-lookup"><span data-stu-id="e25b9-134">String</span></span>|<span data-ttu-id="e25b9-135">设备运行状况脚本的键运行摘要实体。</span><span class="sxs-lookup"><span data-stu-id="e25b9-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="e25b9-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e25b9-136">This property is read-only.</span></span>|
|<span data-ttu-id="e25b9-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="e25b9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-138">Int32</span></span>|<span data-ttu-id="e25b9-139">检测脚本找不到问题且设备正常运行的设备数</span><span class="sxs-lookup"><span data-stu-id="e25b9-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="e25b9-140">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="e25b9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-141">Int32</span></span>|<span data-ttu-id="e25b9-142">检测脚本发现问题的设备数</span><span class="sxs-lookup"><span data-stu-id="e25b9-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="e25b9-143">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="e25b9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-144">Int32</span></span>|<span data-ttu-id="e25b9-145">检测脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="e25b9-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="e25b9-146">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="e25b9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-147">Int32</span></span>|<span data-ttu-id="e25b9-148">尚未运行的设备运行状况脚本的最新版本的设备数量</span><span class="sxs-lookup"><span data-stu-id="e25b9-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="e25b9-149">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-149">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="e25b9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-150">Int32</span></span>|<span data-ttu-id="e25b9-151">修正脚本能够解决检测到的问题的设备数</span><span class="sxs-lookup"><span data-stu-id="e25b9-151">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="e25b9-152">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-152">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="e25b9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-153">Int32</span></span>|<span data-ttu-id="e25b9-154">跳过修正的设备数</span><span class="sxs-lookup"><span data-stu-id="e25b9-154">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="e25b9-155">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-155">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="e25b9-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-156">Int32</span></span>|<span data-ttu-id="e25b9-157">已成功执行修正脚本但未能解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="e25b9-157">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="e25b9-158">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-158">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="e25b9-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-159">Int32</span></span>|<span data-ttu-id="e25b9-160">修正脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="e25b9-160">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="e25b9-161">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="e25b9-161">lastScriptRunDateTime</span></span>|<span data-ttu-id="e25b9-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e25b9-162">DateTimeOffset</span></span>|<span data-ttu-id="e25b9-163">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="e25b9-163">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="e25b9-164">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e25b9-164">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="e25b9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e25b9-165">Int32</span></span>|<span data-ttu-id="e25b9-166">最近30天内修正的设备数量</span><span class="sxs-lookup"><span data-stu-id="e25b9-166">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="e25b9-167">响应</span><span class="sxs-lookup"><span data-stu-id="e25b9-167">Response</span></span>
<span data-ttu-id="e25b9-168">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e25b9-168">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e25b9-169">示例</span><span class="sxs-lookup"><span data-stu-id="e25b9-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="e25b9-170">请求</span><span class="sxs-lookup"><span data-stu-id="e25b9-170">Request</span></span>
<span data-ttu-id="e25b9-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e25b9-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a><span data-ttu-id="e25b9-172">响应</span><span class="sxs-lookup"><span data-stu-id="e25b9-172">Response</span></span>
<span data-ttu-id="e25b9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e25b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```





