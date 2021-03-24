---
title: 更新 deviceCompliancePolicyDeviceStateSummary
description: 更新 deviceCompliancePolicyDeviceStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f41e642efd78d0ce237ca650e971550cb507cd0a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132749"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="c315e-103">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c315e-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="c315e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c315e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c315e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c315e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c315e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c315e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c315e-107">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c315e-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c315e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c315e-108">Prerequisites</span></span>
<span data-ttu-id="c315e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c315e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c315e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c315e-111">Permission type</span></span>|<span data-ttu-id="c315e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c315e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c315e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c315e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c315e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c315e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c315e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c315e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c315e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c315e-116">Not supported.</span></span>|
|<span data-ttu-id="c315e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c315e-117">Application</span></span>|<span data-ttu-id="c315e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c315e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c315e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c315e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c315e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c315e-120">Request headers</span></span>
|<span data-ttu-id="c315e-121">标头</span><span class="sxs-lookup"><span data-stu-id="c315e-121">Header</span></span>|<span data-ttu-id="c315e-122">值</span><span class="sxs-lookup"><span data-stu-id="c315e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c315e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c315e-123">Authorization</span></span>|<span data-ttu-id="c315e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c315e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c315e-125">接受</span><span class="sxs-lookup"><span data-stu-id="c315e-125">Accept</span></span>|<span data-ttu-id="c315e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c315e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c315e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c315e-127">Request body</span></span>
<span data-ttu-id="c315e-128">在请求正文中，提供 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c315e-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="c315e-129">下表显示了创建 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c315e-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="c315e-130">属性</span><span class="sxs-lookup"><span data-stu-id="c315e-130">Property</span></span>|<span data-ttu-id="c315e-131">类型</span><span class="sxs-lookup"><span data-stu-id="c315e-131">Type</span></span>|<span data-ttu-id="c315e-132">说明</span><span class="sxs-lookup"><span data-stu-id="c315e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c315e-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="c315e-133">inGracePeriodCount</span></span>|<span data-ttu-id="c315e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-134">Int32</span></span>|<span data-ttu-id="c315e-135">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="c315e-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="c315e-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="c315e-136">configManagerCount</span></span>|<span data-ttu-id="c315e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-137">Int32</span></span>|<span data-ttu-id="c315e-138">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="c315e-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="c315e-139">id</span><span class="sxs-lookup"><span data-stu-id="c315e-139">id</span></span>|<span data-ttu-id="c315e-140">String</span><span class="sxs-lookup"><span data-stu-id="c315e-140">String</span></span>|<span data-ttu-id="c315e-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c315e-141">Key of the entity.</span></span>|
|<span data-ttu-id="c315e-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-142">unknownDeviceCount</span></span>|<span data-ttu-id="c315e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-143">Int32</span></span>|<span data-ttu-id="c315e-144">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-144">Number of unknown devices</span></span>|
|<span data-ttu-id="c315e-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="c315e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-146">Int32</span></span>|<span data-ttu-id="c315e-147">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="c315e-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-148">compliantDeviceCount</span></span>|<span data-ttu-id="c315e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-149">Int32</span></span>|<span data-ttu-id="c315e-150">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-150">Number of compliant devices</span></span>|
|<span data-ttu-id="c315e-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-151">remediatedDeviceCount</span></span>|<span data-ttu-id="c315e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-152">Int32</span></span>|<span data-ttu-id="c315e-153">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-153">Number of remediated devices</span></span>|
|<span data-ttu-id="c315e-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c315e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-155">Int32</span></span>|<span data-ttu-id="c315e-156">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c315e-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-157">errorDeviceCount</span></span>|<span data-ttu-id="c315e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-158">Int32</span></span>|<span data-ttu-id="c315e-159">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-159">Number of error devices</span></span>|
|<span data-ttu-id="c315e-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c315e-160">conflictDeviceCount</span></span>|<span data-ttu-id="c315e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c315e-161">Int32</span></span>|<span data-ttu-id="c315e-162">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="c315e-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="c315e-163">响应</span><span class="sxs-lookup"><span data-stu-id="c315e-163">Response</span></span>
<span data-ttu-id="c315e-164">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c315e-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c315e-165">示例</span><span class="sxs-lookup"><span data-stu-id="c315e-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c315e-166">请求</span><span class="sxs-lookup"><span data-stu-id="c315e-166">Request</span></span>
<span data-ttu-id="c315e-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c315e-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
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

### <a name="response"></a><span data-ttu-id="c315e-168">响应</span><span class="sxs-lookup"><span data-stu-id="c315e-168">Response</span></span>
<span data-ttu-id="c315e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c315e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




