---
title: 更新 deviceHealthScriptRunSummary
description: 更新 deviceHealthScriptRunSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 47364fad3d582f576818d69dac8aed9714d5bcf9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531061"
---
# <a name="update-devicehealthscriptrunsummary"></a><span data-ttu-id="19429-103">更新 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="19429-103">Update deviceHealthScriptRunSummary</span></span>

> <span data-ttu-id="19429-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19429-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19429-106">更新[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="19429-106">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19429-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="19429-107">Prerequisites</span></span>
<span data-ttu-id="19429-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19429-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19429-110">Permission type</span></span>|<span data-ttu-id="19429-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="19429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19429-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19429-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19429-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="19429-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19429-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19429-115">Not supported.</span></span>|
|<span data-ttu-id="19429-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19429-116">Application</span></span>|<span data-ttu-id="19429-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19429-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19429-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="19429-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19429-119">Request headers</span></span>
|<span data-ttu-id="19429-120">标头</span><span class="sxs-lookup"><span data-stu-id="19429-120">Header</span></span>|<span data-ttu-id="19429-121">值</span><span class="sxs-lookup"><span data-stu-id="19429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19429-122">授权</span><span class="sxs-lookup"><span data-stu-id="19429-122">Authorization</span></span>|<span data-ttu-id="19429-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="19429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19429-124">接受</span><span class="sxs-lookup"><span data-stu-id="19429-124">Accept</span></span>|<span data-ttu-id="19429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19429-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="19429-126">Request body</span></span>
<span data-ttu-id="19429-127">在请求正文中，提供[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19429-127">In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

<span data-ttu-id="19429-128">下表显示创建[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="19429-128">The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).</span></span>

|<span data-ttu-id="19429-129">属性</span><span class="sxs-lookup"><span data-stu-id="19429-129">Property</span></span>|<span data-ttu-id="19429-130">类型</span><span class="sxs-lookup"><span data-stu-id="19429-130">Type</span></span>|<span data-ttu-id="19429-131">说明</span><span class="sxs-lookup"><span data-stu-id="19429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19429-132">id</span><span class="sxs-lookup"><span data-stu-id="19429-132">id</span></span>|<span data-ttu-id="19429-133">字符串</span><span class="sxs-lookup"><span data-stu-id="19429-133">String</span></span>|<span data-ttu-id="19429-134">设备运行状况脚本的键运行摘要实体。</span><span class="sxs-lookup"><span data-stu-id="19429-134">Key of the device health script run summary entity.</span></span> <span data-ttu-id="19429-135">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="19429-135">This property is read-only.</span></span>|
|<span data-ttu-id="19429-136">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-136">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="19429-137">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-137">Int32</span></span>|<span data-ttu-id="19429-138">检测脚本找不到问题且设备正常运行的设备数</span><span class="sxs-lookup"><span data-stu-id="19429-138">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="19429-139">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-139">issueDetectedDeviceCount</span></span>|<span data-ttu-id="19429-140">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-140">Int32</span></span>|<span data-ttu-id="19429-141">检测脚本发现问题的设备数</span><span class="sxs-lookup"><span data-stu-id="19429-141">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="19429-142">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-142">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="19429-143">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-143">Int32</span></span>|<span data-ttu-id="19429-144">检测脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="19429-144">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="19429-145">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-145">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="19429-146">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-146">Int32</span></span>|<span data-ttu-id="19429-147">尚未运行的设备运行状况脚本的最新版本的设备数量</span><span class="sxs-lookup"><span data-stu-id="19429-147">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="19429-148">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-148">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="19429-149">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-149">Int32</span></span>|<span data-ttu-id="19429-150">修正脚本能够解决检测到的问题的设备数</span><span class="sxs-lookup"><span data-stu-id="19429-150">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="19429-151">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-151">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="19429-152">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-152">Int32</span></span>|<span data-ttu-id="19429-153">跳过修正的设备数</span><span class="sxs-lookup"><span data-stu-id="19429-153">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="19429-154">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-154">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="19429-155">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-155">Int32</span></span>|<span data-ttu-id="19429-156">已成功执行修正脚本但未能解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="19429-156">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="19429-157">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19429-157">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="19429-158">Int32</span><span class="sxs-lookup"><span data-stu-id="19429-158">Int32</span></span>|<span data-ttu-id="19429-159">修正脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="19429-159">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="19429-160">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="19429-160">lastScriptRunDateTime</span></span>|<span data-ttu-id="19429-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19429-161">DateTimeOffset</span></span>|<span data-ttu-id="19429-162">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="19429-162">Last run time for the script across all devices</span></span>|



## <a name="response"></a><span data-ttu-id="19429-163">响应</span><span class="sxs-lookup"><span data-stu-id="19429-163">Response</span></span>
<span data-ttu-id="19429-164">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="19429-164">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19429-165">示例</span><span class="sxs-lookup"><span data-stu-id="19429-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="19429-166">请求</span><span class="sxs-lookup"><span data-stu-id="19429-166">Request</span></span>
<span data-ttu-id="19429-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19429-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 448

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
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a><span data-ttu-id="19429-168">响应</span><span class="sxs-lookup"><span data-stu-id="19429-168">Response</span></span>
<span data-ttu-id="19429-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19429-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

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
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```






