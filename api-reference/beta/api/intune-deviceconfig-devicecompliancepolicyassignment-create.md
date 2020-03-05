---
title: 创建 deviceCompliancePolicyAssignment
description: 创建新的 deviceCompliancePolicyAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95e24a6c30dd910de9e7d43e717f0a52bb42db7d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443235"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="150d8-103">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="150d8-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="150d8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="150d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="150d8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="150d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="150d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="150d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="150d8-107">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="150d8-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="150d8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="150d8-108">Prerequisites</span></span>
<span data-ttu-id="150d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="150d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="150d8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="150d8-111">Permission type</span></span>|<span data-ttu-id="150d8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="150d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="150d8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="150d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="150d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="150d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="150d8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="150d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="150d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="150d8-116">Not supported.</span></span>|
|<span data-ttu-id="150d8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="150d8-117">Application</span></span>|<span data-ttu-id="150d8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="150d8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="150d8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="150d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="150d8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="150d8-120">Request headers</span></span>
|<span data-ttu-id="150d8-121">标头</span><span class="sxs-lookup"><span data-stu-id="150d8-121">Header</span></span>|<span data-ttu-id="150d8-122">值</span><span class="sxs-lookup"><span data-stu-id="150d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="150d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="150d8-123">Authorization</span></span>|<span data-ttu-id="150d8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="150d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="150d8-125">接受</span><span class="sxs-lookup"><span data-stu-id="150d8-125">Accept</span></span>|<span data-ttu-id="150d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="150d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="150d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="150d8-127">Request body</span></span>
<span data-ttu-id="150d8-128">在请求正文中，提供 deviceCompliancePolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="150d8-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="150d8-129">下表显示创建 deviceCompliancePolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="150d8-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="150d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="150d8-130">Property</span></span>|<span data-ttu-id="150d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="150d8-131">Type</span></span>|<span data-ttu-id="150d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="150d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="150d8-133">id</span><span class="sxs-lookup"><span data-stu-id="150d8-133">id</span></span>|<span data-ttu-id="150d8-134">String</span><span class="sxs-lookup"><span data-stu-id="150d8-134">String</span></span>|<span data-ttu-id="150d8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="150d8-135">Key of the entity.</span></span>|
|<span data-ttu-id="150d8-136">target</span><span class="sxs-lookup"><span data-stu-id="150d8-136">target</span></span>|[<span data-ttu-id="150d8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="150d8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="150d8-138">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="150d8-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="150d8-139">source</span><span class="sxs-lookup"><span data-stu-id="150d8-139">source</span></span>|[<span data-ttu-id="150d8-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="150d8-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="150d8-141">设备合规性策略、direct 或包裹/policySet 的分配源。</span><span class="sxs-lookup"><span data-stu-id="150d8-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="150d8-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="150d8-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="150d8-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="150d8-143">sourceId</span></span>|<span data-ttu-id="150d8-144">String</span><span class="sxs-lookup"><span data-stu-id="150d8-144">String</span></span>|<span data-ttu-id="150d8-145">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="150d8-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="150d8-146">响应</span><span class="sxs-lookup"><span data-stu-id="150d8-146">Response</span></span>
<span data-ttu-id="150d8-147">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="150d8-147">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="150d8-148">示例</span><span class="sxs-lookup"><span data-stu-id="150d8-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="150d8-149">请求</span><span class="sxs-lookup"><span data-stu-id="150d8-149">Request</span></span>
<span data-ttu-id="150d8-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="150d8-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
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

### <a name="response"></a><span data-ttu-id="150d8-151">响应</span><span class="sxs-lookup"><span data-stu-id="150d8-151">Response</span></span>
<span data-ttu-id="150d8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="150d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





