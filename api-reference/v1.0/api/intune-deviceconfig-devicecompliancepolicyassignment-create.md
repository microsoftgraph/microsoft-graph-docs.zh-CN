---
title: 创建 deviceCompliancePolicyAssignment
description: 创建新的 deviceCompliancePolicyAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b62cd5be14503bd6d725a1ede08b281f7a13c3be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019413"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="b915b-103">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b915b-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="b915b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b915b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b915b-105">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b915b-105">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b915b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b915b-106">Prerequisites</span></span>
<span data-ttu-id="b915b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b915b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b915b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b915b-109">Permission type</span></span>|<span data-ttu-id="b915b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b915b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b915b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b915b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b915b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b915b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b915b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b915b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b915b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b915b-114">Not supported.</span></span>|
|<span data-ttu-id="b915b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b915b-115">Application</span></span>|<span data-ttu-id="b915b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b915b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b915b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b915b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b915b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b915b-118">Request headers</span></span>
|<span data-ttu-id="b915b-119">标头</span><span class="sxs-lookup"><span data-stu-id="b915b-119">Header</span></span>|<span data-ttu-id="b915b-120">值</span><span class="sxs-lookup"><span data-stu-id="b915b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b915b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b915b-121">Authorization</span></span>|<span data-ttu-id="b915b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b915b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b915b-123">接受</span><span class="sxs-lookup"><span data-stu-id="b915b-123">Accept</span></span>|<span data-ttu-id="b915b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b915b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b915b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b915b-125">Request body</span></span>
<span data-ttu-id="b915b-126">在请求正文中，提供 deviceCompliancePolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b915b-126">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="b915b-127">下表显示创建 deviceCompliancePolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b915b-127">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="b915b-128">属性</span><span class="sxs-lookup"><span data-stu-id="b915b-128">Property</span></span>|<span data-ttu-id="b915b-129">类型</span><span class="sxs-lookup"><span data-stu-id="b915b-129">Type</span></span>|<span data-ttu-id="b915b-130">说明</span><span class="sxs-lookup"><span data-stu-id="b915b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b915b-131">id</span><span class="sxs-lookup"><span data-stu-id="b915b-131">id</span></span>|<span data-ttu-id="b915b-132">String</span><span class="sxs-lookup"><span data-stu-id="b915b-132">String</span></span>|<span data-ttu-id="b915b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b915b-133">Key of the entity.</span></span>|
|<span data-ttu-id="b915b-134">target</span><span class="sxs-lookup"><span data-stu-id="b915b-134">target</span></span>|[<span data-ttu-id="b915b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b915b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b915b-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="b915b-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="b915b-137">响应</span><span class="sxs-lookup"><span data-stu-id="b915b-137">Response</span></span>
<span data-ttu-id="b915b-138">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b915b-138">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b915b-139">示例</span><span class="sxs-lookup"><span data-stu-id="b915b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b915b-140">请求</span><span class="sxs-lookup"><span data-stu-id="b915b-140">Request</span></span>
<span data-ttu-id="b915b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b915b-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b915b-142">响应</span><span class="sxs-lookup"><span data-stu-id="b915b-142">Response</span></span>
<span data-ttu-id="b915b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b915b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



