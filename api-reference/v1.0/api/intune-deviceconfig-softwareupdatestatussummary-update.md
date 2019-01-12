---
title: 更新 softwareUpdateStatusSummary
description: 更新 softwareUpdateStatusSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 84402834e7e1cfea5c08cc2d0714f5676946920f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938130"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="a077e-103">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a077e-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="a077e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a077e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a077e-105">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a077e-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a077e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a077e-106">Prerequisites</span></span>
<span data-ttu-id="a077e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a077e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a077e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a077e-109">Permission type</span></span>|<span data-ttu-id="a077e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a077e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a077e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a077e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a077e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a077e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a077e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a077e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a077e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a077e-114">Not supported.</span></span>|
|<span data-ttu-id="a077e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a077e-115">Application</span></span>|<span data-ttu-id="a077e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a077e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a077e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a077e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a077e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a077e-118">Request headers</span></span>
|<span data-ttu-id="a077e-119">标头</span><span class="sxs-lookup"><span data-stu-id="a077e-119">Header</span></span>|<span data-ttu-id="a077e-120">值</span><span class="sxs-lookup"><span data-stu-id="a077e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a077e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a077e-121">Authorization</span></span>|<span data-ttu-id="a077e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a077e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a077e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a077e-123">Accept</span></span>|<span data-ttu-id="a077e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a077e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a077e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a077e-125">Request body</span></span>
<span data-ttu-id="a077e-126">在请求正文中，提供 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a077e-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="a077e-127">下表显示了创建 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a077e-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="a077e-128">属性</span><span class="sxs-lookup"><span data-stu-id="a077e-128">Property</span></span>|<span data-ttu-id="a077e-129">类型</span><span class="sxs-lookup"><span data-stu-id="a077e-129">Type</span></span>|<span data-ttu-id="a077e-130">说明</span><span class="sxs-lookup"><span data-stu-id="a077e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a077e-131">id</span><span class="sxs-lookup"><span data-stu-id="a077e-131">id</span></span>|<span data-ttu-id="a077e-132">String</span><span class="sxs-lookup"><span data-stu-id="a077e-132">String</span></span>|<span data-ttu-id="a077e-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a077e-133">Key of the entity.</span></span>|
|<span data-ttu-id="a077e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a077e-134">displayName</span></span>|<span data-ttu-id="a077e-135">String</span><span class="sxs-lookup"><span data-stu-id="a077e-135">String</span></span>|<span data-ttu-id="a077e-136">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="a077e-136">The name of the policy.</span></span>|
|<span data-ttu-id="a077e-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-137">compliantDeviceCount</span></span>|<span data-ttu-id="a077e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-138">Int32</span></span>|<span data-ttu-id="a077e-139">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="a077e-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a077e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-141">Int32</span></span>|<span data-ttu-id="a077e-142">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="a077e-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-143">remediatedDeviceCount</span></span>|<span data-ttu-id="a077e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-144">Int32</span></span>|<span data-ttu-id="a077e-145">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="a077e-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-146">errorDeviceCount</span></span>|<span data-ttu-id="a077e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-147">Int32</span></span>|<span data-ttu-id="a077e-148">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-148">Number of devices had error.</span></span>|
|<span data-ttu-id="a077e-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-149">unknownDeviceCount</span></span>|<span data-ttu-id="a077e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-150">Int32</span></span>|<span data-ttu-id="a077e-151">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="a077e-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-152">conflictDeviceCount</span></span>|<span data-ttu-id="a077e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-153">Int32</span></span>|<span data-ttu-id="a077e-154">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="a077e-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a077e-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="a077e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-156">Int32</span></span>|<span data-ttu-id="a077e-157">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="a077e-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-158">compliantUserCount</span></span>|<span data-ttu-id="a077e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-159">Int32</span></span>|<span data-ttu-id="a077e-160">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-160">Number of compliant users.</span></span>|
|<span data-ttu-id="a077e-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-161">nonCompliantUserCount</span></span>|<span data-ttu-id="a077e-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-162">Int32</span></span>|<span data-ttu-id="a077e-163">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="a077e-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-164">remediatedUserCount</span></span>|<span data-ttu-id="a077e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-165">Int32</span></span>|<span data-ttu-id="a077e-166">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-166">Number of remediated users.</span></span>|
|<span data-ttu-id="a077e-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-167">errorUserCount</span></span>|<span data-ttu-id="a077e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-168">Int32</span></span>|<span data-ttu-id="a077e-169">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-169">Number of users had error.</span></span>|
|<span data-ttu-id="a077e-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-170">unknownUserCount</span></span>|<span data-ttu-id="a077e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-171">Int32</span></span>|<span data-ttu-id="a077e-172">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-172">Number of unknown users.</span></span>|
|<span data-ttu-id="a077e-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-173">conflictUserCount</span></span>|<span data-ttu-id="a077e-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-174">Int32</span></span>|<span data-ttu-id="a077e-175">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-175">Number of conflict users.</span></span>|
|<span data-ttu-id="a077e-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a077e-176">notApplicableUserCount</span></span>|<span data-ttu-id="a077e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a077e-177">Int32</span></span>|<span data-ttu-id="a077e-178">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="a077e-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="a077e-179">响应</span><span class="sxs-lookup"><span data-stu-id="a077e-179">Response</span></span>
<span data-ttu-id="a077e-180">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a077e-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a077e-181">示例</span><span class="sxs-lookup"><span data-stu-id="a077e-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="a077e-182">请求</span><span class="sxs-lookup"><span data-stu-id="a077e-182">Request</span></span>
<span data-ttu-id="a077e-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a077e-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
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

### <a name="response"></a><span data-ttu-id="a077e-184">响应</span><span class="sxs-lookup"><span data-stu-id="a077e-184">Response</span></span>
<span data-ttu-id="a077e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a077e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



