---
title: 更新 deviceCompliancePolicyDeviceStateSummary
description: 更新 deviceCompliancePolicyDeviceStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd58291b1f9dbec8c18449202aa10f461c645b6f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959514"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="63e47-103">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="63e47-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="63e47-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63e47-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e47-105">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="63e47-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63e47-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="63e47-106">Prerequisites</span></span>
<span data-ttu-id="63e47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63e47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63e47-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63e47-109">Permission type</span></span>|<span data-ttu-id="63e47-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63e47-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63e47-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63e47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="63e47-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63e47-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63e47-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63e47-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63e47-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63e47-114">Not supported.</span></span>|
|<span data-ttu-id="63e47-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="63e47-115">Application</span></span>|<span data-ttu-id="63e47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63e47-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63e47-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63e47-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="63e47-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="63e47-118">Request headers</span></span>
|<span data-ttu-id="63e47-119">标头</span><span class="sxs-lookup"><span data-stu-id="63e47-119">Header</span></span>|<span data-ttu-id="63e47-120">值</span><span class="sxs-lookup"><span data-stu-id="63e47-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63e47-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="63e47-121">Authorization</span></span>|<span data-ttu-id="63e47-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63e47-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63e47-123">接受</span><span class="sxs-lookup"><span data-stu-id="63e47-123">Accept</span></span>|<span data-ttu-id="63e47-124">application/json</span><span class="sxs-lookup"><span data-stu-id="63e47-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63e47-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="63e47-125">Request body</span></span>
<span data-ttu-id="63e47-126">在请求正文中，提供 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63e47-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="63e47-127">下表显示了创建 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63e47-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="63e47-128">属性</span><span class="sxs-lookup"><span data-stu-id="63e47-128">Property</span></span>|<span data-ttu-id="63e47-129">类型</span><span class="sxs-lookup"><span data-stu-id="63e47-129">Type</span></span>|<span data-ttu-id="63e47-130">说明</span><span class="sxs-lookup"><span data-stu-id="63e47-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e47-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="63e47-131">inGracePeriodCount</span></span>|<span data-ttu-id="63e47-132">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-132">Int32</span></span>|<span data-ttu-id="63e47-133">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="63e47-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="63e47-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="63e47-134">configManagerCount</span></span>|<span data-ttu-id="63e47-135">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-135">Int32</span></span>|<span data-ttu-id="63e47-136">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="63e47-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="63e47-137">id</span><span class="sxs-lookup"><span data-stu-id="63e47-137">id</span></span>|<span data-ttu-id="63e47-138">String</span><span class="sxs-lookup"><span data-stu-id="63e47-138">String</span></span>|<span data-ttu-id="63e47-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63e47-139">Key of the entity.</span></span>|
|<span data-ttu-id="63e47-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-140">unknownDeviceCount</span></span>|<span data-ttu-id="63e47-141">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-141">Int32</span></span>|<span data-ttu-id="63e47-142">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-142">Number of unknown devices</span></span>|
|<span data-ttu-id="63e47-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="63e47-144">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-144">Int32</span></span>|<span data-ttu-id="63e47-145">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="63e47-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-146">compliantDeviceCount</span></span>|<span data-ttu-id="63e47-147">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-147">Int32</span></span>|<span data-ttu-id="63e47-148">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-148">Number of compliant devices</span></span>|
|<span data-ttu-id="63e47-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-149">remediatedDeviceCount</span></span>|<span data-ttu-id="63e47-150">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-150">Int32</span></span>|<span data-ttu-id="63e47-151">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-151">Number of remediated devices</span></span>|
|<span data-ttu-id="63e47-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="63e47-153">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-153">Int32</span></span>|<span data-ttu-id="63e47-154">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="63e47-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-155">errorDeviceCount</span></span>|<span data-ttu-id="63e47-156">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-156">Int32</span></span>|<span data-ttu-id="63e47-157">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-157">Number of error devices</span></span>|
|<span data-ttu-id="63e47-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63e47-158">conflictDeviceCount</span></span>|<span data-ttu-id="63e47-159">Int32</span><span class="sxs-lookup"><span data-stu-id="63e47-159">Int32</span></span>|<span data-ttu-id="63e47-160">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="63e47-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="63e47-161">响应</span><span class="sxs-lookup"><span data-stu-id="63e47-161">Response</span></span>
<span data-ttu-id="63e47-162">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63e47-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63e47-163">示例</span><span class="sxs-lookup"><span data-stu-id="63e47-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="63e47-164">请求</span><span class="sxs-lookup"><span data-stu-id="63e47-164">Request</span></span>
<span data-ttu-id="63e47-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63e47-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="63e47-166">响应</span><span class="sxs-lookup"><span data-stu-id="63e47-166">Response</span></span>
<span data-ttu-id="63e47-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63e47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



