---
title: 更新 deviceCompliancePolicyDeviceStateSummary
description: 更新 deviceCompliancePolicyDeviceStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e1e7d65eff1bb02669abc7fbd8b3ab6b149acfa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748430"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="6d2d7-103">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="6d2d7-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="6d2d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d2d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d2d7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d2d7-106">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d2d7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d2d7-107">Prerequisites</span></span>
<span data-ttu-id="6d2d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d2d7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d2d7-110">Permission type</span></span>|<span data-ttu-id="6d2d7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d2d7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d2d7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d2d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d2d7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2d7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d2d7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d2d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d2d7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-115">Not supported.</span></span>|
|<span data-ttu-id="6d2d7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d2d7-116">Application</span></span>|<span data-ttu-id="6d2d7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2d7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d2d7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d2d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="6d2d7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d2d7-119">Request headers</span></span>
|<span data-ttu-id="6d2d7-120">标头</span><span class="sxs-lookup"><span data-stu-id="6d2d7-120">Header</span></span>|<span data-ttu-id="6d2d7-121">值</span><span class="sxs-lookup"><span data-stu-id="6d2d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d2d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d2d7-122">Authorization</span></span>|<span data-ttu-id="6d2d7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d2d7-124">接受</span><span class="sxs-lookup"><span data-stu-id="6d2d7-124">Accept</span></span>|<span data-ttu-id="6d2d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d2d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d2d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d2d7-126">Request body</span></span>
<span data-ttu-id="6d2d7-127">在请求正文中，提供 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="6d2d7-128">下表显示了创建 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="6d2d7-129">属性</span><span class="sxs-lookup"><span data-stu-id="6d2d7-129">Property</span></span>|<span data-ttu-id="6d2d7-130">类型</span><span class="sxs-lookup"><span data-stu-id="6d2d7-130">Type</span></span>|<span data-ttu-id="6d2d7-131">说明</span><span class="sxs-lookup"><span data-stu-id="6d2d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d2d7-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-132">inGracePeriodCount</span></span>|<span data-ttu-id="6d2d7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-133">Int32</span></span>|<span data-ttu-id="6d2d7-134">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="6d2d7-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="6d2d7-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-135">configManagerCount</span></span>|<span data-ttu-id="6d2d7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-136">Int32</span></span>|<span data-ttu-id="6d2d7-137">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="6d2d7-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="6d2d7-138">id</span><span class="sxs-lookup"><span data-stu-id="6d2d7-138">id</span></span>|<span data-ttu-id="6d2d7-139">String</span><span class="sxs-lookup"><span data-stu-id="6d2d7-139">String</span></span>|<span data-ttu-id="6d2d7-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-140">Key of the entity.</span></span>|
|<span data-ttu-id="6d2d7-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-141">unknownDeviceCount</span></span>|<span data-ttu-id="6d2d7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-142">Int32</span></span>|<span data-ttu-id="6d2d7-143">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-143">Number of unknown devices</span></span>|
|<span data-ttu-id="6d2d7-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="6d2d7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-145">Int32</span></span>|<span data-ttu-id="6d2d7-146">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="6d2d7-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-147">compliantDeviceCount</span></span>|<span data-ttu-id="6d2d7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-148">Int32</span></span>|<span data-ttu-id="6d2d7-149">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-149">Number of compliant devices</span></span>|
|<span data-ttu-id="6d2d7-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-150">remediatedDeviceCount</span></span>|<span data-ttu-id="6d2d7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-151">Int32</span></span>|<span data-ttu-id="6d2d7-152">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-152">Number of remediated devices</span></span>|
|<span data-ttu-id="6d2d7-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6d2d7-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-154">Int32</span></span>|<span data-ttu-id="6d2d7-155">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="6d2d7-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-156">errorDeviceCount</span></span>|<span data-ttu-id="6d2d7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-157">Int32</span></span>|<span data-ttu-id="6d2d7-158">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-158">Number of error devices</span></span>|
|<span data-ttu-id="6d2d7-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6d2d7-159">conflictDeviceCount</span></span>|<span data-ttu-id="6d2d7-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2d7-160">Int32</span></span>|<span data-ttu-id="6d2d7-161">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="6d2d7-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="6d2d7-162">响应</span><span class="sxs-lookup"><span data-stu-id="6d2d7-162">Response</span></span>
<span data-ttu-id="6d2d7-163">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d2d7-164">示例</span><span class="sxs-lookup"><span data-stu-id="6d2d7-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d2d7-165">请求</span><span class="sxs-lookup"><span data-stu-id="6d2d7-165">Request</span></span>
<span data-ttu-id="6d2d7-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d2d7-167">响应</span><span class="sxs-lookup"><span data-stu-id="6d2d7-167">Response</span></span>
<span data-ttu-id="6d2d7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d2d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




