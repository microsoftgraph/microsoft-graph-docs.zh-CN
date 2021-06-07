---
title: 更新 softwareUpdateStatusSummary
description: 更新 softwareUpdateStatusSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48585dc0ccd4605c84e5bad0b8395f30bc248707
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756237"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="bcbf2-103">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="bcbf2-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="bcbf2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcbf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcbf2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcbf2-106">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcbf2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bcbf2-107">Prerequisites</span></span>
<span data-ttu-id="bcbf2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcbf2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcbf2-110">Permission type</span></span>|<span data-ttu-id="bcbf2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcbf2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcbf2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcbf2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcbf2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbf2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcbf2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcbf2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcbf2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-115">Not supported.</span></span>|
|<span data-ttu-id="bcbf2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcbf2-116">Application</span></span>|<span data-ttu-id="bcbf2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbf2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcbf2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcbf2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="bcbf2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcbf2-119">Request headers</span></span>
|<span data-ttu-id="bcbf2-120">标头</span><span class="sxs-lookup"><span data-stu-id="bcbf2-120">Header</span></span>|<span data-ttu-id="bcbf2-121">值</span><span class="sxs-lookup"><span data-stu-id="bcbf2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcbf2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcbf2-122">Authorization</span></span>|<span data-ttu-id="bcbf2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcbf2-124">接受</span><span class="sxs-lookup"><span data-stu-id="bcbf2-124">Accept</span></span>|<span data-ttu-id="bcbf2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bcbf2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcbf2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcbf2-126">Request body</span></span>
<span data-ttu-id="bcbf2-127">在请求正文中，提供 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="bcbf2-128">下表显示了创建 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="bcbf2-129">属性</span><span class="sxs-lookup"><span data-stu-id="bcbf2-129">Property</span></span>|<span data-ttu-id="bcbf2-130">类型</span><span class="sxs-lookup"><span data-stu-id="bcbf2-130">Type</span></span>|<span data-ttu-id="bcbf2-131">说明</span><span class="sxs-lookup"><span data-stu-id="bcbf2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcbf2-132">id</span><span class="sxs-lookup"><span data-stu-id="bcbf2-132">id</span></span>|<span data-ttu-id="bcbf2-133">String</span><span class="sxs-lookup"><span data-stu-id="bcbf2-133">String</span></span>|<span data-ttu-id="bcbf2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-134">Key of the entity.</span></span>|
|<span data-ttu-id="bcbf2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bcbf2-135">displayName</span></span>|<span data-ttu-id="bcbf2-136">String</span><span class="sxs-lookup"><span data-stu-id="bcbf2-136">String</span></span>|<span data-ttu-id="bcbf2-137">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-137">The name of the policy.</span></span>|
|<span data-ttu-id="bcbf2-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-138">compliantDeviceCount</span></span>|<span data-ttu-id="bcbf2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-139">Int32</span></span>|<span data-ttu-id="bcbf2-140">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="bcbf2-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bcbf2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-142">Int32</span></span>|<span data-ttu-id="bcbf2-143">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="bcbf2-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-144">remediatedDeviceCount</span></span>|<span data-ttu-id="bcbf2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-145">Int32</span></span>|<span data-ttu-id="bcbf2-146">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="bcbf2-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-147">errorDeviceCount</span></span>|<span data-ttu-id="bcbf2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-148">Int32</span></span>|<span data-ttu-id="bcbf2-149">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-149">Number of devices had error.</span></span>|
|<span data-ttu-id="bcbf2-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-150">unknownDeviceCount</span></span>|<span data-ttu-id="bcbf2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-151">Int32</span></span>|<span data-ttu-id="bcbf2-152">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="bcbf2-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-153">conflictDeviceCount</span></span>|<span data-ttu-id="bcbf2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-154">Int32</span></span>|<span data-ttu-id="bcbf2-155">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="bcbf2-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="bcbf2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-157">Int32</span></span>|<span data-ttu-id="bcbf2-158">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="bcbf2-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-159">compliantUserCount</span></span>|<span data-ttu-id="bcbf2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-160">Int32</span></span>|<span data-ttu-id="bcbf2-161">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-161">Number of compliant users.</span></span>|
|<span data-ttu-id="bcbf2-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-162">nonCompliantUserCount</span></span>|<span data-ttu-id="bcbf2-163">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-163">Int32</span></span>|<span data-ttu-id="bcbf2-164">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="bcbf2-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-165">remediatedUserCount</span></span>|<span data-ttu-id="bcbf2-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-166">Int32</span></span>|<span data-ttu-id="bcbf2-167">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-167">Number of remediated users.</span></span>|
|<span data-ttu-id="bcbf2-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-168">errorUserCount</span></span>|<span data-ttu-id="bcbf2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-169">Int32</span></span>|<span data-ttu-id="bcbf2-170">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-170">Number of users had error.</span></span>|
|<span data-ttu-id="bcbf2-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-171">unknownUserCount</span></span>|<span data-ttu-id="bcbf2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-172">Int32</span></span>|<span data-ttu-id="bcbf2-173">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-173">Number of unknown users.</span></span>|
|<span data-ttu-id="bcbf2-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-174">conflictUserCount</span></span>|<span data-ttu-id="bcbf2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-175">Int32</span></span>|<span data-ttu-id="bcbf2-176">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-176">Number of conflict users.</span></span>|
|<span data-ttu-id="bcbf2-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="bcbf2-177">notApplicableUserCount</span></span>|<span data-ttu-id="bcbf2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbf2-178">Int32</span></span>|<span data-ttu-id="bcbf2-179">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="bcbf2-180">响应</span><span class="sxs-lookup"><span data-stu-id="bcbf2-180">Response</span></span>
<span data-ttu-id="bcbf2-181">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcbf2-182">示例</span><span class="sxs-lookup"><span data-stu-id="bcbf2-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcbf2-183">请求</span><span class="sxs-lookup"><span data-stu-id="bcbf2-183">Request</span></span>
<span data-ttu-id="bcbf2-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcbf2-185">响应</span><span class="sxs-lookup"><span data-stu-id="bcbf2-185">Response</span></span>
<span data-ttu-id="bcbf2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bcbf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




