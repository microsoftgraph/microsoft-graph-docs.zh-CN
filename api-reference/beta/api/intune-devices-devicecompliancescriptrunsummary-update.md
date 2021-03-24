---
title: 更新 deviceComplianceScriptRunSummary
description: 更新 deviceComplianceScriptRunSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bbd7d35373caaaf9a463955fa3de09025839e38
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130761"
---
# <a name="update-devicecompliancescriptrunsummary"></a><span data-ttu-id="176f6-103">更新 deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="176f6-103">Update deviceComplianceScriptRunSummary</span></span>

<span data-ttu-id="176f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="176f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="176f6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="176f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="176f6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="176f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="176f6-107">更新 [deviceComplianceScriptRunSummary 对象](../resources/intune-devices-devicecompliancescriptrunsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="176f6-107">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="176f6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="176f6-108">Prerequisites</span></span>
<span data-ttu-id="176f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="176f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="176f6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="176f6-111">Permission type</span></span>|<span data-ttu-id="176f6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="176f6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="176f6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="176f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="176f6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176f6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="176f6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="176f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="176f6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="176f6-116">Not supported.</span></span>|
|<span data-ttu-id="176f6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="176f6-117">Application</span></span>|<span data-ttu-id="176f6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176f6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="176f6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="176f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="176f6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="176f6-120">Request headers</span></span>
|<span data-ttu-id="176f6-121">标头</span><span class="sxs-lookup"><span data-stu-id="176f6-121">Header</span></span>|<span data-ttu-id="176f6-122">值</span><span class="sxs-lookup"><span data-stu-id="176f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="176f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="176f6-123">Authorization</span></span>|<span data-ttu-id="176f6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="176f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="176f6-125">接受</span><span class="sxs-lookup"><span data-stu-id="176f6-125">Accept</span></span>|<span data-ttu-id="176f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="176f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="176f6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="176f6-127">Request body</span></span>
<span data-ttu-id="176f6-128">在请求正文中，提供 [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="176f6-128">In the request body, supply a JSON representation for the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

<span data-ttu-id="176f6-129">下表显示创建 [deviceComplianceScriptRunSummary 时所需的属性](../resources/intune-devices-devicecompliancescriptrunsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="176f6-129">The following table shows the properties that are required when you create the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span></span>

|<span data-ttu-id="176f6-130">属性</span><span class="sxs-lookup"><span data-stu-id="176f6-130">Property</span></span>|<span data-ttu-id="176f6-131">类型</span><span class="sxs-lookup"><span data-stu-id="176f6-131">Type</span></span>|<span data-ttu-id="176f6-132">说明</span><span class="sxs-lookup"><span data-stu-id="176f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176f6-133">id</span><span class="sxs-lookup"><span data-stu-id="176f6-133">id</span></span>|<span data-ttu-id="176f6-134">String</span><span class="sxs-lookup"><span data-stu-id="176f6-134">String</span></span>|<span data-ttu-id="176f6-135">设备合规性脚本运行摘要实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="176f6-135">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="176f6-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="176f6-136">This property is read-only.</span></span>|
|<span data-ttu-id="176f6-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="176f6-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="176f6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="176f6-138">Int32</span></span>|<span data-ttu-id="176f6-139">检测脚本未发现问题且设备正常运行的设备数量。</span><span class="sxs-lookup"><span data-stu-id="176f6-139">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="176f6-140">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="176f6-140">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="176f6-141">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="176f6-141">issueDetectedDeviceCount</span></span>|<span data-ttu-id="176f6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="176f6-142">Int32</span></span>|<span data-ttu-id="176f6-143">检测脚本发现问题的设备数量。</span><span class="sxs-lookup"><span data-stu-id="176f6-143">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="176f6-144">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="176f6-144">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="176f6-145">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="176f6-145">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="176f6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="176f6-146">Int32</span></span>|<span data-ttu-id="176f6-147">检测脚本执行遇到错误且未完成的设备数量。</span><span class="sxs-lookup"><span data-stu-id="176f6-147">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="176f6-148">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="176f6-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="176f6-149">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="176f6-149">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="176f6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="176f6-150">Int32</span></span>|<span data-ttu-id="176f6-151">尚未运行最新版本的设备合规性脚本的设备数量。</span><span class="sxs-lookup"><span data-stu-id="176f6-151">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="176f6-152">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="176f6-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="176f6-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="176f6-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="176f6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="176f6-154">DateTimeOffset</span></span>|<span data-ttu-id="176f6-155">脚本跨所有设备的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="176f6-155">Last run time for the script across all devices</span></span>|



## <a name="response"></a><span data-ttu-id="176f6-156">响应</span><span class="sxs-lookup"><span data-stu-id="176f6-156">Response</span></span>
<span data-ttu-id="176f6-157">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="176f6-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="176f6-158">示例</span><span class="sxs-lookup"><span data-stu-id="176f6-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="176f6-159">请求</span><span class="sxs-lookup"><span data-stu-id="176f6-159">Request</span></span>
<span data-ttu-id="176f6-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="176f6-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="176f6-161">响应</span><span class="sxs-lookup"><span data-stu-id="176f6-161">Response</span></span>
<span data-ttu-id="176f6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="176f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




