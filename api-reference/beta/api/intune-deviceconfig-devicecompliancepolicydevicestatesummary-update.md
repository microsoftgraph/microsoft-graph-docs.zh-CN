---
title: 更新 deviceCompliancePolicyDeviceStateSummary
description: 更新 deviceCompliancePolicyDeviceStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71e672ead580f44a1089def05c606aa1504e8216
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443200"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="f0415-103">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f0415-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="f0415-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0415-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0415-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0415-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0415-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0415-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0415-107">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0415-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0415-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0415-108">Prerequisites</span></span>
<span data-ttu-id="f0415-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0415-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0415-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0415-111">Permission type</span></span>|<span data-ttu-id="f0415-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0415-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0415-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0415-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0415-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0415-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0415-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0415-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0415-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0415-116">Not supported.</span></span>|
|<span data-ttu-id="f0415-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0415-117">Application</span></span>|<span data-ttu-id="f0415-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0415-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0415-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0415-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="f0415-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0415-120">Request headers</span></span>
|<span data-ttu-id="f0415-121">标头</span><span class="sxs-lookup"><span data-stu-id="f0415-121">Header</span></span>|<span data-ttu-id="f0415-122">值</span><span class="sxs-lookup"><span data-stu-id="f0415-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0415-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0415-123">Authorization</span></span>|<span data-ttu-id="f0415-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0415-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0415-125">接受</span><span class="sxs-lookup"><span data-stu-id="f0415-125">Accept</span></span>|<span data-ttu-id="f0415-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0415-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0415-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0415-127">Request body</span></span>
<span data-ttu-id="f0415-128">在请求正文中，提供 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0415-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="f0415-129">下表显示了创建 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f0415-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="f0415-130">属性</span><span class="sxs-lookup"><span data-stu-id="f0415-130">Property</span></span>|<span data-ttu-id="f0415-131">类型</span><span class="sxs-lookup"><span data-stu-id="f0415-131">Type</span></span>|<span data-ttu-id="f0415-132">说明</span><span class="sxs-lookup"><span data-stu-id="f0415-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0415-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="f0415-133">inGracePeriodCount</span></span>|<span data-ttu-id="f0415-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-134">Int32</span></span>|<span data-ttu-id="f0415-135">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="f0415-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="f0415-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="f0415-136">configManagerCount</span></span>|<span data-ttu-id="f0415-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-137">Int32</span></span>|<span data-ttu-id="f0415-138">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="f0415-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="f0415-139">id</span><span class="sxs-lookup"><span data-stu-id="f0415-139">id</span></span>|<span data-ttu-id="f0415-140">String</span><span class="sxs-lookup"><span data-stu-id="f0415-140">String</span></span>|<span data-ttu-id="f0415-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f0415-141">Key of the entity.</span></span>|
|<span data-ttu-id="f0415-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-142">unknownDeviceCount</span></span>|<span data-ttu-id="f0415-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-143">Int32</span></span>|<span data-ttu-id="f0415-144">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-144">Number of unknown devices</span></span>|
|<span data-ttu-id="f0415-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="f0415-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-146">Int32</span></span>|<span data-ttu-id="f0415-147">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="f0415-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-148">compliantDeviceCount</span></span>|<span data-ttu-id="f0415-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-149">Int32</span></span>|<span data-ttu-id="f0415-150">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-150">Number of compliant devices</span></span>|
|<span data-ttu-id="f0415-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-151">remediatedDeviceCount</span></span>|<span data-ttu-id="f0415-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-152">Int32</span></span>|<span data-ttu-id="f0415-153">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-153">Number of remediated devices</span></span>|
|<span data-ttu-id="f0415-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f0415-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-155">Int32</span></span>|<span data-ttu-id="f0415-156">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f0415-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-157">errorDeviceCount</span></span>|<span data-ttu-id="f0415-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-158">Int32</span></span>|<span data-ttu-id="f0415-159">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-159">Number of error devices</span></span>|
|<span data-ttu-id="f0415-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0415-160">conflictDeviceCount</span></span>|<span data-ttu-id="f0415-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f0415-161">Int32</span></span>|<span data-ttu-id="f0415-162">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="f0415-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f0415-163">响应</span><span class="sxs-lookup"><span data-stu-id="f0415-163">Response</span></span>
<span data-ttu-id="f0415-164">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0415-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0415-165">示例</span><span class="sxs-lookup"><span data-stu-id="f0415-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0415-166">请求</span><span class="sxs-lookup"><span data-stu-id="f0415-166">Request</span></span>
<span data-ttu-id="f0415-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0415-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0415-168">响应</span><span class="sxs-lookup"><span data-stu-id="f0415-168">Response</span></span>
<span data-ttu-id="f0415-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0415-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





