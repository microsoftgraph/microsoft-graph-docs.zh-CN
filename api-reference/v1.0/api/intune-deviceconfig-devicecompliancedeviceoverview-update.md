---
title: 更新 deviceComplianceDeviceOverview
description: 更新 deviceComplianceDeviceOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1799f4825346643e54065b199adb728023df2a2d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019427"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="80ed0-103">更新 deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="80ed0-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="80ed0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80ed0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80ed0-105">更新 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80ed0-105">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80ed0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="80ed0-106">Prerequisites</span></span>
<span data-ttu-id="80ed0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80ed0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ed0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80ed0-109">Permission type</span></span>|<span data-ttu-id="80ed0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80ed0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80ed0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80ed0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80ed0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ed0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80ed0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80ed0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80ed0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80ed0-114">Not supported.</span></span>|
|<span data-ttu-id="80ed0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80ed0-115">Application</span></span>|<span data-ttu-id="80ed0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80ed0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80ed0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80ed0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="80ed0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80ed0-118">Request headers</span></span>
|<span data-ttu-id="80ed0-119">标头</span><span class="sxs-lookup"><span data-stu-id="80ed0-119">Header</span></span>|<span data-ttu-id="80ed0-120">值</span><span class="sxs-lookup"><span data-stu-id="80ed0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80ed0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80ed0-121">Authorization</span></span>|<span data-ttu-id="80ed0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80ed0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80ed0-123">接受</span><span class="sxs-lookup"><span data-stu-id="80ed0-123">Accept</span></span>|<span data-ttu-id="80ed0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80ed0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ed0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80ed0-125">Request body</span></span>
<span data-ttu-id="80ed0-126">在请求正文中，提供 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80ed0-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="80ed0-127">下表显示创建 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80ed0-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="80ed0-128">属性</span><span class="sxs-lookup"><span data-stu-id="80ed0-128">Property</span></span>|<span data-ttu-id="80ed0-129">类型</span><span class="sxs-lookup"><span data-stu-id="80ed0-129">Type</span></span>|<span data-ttu-id="80ed0-130">说明</span><span class="sxs-lookup"><span data-stu-id="80ed0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80ed0-131">id</span><span class="sxs-lookup"><span data-stu-id="80ed0-131">id</span></span>|<span data-ttu-id="80ed0-132">String</span><span class="sxs-lookup"><span data-stu-id="80ed0-132">String</span></span>|<span data-ttu-id="80ed0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80ed0-133">Key of the entity.</span></span>|
|<span data-ttu-id="80ed0-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="80ed0-134">pendingCount</span></span>|<span data-ttu-id="80ed0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="80ed0-135">Int32</span></span>|<span data-ttu-id="80ed0-136">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="80ed0-136">Number of pending devices</span></span>|
|<span data-ttu-id="80ed0-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="80ed0-137">notApplicableCount</span></span>|<span data-ttu-id="80ed0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="80ed0-138">Int32</span></span>|<span data-ttu-id="80ed0-139">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="80ed0-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="80ed0-140">successCount</span><span class="sxs-lookup"><span data-stu-id="80ed0-140">successCount</span></span>|<span data-ttu-id="80ed0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="80ed0-141">Int32</span></span>|<span data-ttu-id="80ed0-142">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="80ed0-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="80ed0-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="80ed0-143">errorCount</span></span>|<span data-ttu-id="80ed0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="80ed0-144">Int32</span></span>|<span data-ttu-id="80ed0-145">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="80ed0-145">Number of error devices</span></span>|
|<span data-ttu-id="80ed0-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="80ed0-146">failedCount</span></span>|<span data-ttu-id="80ed0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="80ed0-147">Int32</span></span>|<span data-ttu-id="80ed0-148">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="80ed0-148">Number of failed devices</span></span>|
|<span data-ttu-id="80ed0-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="80ed0-149">lastUpdateDateTime</span></span>|<span data-ttu-id="80ed0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80ed0-150">DateTimeOffset</span></span>|<span data-ttu-id="80ed0-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="80ed0-151">Last update time</span></span>|
|<span data-ttu-id="80ed0-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="80ed0-152">configurationVersion</span></span>|<span data-ttu-id="80ed0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="80ed0-153">Int32</span></span>|<span data-ttu-id="80ed0-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="80ed0-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="80ed0-155">响应</span><span class="sxs-lookup"><span data-stu-id="80ed0-155">Response</span></span>
<span data-ttu-id="80ed0-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80ed0-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80ed0-157">示例</span><span class="sxs-lookup"><span data-stu-id="80ed0-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="80ed0-158">请求</span><span class="sxs-lookup"><span data-stu-id="80ed0-158">Request</span></span>
<span data-ttu-id="80ed0-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80ed0-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="80ed0-160">响应</span><span class="sxs-lookup"><span data-stu-id="80ed0-160">Response</span></span>
<span data-ttu-id="80ed0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80ed0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



