---
title: 创建 deviceCompliancePolicyAssignment
description: 创建新的 deviceCompliancePolicyAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 520332a4e8ab873730bf138d3f024b512a8fd7c2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155489"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="53f6e-103">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="53f6e-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="53f6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53f6e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53f6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53f6e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53f6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f6e-107">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53f6e-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53f6e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="53f6e-108">Prerequisites</span></span>
<span data-ttu-id="53f6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f6e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53f6e-111">Permission type</span></span>|<span data-ttu-id="53f6e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53f6e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53f6e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53f6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53f6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53f6e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53f6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53f6e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53f6e-116">Not supported.</span></span>|
|<span data-ttu-id="53f6e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53f6e-117">Application</span></span>|<span data-ttu-id="53f6e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f6e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53f6e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53f6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="53f6e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53f6e-120">Request headers</span></span>
|<span data-ttu-id="53f6e-121">标头</span><span class="sxs-lookup"><span data-stu-id="53f6e-121">Header</span></span>|<span data-ttu-id="53f6e-122">值</span><span class="sxs-lookup"><span data-stu-id="53f6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53f6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f6e-123">Authorization</span></span>|<span data-ttu-id="53f6e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53f6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53f6e-125">接受</span><span class="sxs-lookup"><span data-stu-id="53f6e-125">Accept</span></span>|<span data-ttu-id="53f6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53f6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f6e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53f6e-127">Request body</span></span>
<span data-ttu-id="53f6e-128">在请求正文中，提供 deviceCompliancePolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53f6e-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="53f6e-129">下表显示创建 deviceCompliancePolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53f6e-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="53f6e-130">属性</span><span class="sxs-lookup"><span data-stu-id="53f6e-130">Property</span></span>|<span data-ttu-id="53f6e-131">类型</span><span class="sxs-lookup"><span data-stu-id="53f6e-131">Type</span></span>|<span data-ttu-id="53f6e-132">说明</span><span class="sxs-lookup"><span data-stu-id="53f6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f6e-133">id</span><span class="sxs-lookup"><span data-stu-id="53f6e-133">id</span></span>|<span data-ttu-id="53f6e-134">String</span><span class="sxs-lookup"><span data-stu-id="53f6e-134">String</span></span>|<span data-ttu-id="53f6e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53f6e-135">Key of the entity.</span></span>|
|<span data-ttu-id="53f6e-136">target</span><span class="sxs-lookup"><span data-stu-id="53f6e-136">target</span></span>|[<span data-ttu-id="53f6e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="53f6e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="53f6e-138">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="53f6e-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="53f6e-139">source</span><span class="sxs-lookup"><span data-stu-id="53f6e-139">source</span></span>|[<span data-ttu-id="53f6e-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="53f6e-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="53f6e-141">设备合规性策略的分配源：direct 或更新/policySet。</span><span class="sxs-lookup"><span data-stu-id="53f6e-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="53f6e-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="53f6e-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="53f6e-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="53f6e-143">sourceId</span></span>|<span data-ttu-id="53f6e-144">String</span><span class="sxs-lookup"><span data-stu-id="53f6e-144">String</span></span>|<span data-ttu-id="53f6e-145">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="53f6e-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="53f6e-146">响应</span><span class="sxs-lookup"><span data-stu-id="53f6e-146">Response</span></span>
<span data-ttu-id="53f6e-147">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53f6e-147">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53f6e-148">示例</span><span class="sxs-lookup"><span data-stu-id="53f6e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="53f6e-149">请求</span><span class="sxs-lookup"><span data-stu-id="53f6e-149">Request</span></span>
<span data-ttu-id="53f6e-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53f6e-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="53f6e-151">响应</span><span class="sxs-lookup"><span data-stu-id="53f6e-151">Response</span></span>
<span data-ttu-id="53f6e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53f6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




