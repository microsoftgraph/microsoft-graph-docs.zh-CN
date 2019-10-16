---
title: 更新 deviceCompliancePolicyAssignment
description: 更新 deviceCompliancePolicyAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1c5774eb9e40e42005c65b2910098578d511e00
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534181"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="db3c6-103">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="db3c6-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="db3c6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db3c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db3c6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db3c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db3c6-106">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db3c6-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db3c6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db3c6-107">Prerequisites</span></span>
<span data-ttu-id="db3c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db3c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db3c6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db3c6-110">Permission type</span></span>|<span data-ttu-id="db3c6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db3c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db3c6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db3c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db3c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db3c6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db3c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db3c6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db3c6-115">Not supported.</span></span>|
|<span data-ttu-id="db3c6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db3c6-116">Application</span></span>|<span data-ttu-id="db3c6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3c6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db3c6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db3c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="db3c6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db3c6-119">Request headers</span></span>
|<span data-ttu-id="db3c6-120">标头</span><span class="sxs-lookup"><span data-stu-id="db3c6-120">Header</span></span>|<span data-ttu-id="db3c6-121">值</span><span class="sxs-lookup"><span data-stu-id="db3c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db3c6-122">授权</span><span class="sxs-lookup"><span data-stu-id="db3c6-122">Authorization</span></span>|<span data-ttu-id="db3c6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db3c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db3c6-124">接受</span><span class="sxs-lookup"><span data-stu-id="db3c6-124">Accept</span></span>|<span data-ttu-id="db3c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db3c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db3c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db3c6-126">Request body</span></span>
<span data-ttu-id="db3c6-127">在请求正文中，提供 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db3c6-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="db3c6-128">下表显示创建 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db3c6-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="db3c6-129">属性</span><span class="sxs-lookup"><span data-stu-id="db3c6-129">Property</span></span>|<span data-ttu-id="db3c6-130">类型</span><span class="sxs-lookup"><span data-stu-id="db3c6-130">Type</span></span>|<span data-ttu-id="db3c6-131">说明</span><span class="sxs-lookup"><span data-stu-id="db3c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db3c6-132">id</span><span class="sxs-lookup"><span data-stu-id="db3c6-132">id</span></span>|<span data-ttu-id="db3c6-133">字符串</span><span class="sxs-lookup"><span data-stu-id="db3c6-133">String</span></span>|<span data-ttu-id="db3c6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db3c6-134">Key of the entity.</span></span>|
|<span data-ttu-id="db3c6-135">target</span><span class="sxs-lookup"><span data-stu-id="db3c6-135">target</span></span>|[<span data-ttu-id="db3c6-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="db3c6-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="db3c6-137">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="db3c6-137">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="db3c6-138">source</span><span class="sxs-lookup"><span data-stu-id="db3c6-138">source</span></span>|[<span data-ttu-id="db3c6-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="db3c6-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="db3c6-140">设备合规性策略、direct 或包裹/policySet 的分配源。</span><span class="sxs-lookup"><span data-stu-id="db3c6-140">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="db3c6-141">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="db3c6-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="db3c6-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="db3c6-142">sourceId</span></span>|<span data-ttu-id="db3c6-143">字符串</span><span class="sxs-lookup"><span data-stu-id="db3c6-143">String</span></span>|<span data-ttu-id="db3c6-144">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="db3c6-144">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="db3c6-145">响应</span><span class="sxs-lookup"><span data-stu-id="db3c6-145">Response</span></span>
<span data-ttu-id="db3c6-146">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db3c6-146">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db3c6-147">示例</span><span class="sxs-lookup"><span data-stu-id="db3c6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="db3c6-148">请求</span><span class="sxs-lookup"><span data-stu-id="db3c6-148">Request</span></span>
<span data-ttu-id="db3c6-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db3c6-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="db3c6-150">响应</span><span class="sxs-lookup"><span data-stu-id="db3c6-150">Response</span></span>
<span data-ttu-id="db3c6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db3c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```






