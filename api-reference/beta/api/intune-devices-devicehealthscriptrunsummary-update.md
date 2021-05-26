---
title: 更新 deviceHealthScriptRunSummary
description: 更新 deviceHealthScriptRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d342f4703ba8dcb04b58007d26fc94ff99c8c91
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665089"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="2ac92-103">更新 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="2ac92-103">Update deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="2ac92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ac92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ac92-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ac92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ac92-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ac92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac92-107">更新 [deviceHealthScriptRunSummary 对象](../resources/intune-devices-devicehealthscriptrunsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2ac92-107">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ac92-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ac92-108">Prerequisites</span></span>
<span data-ttu-id="2ac92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ac92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ac92-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ac92-111">Permission type</span></span>|<span data-ttu-id="2ac92-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ac92-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ac92-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ac92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ac92-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac92-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ac92-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ac92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ac92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ac92-116">Not supported.</span></span>|
|<span data-ttu-id="2ac92-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ac92-117">Application</span></span>|<span data-ttu-id="2ac92-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac92-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ac92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ac92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="2ac92-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ac92-120">Request headers</span></span>
|<span data-ttu-id="2ac92-121">标头</span><span class="sxs-lookup"><span data-stu-id="2ac92-121">Header</span></span>|<span data-ttu-id="2ac92-122">值</span><span class="sxs-lookup"><span data-stu-id="2ac92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ac92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ac92-123">Authorization</span></span>|<span data-ttu-id="2ac92-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ac92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ac92-125">接受</span><span class="sxs-lookup"><span data-stu-id="2ac92-125">Accept</span></span>|<span data-ttu-id="2ac92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ac92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ac92-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ac92-127">Request body</span></span>
<span data-ttu-id="2ac92-128">在请求正文中，提供 [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ac92-128">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="2ac92-129">下表显示创建 [deviceHealthScriptRunSummary 时所需的属性](../resources/intune-devices-devicehealthscriptrunsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="2ac92-129">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="2ac92-130">属性</span><span class="sxs-lookup"><span data-stu-id="2ac92-130">Property</span></span>|<span data-ttu-id="2ac92-131">类型</span><span class="sxs-lookup"><span data-stu-id="2ac92-131">Type</span></span>|<span data-ttu-id="2ac92-132">说明</span><span class="sxs-lookup"><span data-stu-id="2ac92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac92-133">id</span><span class="sxs-lookup"><span data-stu-id="2ac92-133">id</span></span>|<span data-ttu-id="2ac92-134">String</span><span class="sxs-lookup"><span data-stu-id="2ac92-134">String</span></span>|<span data-ttu-id="2ac92-135">设备运行状况脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="2ac92-135">Key of the device health script run summary entity.</span></span> <span data-ttu-id="2ac92-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2ac92-136">This property is read-only.</span></span>|
|<span data-ttu-id="2ac92-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="2ac92-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-138">Int32</span></span>|<span data-ttu-id="2ac92-139">检测脚本未发现问题且设备正常运行的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-139">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="2ac92-140">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-140">issueDetectedDeviceCount</span></span>|<span data-ttu-id="2ac92-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-141">Int32</span></span>|<span data-ttu-id="2ac92-142">检测脚本发现问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-142">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="2ac92-143">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-143">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="2ac92-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-144">Int32</span></span>|<span data-ttu-id="2ac92-145">检测脚本执行遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-145">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="2ac92-146">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-146">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="2ac92-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-147">Int32</span></span>|<span data-ttu-id="2ac92-148">尚未运行最新版本的设备运行状况脚本的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-148">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="2ac92-149">detectionScriptNotApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-149">detectionScriptNotApplicableDeviceCount</span></span>|<span data-ttu-id="2ac92-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-150">Int32</span></span>|<span data-ttu-id="2ac92-151">检测脚本不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-151">Number of devices for which the detection script was not applicable</span></span>|
|<span data-ttu-id="2ac92-152">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-152">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="2ac92-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-153">Int32</span></span>|<span data-ttu-id="2ac92-154">修正脚本能够解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-154">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="2ac92-155">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-155">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="2ac92-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-156">Int32</span></span>|<span data-ttu-id="2ac92-157">已跳过修正的设备数</span><span class="sxs-lookup"><span data-stu-id="2ac92-157">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="2ac92-158">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-158">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="2ac92-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-159">Int32</span></span>|<span data-ttu-id="2ac92-160">修复脚本成功执行但未能解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-160">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="2ac92-161">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-161">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="2ac92-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-162">Int32</span></span>|<span data-ttu-id="2ac92-163">修正脚本执行遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="2ac92-163">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="2ac92-164">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac92-164">lastScriptRunDateTime</span></span>|<span data-ttu-id="2ac92-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac92-165">DateTimeOffset</span></span>|<span data-ttu-id="2ac92-166">脚本跨所有设备的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="2ac92-166">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="2ac92-167">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ac92-167">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="2ac92-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2ac92-168">Int32</span></span>|<span data-ttu-id="2ac92-169">过去 30 天内修正的设备数</span><span class="sxs-lookup"><span data-stu-id="2ac92-169">Number of devices that were remediated over the last 30 days</span></span>|



## <a name="response"></a><span data-ttu-id="2ac92-170">响应</span><span class="sxs-lookup"><span data-stu-id="2ac92-170">Response</span></span>
<span data-ttu-id="2ac92-171">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ac92-171">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ac92-172">示例</span><span class="sxs-lookup"><span data-stu-id="2ac92-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ac92-173">请求</span><span class="sxs-lookup"><span data-stu-id="2ac92-173">Request</span></span>
<span data-ttu-id="2ac92-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ac92-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a><span data-ttu-id="2ac92-175">响应</span><span class="sxs-lookup"><span data-stu-id="2ac92-175">Response</span></span>
<span data-ttu-id="2ac92-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ac92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```




