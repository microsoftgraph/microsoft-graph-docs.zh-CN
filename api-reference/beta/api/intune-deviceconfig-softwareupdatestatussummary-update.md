---
title: 更新 softwareUpdateStatusSummary
description: 更新 softwareUpdateStatusSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a35c52de0da15a20c4607ae7626f9c989795a41d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137054"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="069a3-103">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="069a3-103">Update softwareUpdateStatusSummary</span></span>

<span data-ttu-id="069a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="069a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="069a3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="069a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="069a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="069a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="069a3-107">更新 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="069a3-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="069a3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="069a3-108">Prerequisites</span></span>
<span data-ttu-id="069a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="069a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="069a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="069a3-111">Permission type</span></span>|<span data-ttu-id="069a3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="069a3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="069a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="069a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="069a3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="069a3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="069a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="069a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="069a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="069a3-116">Not supported.</span></span>|
|<span data-ttu-id="069a3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="069a3-117">Application</span></span>|<span data-ttu-id="069a3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="069a3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="069a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="069a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="069a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="069a3-120">Request headers</span></span>
|<span data-ttu-id="069a3-121">标头</span><span class="sxs-lookup"><span data-stu-id="069a3-121">Header</span></span>|<span data-ttu-id="069a3-122">值</span><span class="sxs-lookup"><span data-stu-id="069a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="069a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="069a3-123">Authorization</span></span>|<span data-ttu-id="069a3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="069a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="069a3-125">接受</span><span class="sxs-lookup"><span data-stu-id="069a3-125">Accept</span></span>|<span data-ttu-id="069a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="069a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="069a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="069a3-127">Request body</span></span>
<span data-ttu-id="069a3-128">在请求正文中，提供 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="069a3-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="069a3-129">下表显示了创建 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="069a3-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="069a3-130">属性</span><span class="sxs-lookup"><span data-stu-id="069a3-130">Property</span></span>|<span data-ttu-id="069a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="069a3-131">Type</span></span>|<span data-ttu-id="069a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="069a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="069a3-133">id</span><span class="sxs-lookup"><span data-stu-id="069a3-133">id</span></span>|<span data-ttu-id="069a3-134">String</span><span class="sxs-lookup"><span data-stu-id="069a3-134">String</span></span>|<span data-ttu-id="069a3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="069a3-135">Key of the entity.</span></span>|
|<span data-ttu-id="069a3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="069a3-136">displayName</span></span>|<span data-ttu-id="069a3-137">String</span><span class="sxs-lookup"><span data-stu-id="069a3-137">String</span></span>|<span data-ttu-id="069a3-138">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="069a3-138">The name of the policy.</span></span>|
|<span data-ttu-id="069a3-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-139">compliantDeviceCount</span></span>|<span data-ttu-id="069a3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-140">Int32</span></span>|<span data-ttu-id="069a3-141">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="069a3-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="069a3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-143">Int32</span></span>|<span data-ttu-id="069a3-144">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="069a3-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-145">remediatedDeviceCount</span></span>|<span data-ttu-id="069a3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-146">Int32</span></span>|<span data-ttu-id="069a3-147">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="069a3-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-148">errorDeviceCount</span></span>|<span data-ttu-id="069a3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-149">Int32</span></span>|<span data-ttu-id="069a3-150">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-150">Number of devices had error.</span></span>|
|<span data-ttu-id="069a3-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-151">unknownDeviceCount</span></span>|<span data-ttu-id="069a3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-152">Int32</span></span>|<span data-ttu-id="069a3-153">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="069a3-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-154">conflictDeviceCount</span></span>|<span data-ttu-id="069a3-155">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-155">Int32</span></span>|<span data-ttu-id="069a3-156">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="069a3-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="069a3-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="069a3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-158">Int32</span></span>|<span data-ttu-id="069a3-159">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="069a3-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-160">compliantUserCount</span></span>|<span data-ttu-id="069a3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-161">Int32</span></span>|<span data-ttu-id="069a3-162">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-162">Number of compliant users.</span></span>|
|<span data-ttu-id="069a3-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-163">nonCompliantUserCount</span></span>|<span data-ttu-id="069a3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-164">Int32</span></span>|<span data-ttu-id="069a3-165">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="069a3-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-166">remediatedUserCount</span></span>|<span data-ttu-id="069a3-167">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-167">Int32</span></span>|<span data-ttu-id="069a3-168">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-168">Number of remediated users.</span></span>|
|<span data-ttu-id="069a3-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-169">errorUserCount</span></span>|<span data-ttu-id="069a3-170">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-170">Int32</span></span>|<span data-ttu-id="069a3-171">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-171">Number of users had error.</span></span>|
|<span data-ttu-id="069a3-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-172">unknownUserCount</span></span>|<span data-ttu-id="069a3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-173">Int32</span></span>|<span data-ttu-id="069a3-174">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-174">Number of unknown users.</span></span>|
|<span data-ttu-id="069a3-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-175">conflictUserCount</span></span>|<span data-ttu-id="069a3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-176">Int32</span></span>|<span data-ttu-id="069a3-177">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-177">Number of conflict users.</span></span>|
|<span data-ttu-id="069a3-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="069a3-178">notApplicableUserCount</span></span>|<span data-ttu-id="069a3-179">Int32</span><span class="sxs-lookup"><span data-stu-id="069a3-179">Int32</span></span>|<span data-ttu-id="069a3-180">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="069a3-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="069a3-181">响应</span><span class="sxs-lookup"><span data-stu-id="069a3-181">Response</span></span>
<span data-ttu-id="069a3-182">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="069a3-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="069a3-183">示例</span><span class="sxs-lookup"><span data-stu-id="069a3-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="069a3-184">请求</span><span class="sxs-lookup"><span data-stu-id="069a3-184">Request</span></span>
<span data-ttu-id="069a3-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="069a3-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="069a3-186">响应</span><span class="sxs-lookup"><span data-stu-id="069a3-186">Response</span></span>
<span data-ttu-id="069a3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="069a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




