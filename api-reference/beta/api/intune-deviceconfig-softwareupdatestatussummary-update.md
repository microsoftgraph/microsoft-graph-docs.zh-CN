---
title: 更新 softwareUpdateStatusSummary
description: 更新 softwareUpdateStatusSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c1437e55807e2fba92efb7dab3b908f8bae88487
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837294"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="d2e21-103">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d2e21-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="d2e21-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2e21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2e21-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2e21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2e21-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2e21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2e21-107">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2e21-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2e21-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2e21-108">Prerequisites</span></span>
<span data-ttu-id="d2e21-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d2e21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e21-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2e21-111">Permission type</span></span>|<span data-ttu-id="d2e21-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2e21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2e21-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2e21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2e21-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e21-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2e21-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2e21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2e21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2e21-116">Not supported.</span></span>|
|<span data-ttu-id="d2e21-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2e21-117">Application</span></span>|<span data-ttu-id="d2e21-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2e21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2e21-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2e21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="d2e21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2e21-120">Request headers</span></span>
|<span data-ttu-id="d2e21-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2e21-121">Header</span></span>|<span data-ttu-id="d2e21-122">值</span><span class="sxs-lookup"><span data-stu-id="d2e21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2e21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2e21-123">Authorization</span></span>|<span data-ttu-id="d2e21-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2e21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2e21-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2e21-125">Accept</span></span>|<span data-ttu-id="d2e21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2e21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2e21-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2e21-127">Request body</span></span>
<span data-ttu-id="d2e21-128">在请求正文中，提供 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2e21-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="d2e21-129">下表显示了创建 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2e21-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="d2e21-130">属性</span><span class="sxs-lookup"><span data-stu-id="d2e21-130">Property</span></span>|<span data-ttu-id="d2e21-131">类型</span><span class="sxs-lookup"><span data-stu-id="d2e21-131">Type</span></span>|<span data-ttu-id="d2e21-132">说明</span><span class="sxs-lookup"><span data-stu-id="d2e21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2e21-133">id</span><span class="sxs-lookup"><span data-stu-id="d2e21-133">id</span></span>|<span data-ttu-id="d2e21-134">String</span><span class="sxs-lookup"><span data-stu-id="d2e21-134">String</span></span>|<span data-ttu-id="d2e21-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2e21-135">Key of the entity.</span></span>|
|<span data-ttu-id="d2e21-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d2e21-136">displayName</span></span>|<span data-ttu-id="d2e21-137">String</span><span class="sxs-lookup"><span data-stu-id="d2e21-137">String</span></span>|<span data-ttu-id="d2e21-138">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="d2e21-138">The name of the policy.</span></span>|
|<span data-ttu-id="d2e21-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-139">compliantDeviceCount</span></span>|<span data-ttu-id="d2e21-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-140">Int32</span></span>|<span data-ttu-id="d2e21-141">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="d2e21-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d2e21-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-143">Int32</span></span>|<span data-ttu-id="d2e21-144">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="d2e21-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-145">remediatedDeviceCount</span></span>|<span data-ttu-id="d2e21-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-146">Int32</span></span>|<span data-ttu-id="d2e21-147">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="d2e21-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-148">errorDeviceCount</span></span>|<span data-ttu-id="d2e21-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-149">Int32</span></span>|<span data-ttu-id="d2e21-150">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-150">Number of devices had error.</span></span>|
|<span data-ttu-id="d2e21-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-151">unknownDeviceCount</span></span>|<span data-ttu-id="d2e21-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-152">Int32</span></span>|<span data-ttu-id="d2e21-153">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="d2e21-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-154">conflictDeviceCount</span></span>|<span data-ttu-id="d2e21-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-155">Int32</span></span>|<span data-ttu-id="d2e21-156">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="d2e21-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="d2e21-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-158">Int32</span></span>|<span data-ttu-id="d2e21-159">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="d2e21-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-160">compliantUserCount</span></span>|<span data-ttu-id="d2e21-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-161">Int32</span></span>|<span data-ttu-id="d2e21-162">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-162">Number of compliant users.</span></span>|
|<span data-ttu-id="d2e21-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-163">nonCompliantUserCount</span></span>|<span data-ttu-id="d2e21-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-164">Int32</span></span>|<span data-ttu-id="d2e21-165">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="d2e21-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-166">remediatedUserCount</span></span>|<span data-ttu-id="d2e21-167">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-167">Int32</span></span>|<span data-ttu-id="d2e21-168">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-168">Number of remediated users.</span></span>|
|<span data-ttu-id="d2e21-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-169">errorUserCount</span></span>|<span data-ttu-id="d2e21-170">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-170">Int32</span></span>|<span data-ttu-id="d2e21-171">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-171">Number of users had error.</span></span>|
|<span data-ttu-id="d2e21-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-172">unknownUserCount</span></span>|<span data-ttu-id="d2e21-173">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-173">Int32</span></span>|<span data-ttu-id="d2e21-174">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-174">Number of unknown users.</span></span>|
|<span data-ttu-id="d2e21-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-175">conflictUserCount</span></span>|<span data-ttu-id="d2e21-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-176">Int32</span></span>|<span data-ttu-id="d2e21-177">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-177">Number of conflict users.</span></span>|
|<span data-ttu-id="d2e21-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d2e21-178">notApplicableUserCount</span></span>|<span data-ttu-id="d2e21-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d2e21-179">Int32</span></span>|<span data-ttu-id="d2e21-180">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d2e21-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="d2e21-181">响应</span><span class="sxs-lookup"><span data-stu-id="d2e21-181">Response</span></span>
<span data-ttu-id="d2e21-182">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2e21-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e21-183">示例</span><span class="sxs-lookup"><span data-stu-id="d2e21-183">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2e21-184">请求</span><span class="sxs-lookup"><span data-stu-id="d2e21-184">Request</span></span>
<span data-ttu-id="d2e21-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2e21-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
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

### <a name="response"></a><span data-ttu-id="d2e21-186">响应</span><span class="sxs-lookup"><span data-stu-id="d2e21-186">Response</span></span>
<span data-ttu-id="d2e21-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2e21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





