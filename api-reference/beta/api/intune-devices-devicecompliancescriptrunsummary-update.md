---
title: 更新 deviceComplianceScriptRunSummary
description: 更新 deviceComplianceScriptRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05734a63702ee3fe284484c138211bcdafae29ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728737"
---
# <a name="update-devicecompliancescriptrunsummary"></a><span data-ttu-id="7e2df-103">更新 deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="7e2df-103">Update deviceComplianceScriptRunSummary</span></span>

<span data-ttu-id="7e2df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e2df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e2df-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e2df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e2df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e2df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e2df-107">更新 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e2df-107">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e2df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7e2df-108">Prerequisites</span></span>
<span data-ttu-id="7e2df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e2df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e2df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e2df-111">Permission type</span></span>|<span data-ttu-id="7e2df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7e2df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e2df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e2df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2df-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2df-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7e2df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e2df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e2df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e2df-116">Not supported.</span></span>|
|<span data-ttu-id="7e2df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e2df-117">Application</span></span>|<span data-ttu-id="7e2df-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2df-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e2df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="7e2df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e2df-120">Request headers</span></span>
|<span data-ttu-id="7e2df-121">标头</span><span class="sxs-lookup"><span data-stu-id="7e2df-121">Header</span></span>|<span data-ttu-id="7e2df-122">值</span><span class="sxs-lookup"><span data-stu-id="7e2df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e2df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e2df-123">Authorization</span></span>|<span data-ttu-id="7e2df-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7e2df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e2df-125">接受</span><span class="sxs-lookup"><span data-stu-id="7e2df-125">Accept</span></span>|<span data-ttu-id="7e2df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e2df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e2df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e2df-127">Request body</span></span>
<span data-ttu-id="7e2df-128">在请求正文中，提供 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e2df-128">In the request body, supply a JSON representation for the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

<span data-ttu-id="7e2df-129">下表显示创建 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7e2df-129">The following table shows the properties that are required when you create the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span></span>

|<span data-ttu-id="7e2df-130">属性</span><span class="sxs-lookup"><span data-stu-id="7e2df-130">Property</span></span>|<span data-ttu-id="7e2df-131">类型</span><span class="sxs-lookup"><span data-stu-id="7e2df-131">Type</span></span>|<span data-ttu-id="7e2df-132">说明</span><span class="sxs-lookup"><span data-stu-id="7e2df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2df-133">id</span><span class="sxs-lookup"><span data-stu-id="7e2df-133">id</span></span>|<span data-ttu-id="7e2df-134">String</span><span class="sxs-lookup"><span data-stu-id="7e2df-134">String</span></span>|<span data-ttu-id="7e2df-135">设备符合性脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="7e2df-135">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="7e2df-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7e2df-136">This property is read-only.</span></span>|
|<span data-ttu-id="7e2df-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2df-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="7e2df-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2df-138">Int32</span></span>|<span data-ttu-id="7e2df-139">检测脚本找不到问题且设备正常运行的设备数量。</span><span class="sxs-lookup"><span data-stu-id="7e2df-139">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="7e2df-140">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="7e2df-140">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7e2df-141">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2df-141">issueDetectedDeviceCount</span></span>|<span data-ttu-id="7e2df-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2df-142">Int32</span></span>|<span data-ttu-id="7e2df-143">检测脚本发现问题的设备数。</span><span class="sxs-lookup"><span data-stu-id="7e2df-143">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="7e2df-144">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="7e2df-144">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7e2df-145">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2df-145">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="7e2df-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2df-146">Int32</span></span>|<span data-ttu-id="7e2df-147">检测脚本执行时遇到错误且未完成的设备数量。</span><span class="sxs-lookup"><span data-stu-id="7e2df-147">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="7e2df-148">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="7e2df-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7e2df-149">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e2df-149">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="7e2df-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2df-150">Int32</span></span>|<span data-ttu-id="7e2df-151">尚未运行的设备符合性脚本的最新版本的设备数量。</span><span class="sxs-lookup"><span data-stu-id="7e2df-151">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="7e2df-152">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="7e2df-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7e2df-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="7e2df-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="7e2df-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e2df-154">DateTimeOffset</span></span>|<span data-ttu-id="7e2df-155">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="7e2df-155">Last run time for the script across all devices</span></span>|



## <a name="response"></a><span data-ttu-id="7e2df-156">响应</span><span class="sxs-lookup"><span data-stu-id="7e2df-156">Response</span></span>
<span data-ttu-id="7e2df-157">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e2df-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2df-158">示例</span><span class="sxs-lookup"><span data-stu-id="7e2df-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e2df-159">请求</span><span class="sxs-lookup"><span data-stu-id="7e2df-159">Request</span></span>
<span data-ttu-id="7e2df-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e2df-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a><span data-ttu-id="7e2df-161">响应</span><span class="sxs-lookup"><span data-stu-id="7e2df-161">Response</span></span>
<span data-ttu-id="7e2df-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e2df-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```





