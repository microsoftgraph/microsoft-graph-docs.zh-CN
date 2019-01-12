---
title: 更新 deviceCompliancePolicyDeviceStateSummary
description: 更新 deviceCompliancePolicyDeviceStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a8df64bd2b6c5976481b00eedf3212d115eba23
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933363"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="de5d8-103">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="de5d8-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="de5d8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de5d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de5d8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de5d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de5d8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="de5d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de5d8-107">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de5d8-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de5d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="de5d8-108">Prerequisites</span></span>
<span data-ttu-id="de5d8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="de5d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de5d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de5d8-111">Permission type</span></span>|<span data-ttu-id="de5d8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de5d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de5d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de5d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de5d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de5d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de5d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de5d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de5d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de5d8-116">Not supported.</span></span>|
|<span data-ttu-id="de5d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de5d8-117">Application</span></span>|<span data-ttu-id="de5d8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="de5d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de5d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de5d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="de5d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de5d8-120">Request headers</span></span>
|<span data-ttu-id="de5d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="de5d8-121">Header</span></span>|<span data-ttu-id="de5d8-122">值</span><span class="sxs-lookup"><span data-stu-id="de5d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de5d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de5d8-123">Authorization</span></span>|<span data-ttu-id="de5d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de5d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de5d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de5d8-125">Accept</span></span>|<span data-ttu-id="de5d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de5d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de5d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de5d8-127">Request body</span></span>
<span data-ttu-id="de5d8-128">在请求正文中，提供 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de5d8-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="de5d8-129">下表显示了创建 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de5d8-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="de5d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="de5d8-130">Property</span></span>|<span data-ttu-id="de5d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="de5d8-131">Type</span></span>|<span data-ttu-id="de5d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="de5d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de5d8-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-133">inGracePeriodCount</span></span>|<span data-ttu-id="de5d8-134">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-134">Int32</span></span>|<span data-ttu-id="de5d8-135">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="de5d8-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="de5d8-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-136">configManagerCount</span></span>|<span data-ttu-id="de5d8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-137">Int32</span></span>|<span data-ttu-id="de5d8-138">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="de5d8-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="de5d8-139">id</span><span class="sxs-lookup"><span data-stu-id="de5d8-139">id</span></span>|<span data-ttu-id="de5d8-140">String</span><span class="sxs-lookup"><span data-stu-id="de5d8-140">String</span></span>|<span data-ttu-id="de5d8-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="de5d8-141">Key of the entity.</span></span>|
|<span data-ttu-id="de5d8-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-142">unknownDeviceCount</span></span>|<span data-ttu-id="de5d8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-143">Int32</span></span>|<span data-ttu-id="de5d8-144">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-144">Number of unknown devices</span></span>|
|<span data-ttu-id="de5d8-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="de5d8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-146">Int32</span></span>|<span data-ttu-id="de5d8-147">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="de5d8-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-148">compliantDeviceCount</span></span>|<span data-ttu-id="de5d8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-149">Int32</span></span>|<span data-ttu-id="de5d8-150">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-150">Number of compliant devices</span></span>|
|<span data-ttu-id="de5d8-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-151">remediatedDeviceCount</span></span>|<span data-ttu-id="de5d8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-152">Int32</span></span>|<span data-ttu-id="de5d8-153">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-153">Number of remediated devices</span></span>|
|<span data-ttu-id="de5d8-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="de5d8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-155">Int32</span></span>|<span data-ttu-id="de5d8-156">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="de5d8-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-157">errorDeviceCount</span></span>|<span data-ttu-id="de5d8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-158">Int32</span></span>|<span data-ttu-id="de5d8-159">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-159">Number of error devices</span></span>|
|<span data-ttu-id="de5d8-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="de5d8-160">conflictDeviceCount</span></span>|<span data-ttu-id="de5d8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="de5d8-161">Int32</span></span>|<span data-ttu-id="de5d8-162">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="de5d8-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="de5d8-163">响应</span><span class="sxs-lookup"><span data-stu-id="de5d8-163">Response</span></span>
<span data-ttu-id="de5d8-164">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de5d8-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de5d8-165">示例</span><span class="sxs-lookup"><span data-stu-id="de5d8-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="de5d8-166">请求</span><span class="sxs-lookup"><span data-stu-id="de5d8-166">Request</span></span>
<span data-ttu-id="de5d8-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de5d8-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
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

### <a name="response"></a><span data-ttu-id="de5d8-168">响应</span><span class="sxs-lookup"><span data-stu-id="de5d8-168">Response</span></span>
<span data-ttu-id="de5d8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de5d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





