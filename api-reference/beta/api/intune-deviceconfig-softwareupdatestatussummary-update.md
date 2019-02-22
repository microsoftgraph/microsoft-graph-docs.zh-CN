---
title: 更新 softwareUpdateStatusSummary
description: 更新 softwareUpdateStatusSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76475402e0bb240606cfff0ed25b4502b2feb206
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145092"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="120d3-103">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="120d3-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="120d3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="120d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="120d3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="120d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="120d3-106">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="120d3-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="120d3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="120d3-107">Prerequisites</span></span>
<span data-ttu-id="120d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="120d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="120d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="120d3-110">Permission type</span></span>|<span data-ttu-id="120d3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="120d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="120d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="120d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="120d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="120d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="120d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="120d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="120d3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="120d3-115">Not supported.</span></span>|
|<span data-ttu-id="120d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="120d3-116">Application</span></span>|<span data-ttu-id="120d3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="120d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="120d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="120d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="120d3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="120d3-119">Request headers</span></span>
|<span data-ttu-id="120d3-120">标头</span><span class="sxs-lookup"><span data-stu-id="120d3-120">Header</span></span>|<span data-ttu-id="120d3-121">值</span><span class="sxs-lookup"><span data-stu-id="120d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="120d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="120d3-122">Authorization</span></span>|<span data-ttu-id="120d3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="120d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="120d3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="120d3-124">Accept</span></span>|<span data-ttu-id="120d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="120d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="120d3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="120d3-126">Request body</span></span>
<span data-ttu-id="120d3-127">在请求正文中，提供 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="120d3-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="120d3-128">下表显示了创建 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="120d3-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="120d3-129">属性</span><span class="sxs-lookup"><span data-stu-id="120d3-129">Property</span></span>|<span data-ttu-id="120d3-130">类型</span><span class="sxs-lookup"><span data-stu-id="120d3-130">Type</span></span>|<span data-ttu-id="120d3-131">说明</span><span class="sxs-lookup"><span data-stu-id="120d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120d3-132">id</span><span class="sxs-lookup"><span data-stu-id="120d3-132">id</span></span>|<span data-ttu-id="120d3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="120d3-133">String</span></span>|<span data-ttu-id="120d3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="120d3-134">Key of the entity.</span></span>|
|<span data-ttu-id="120d3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="120d3-135">displayName</span></span>|<span data-ttu-id="120d3-136">String</span><span class="sxs-lookup"><span data-stu-id="120d3-136">String</span></span>|<span data-ttu-id="120d3-137">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="120d3-137">The name of the policy.</span></span>|
|<span data-ttu-id="120d3-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-138">compliantDeviceCount</span></span>|<span data-ttu-id="120d3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-139">Int32</span></span>|<span data-ttu-id="120d3-140">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="120d3-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="120d3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-142">Int32</span></span>|<span data-ttu-id="120d3-143">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="120d3-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-144">remediatedDeviceCount</span></span>|<span data-ttu-id="120d3-145">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-145">Int32</span></span>|<span data-ttu-id="120d3-146">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="120d3-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-147">errorDeviceCount</span></span>|<span data-ttu-id="120d3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-148">Int32</span></span>|<span data-ttu-id="120d3-149">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-149">Number of devices had error.</span></span>|
|<span data-ttu-id="120d3-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-150">unknownDeviceCount</span></span>|<span data-ttu-id="120d3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-151">Int32</span></span>|<span data-ttu-id="120d3-152">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="120d3-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-153">conflictDeviceCount</span></span>|<span data-ttu-id="120d3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-154">Int32</span></span>|<span data-ttu-id="120d3-155">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="120d3-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="120d3-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="120d3-157">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-157">Int32</span></span>|<span data-ttu-id="120d3-158">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="120d3-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-159">compliantUserCount</span></span>|<span data-ttu-id="120d3-160">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-160">Int32</span></span>|<span data-ttu-id="120d3-161">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-161">Number of compliant users.</span></span>|
|<span data-ttu-id="120d3-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-162">nonCompliantUserCount</span></span>|<span data-ttu-id="120d3-163">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-163">Int32</span></span>|<span data-ttu-id="120d3-164">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="120d3-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-165">remediatedUserCount</span></span>|<span data-ttu-id="120d3-166">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-166">Int32</span></span>|<span data-ttu-id="120d3-167">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-167">Number of remediated users.</span></span>|
|<span data-ttu-id="120d3-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-168">errorUserCount</span></span>|<span data-ttu-id="120d3-169">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-169">Int32</span></span>|<span data-ttu-id="120d3-170">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-170">Number of users had error.</span></span>|
|<span data-ttu-id="120d3-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-171">unknownUserCount</span></span>|<span data-ttu-id="120d3-172">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-172">Int32</span></span>|<span data-ttu-id="120d3-173">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-173">Number of unknown users.</span></span>|
|<span data-ttu-id="120d3-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-174">conflictUserCount</span></span>|<span data-ttu-id="120d3-175">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-175">Int32</span></span>|<span data-ttu-id="120d3-176">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-176">Number of conflict users.</span></span>|
|<span data-ttu-id="120d3-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="120d3-177">notApplicableUserCount</span></span>|<span data-ttu-id="120d3-178">Int32</span><span class="sxs-lookup"><span data-stu-id="120d3-178">Int32</span></span>|<span data-ttu-id="120d3-179">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="120d3-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="120d3-180">响应</span><span class="sxs-lookup"><span data-stu-id="120d3-180">Response</span></span>
<span data-ttu-id="120d3-181">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="120d3-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="120d3-182">示例</span><span class="sxs-lookup"><span data-stu-id="120d3-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="120d3-183">请求</span><span class="sxs-lookup"><span data-stu-id="120d3-183">Request</span></span>
<span data-ttu-id="120d3-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="120d3-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="120d3-185">响应</span><span class="sxs-lookup"><span data-stu-id="120d3-185">Response</span></span>
<span data-ttu-id="120d3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="120d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```




