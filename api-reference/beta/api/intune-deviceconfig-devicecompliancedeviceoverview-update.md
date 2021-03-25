---
title: 更新 deviceComplianceDeviceOverview
description: 更新 deviceComplianceDeviceOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9c83e4fe6c32b3115ff66c5178446a317ffa382
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155594"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="4d20f-103">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="4d20f-103">Update deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="4d20f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d20f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d20f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d20f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d20f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d20f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d20f-107">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d20f-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d20f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d20f-108">Prerequisites</span></span>
<span data-ttu-id="4d20f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d20f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d20f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d20f-111">Permission type</span></span>|<span data-ttu-id="4d20f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d20f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d20f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d20f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d20f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d20f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d20f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d20f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d20f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d20f-116">Not supported.</span></span>|
|<span data-ttu-id="4d20f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d20f-117">Application</span></span>|<span data-ttu-id="4d20f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d20f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d20f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d20f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="4d20f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d20f-120">Request headers</span></span>
|<span data-ttu-id="4d20f-121">标头</span><span class="sxs-lookup"><span data-stu-id="4d20f-121">Header</span></span>|<span data-ttu-id="4d20f-122">值</span><span class="sxs-lookup"><span data-stu-id="4d20f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d20f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d20f-123">Authorization</span></span>|<span data-ttu-id="4d20f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d20f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d20f-125">接受</span><span class="sxs-lookup"><span data-stu-id="4d20f-125">Accept</span></span>|<span data-ttu-id="4d20f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d20f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d20f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d20f-127">Request body</span></span>
<span data-ttu-id="4d20f-128">在请求正文中，提供 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d20f-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="4d20f-129">下表显示创建 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d20f-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="4d20f-130">属性</span><span class="sxs-lookup"><span data-stu-id="4d20f-130">Property</span></span>|<span data-ttu-id="4d20f-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d20f-131">Type</span></span>|<span data-ttu-id="4d20f-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d20f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d20f-133">id</span><span class="sxs-lookup"><span data-stu-id="4d20f-133">id</span></span>|<span data-ttu-id="4d20f-134">String</span><span class="sxs-lookup"><span data-stu-id="4d20f-134">String</span></span>|<span data-ttu-id="4d20f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d20f-135">Key of the entity.</span></span>|
|<span data-ttu-id="4d20f-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-136">pendingCount</span></span>|<span data-ttu-id="4d20f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-137">Int32</span></span>|<span data-ttu-id="4d20f-138">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d20f-138">Number of pending devices</span></span>|
|<span data-ttu-id="4d20f-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-139">notApplicableCount</span></span>|<span data-ttu-id="4d20f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-140">Int32</span></span>|<span data-ttu-id="4d20f-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d20f-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="4d20f-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="4d20f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-143">Int32</span></span>|<span data-ttu-id="4d20f-144">由于平台和策略不匹配而不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="4d20f-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="4d20f-145">successCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-145">successCount</span></span>|<span data-ttu-id="4d20f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-146">Int32</span></span>|<span data-ttu-id="4d20f-147">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d20f-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="4d20f-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-148">errorCount</span></span>|<span data-ttu-id="4d20f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-149">Int32</span></span>|<span data-ttu-id="4d20f-150">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d20f-150">Number of error devices</span></span>|
|<span data-ttu-id="4d20f-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-151">failedCount</span></span>|<span data-ttu-id="4d20f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-152">Int32</span></span>|<span data-ttu-id="4d20f-153">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d20f-153">Number of failed devices</span></span>|
|<span data-ttu-id="4d20f-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4d20f-154">conflictCount</span></span>|<span data-ttu-id="4d20f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-155">Int32</span></span>|<span data-ttu-id="4d20f-156">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="4d20f-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="4d20f-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4d20f-157">lastUpdateDateTime</span></span>|<span data-ttu-id="4d20f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d20f-158">DateTimeOffset</span></span>|<span data-ttu-id="4d20f-159">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="4d20f-159">Last update time</span></span>|
|<span data-ttu-id="4d20f-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4d20f-160">configurationVersion</span></span>|<span data-ttu-id="4d20f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4d20f-161">Int32</span></span>|<span data-ttu-id="4d20f-162">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="4d20f-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4d20f-163">响应</span><span class="sxs-lookup"><span data-stu-id="4d20f-163">Response</span></span>
<span data-ttu-id="4d20f-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d20f-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d20f-165">示例</span><span class="sxs-lookup"><span data-stu-id="4d20f-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d20f-166">请求</span><span class="sxs-lookup"><span data-stu-id="4d20f-166">Request</span></span>
<span data-ttu-id="4d20f-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d20f-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="4d20f-168">响应</span><span class="sxs-lookup"><span data-stu-id="4d20f-168">Response</span></span>
<span data-ttu-id="4d20f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d20f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




