---
title: 更新 deviceComplianceDeviceOverview
description: 更新 deviceComplianceDeviceOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d09535f2309370984834d150c8aa55cbe436256
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174366"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="92e9a-103">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="92e9a-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="92e9a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92e9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e9a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92e9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e9a-106">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="92e9a-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e9a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="92e9a-107">Prerequisites</span></span>
<span data-ttu-id="92e9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="92e9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="92e9a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="92e9a-110">Permission type</span></span>|<span data-ttu-id="92e9a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92e9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e9a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92e9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92e9a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e9a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92e9a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92e9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e9a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e9a-115">Not supported.</span></span>|
|<span data-ttu-id="92e9a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92e9a-116">Application</span></span>|<span data-ttu-id="92e9a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e9a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e9a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92e9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="92e9a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="92e9a-119">Request headers</span></span>
|<span data-ttu-id="92e9a-120">标头</span><span class="sxs-lookup"><span data-stu-id="92e9a-120">Header</span></span>|<span data-ttu-id="92e9a-121">值</span><span class="sxs-lookup"><span data-stu-id="92e9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e9a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92e9a-122">Authorization</span></span>|<span data-ttu-id="92e9a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92e9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e9a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92e9a-124">Accept</span></span>|<span data-ttu-id="92e9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92e9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e9a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="92e9a-126">Request body</span></span>
<span data-ttu-id="92e9a-127">在请求正文中，提供 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92e9a-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="92e9a-128">下表显示创建 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92e9a-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="92e9a-129">属性</span><span class="sxs-lookup"><span data-stu-id="92e9a-129">Property</span></span>|<span data-ttu-id="92e9a-130">类型</span><span class="sxs-lookup"><span data-stu-id="92e9a-130">Type</span></span>|<span data-ttu-id="92e9a-131">说明</span><span class="sxs-lookup"><span data-stu-id="92e9a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e9a-132">id</span><span class="sxs-lookup"><span data-stu-id="92e9a-132">id</span></span>|<span data-ttu-id="92e9a-133">String</span><span class="sxs-lookup"><span data-stu-id="92e9a-133">String</span></span>|<span data-ttu-id="92e9a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="92e9a-134">Key of the entity.</span></span>|
|<span data-ttu-id="92e9a-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-135">pendingCount</span></span>|<span data-ttu-id="92e9a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-136">Int32</span></span>|<span data-ttu-id="92e9a-137">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="92e9a-137">Number of pending devices</span></span>|
|<span data-ttu-id="92e9a-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-138">notApplicableCount</span></span>|<span data-ttu-id="92e9a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-139">Int32</span></span>|<span data-ttu-id="92e9a-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="92e9a-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="92e9a-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="92e9a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-142">Int32</span></span>|<span data-ttu-id="92e9a-143">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="92e9a-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="92e9a-144">successCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-144">successCount</span></span>|<span data-ttu-id="92e9a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-145">Int32</span></span>|<span data-ttu-id="92e9a-146">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="92e9a-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="92e9a-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-147">errorCount</span></span>|<span data-ttu-id="92e9a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-148">Int32</span></span>|<span data-ttu-id="92e9a-149">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="92e9a-149">Number of error devices</span></span>|
|<span data-ttu-id="92e9a-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-150">failedCount</span></span>|<span data-ttu-id="92e9a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-151">Int32</span></span>|<span data-ttu-id="92e9a-152">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="92e9a-152">Number of failed devices</span></span>|
|<span data-ttu-id="92e9a-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="92e9a-153">conflictCount</span></span>|<span data-ttu-id="92e9a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-154">Int32</span></span>|<span data-ttu-id="92e9a-155">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="92e9a-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="92e9a-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="92e9a-156">lastUpdateDateTime</span></span>|<span data-ttu-id="92e9a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e9a-157">DateTimeOffset</span></span>|<span data-ttu-id="92e9a-158">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="92e9a-158">Last update time</span></span>|
|<span data-ttu-id="92e9a-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="92e9a-159">configurationVersion</span></span>|<span data-ttu-id="92e9a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="92e9a-160">Int32</span></span>|<span data-ttu-id="92e9a-161">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="92e9a-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="92e9a-162">响应</span><span class="sxs-lookup"><span data-stu-id="92e9a-162">Response</span></span>
<span data-ttu-id="92e9a-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92e9a-163">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e9a-164">示例</span><span class="sxs-lookup"><span data-stu-id="92e9a-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e9a-165">请求</span><span class="sxs-lookup"><span data-stu-id="92e9a-165">Request</span></span>
<span data-ttu-id="92e9a-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92e9a-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92e9a-167">响应</span><span class="sxs-lookup"><span data-stu-id="92e9a-167">Response</span></span>
<span data-ttu-id="92e9a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92e9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




