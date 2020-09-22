---
title: 创建 deviceCompliancePolicyAssignment
description: 创建新的 deviceCompliancePolicyAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16259c0f7674a509dd2444f249539e3a91dcde15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052108"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="cac97-103">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cac97-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="cac97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cac97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cac97-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cac97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cac97-106">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cac97-106">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cac97-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cac97-107">Prerequisites</span></span>
<span data-ttu-id="cac97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cac97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cac97-110">Permission type</span></span>|<span data-ttu-id="cac97-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cac97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cac97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cac97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cac97-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac97-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cac97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cac97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cac97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cac97-115">Not supported.</span></span>|
|<span data-ttu-id="cac97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cac97-116">Application</span></span>|<span data-ttu-id="cac97-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cac97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cac97-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cac97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cac97-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cac97-119">Request headers</span></span>
|<span data-ttu-id="cac97-120">标头</span><span class="sxs-lookup"><span data-stu-id="cac97-120">Header</span></span>|<span data-ttu-id="cac97-121">值</span><span class="sxs-lookup"><span data-stu-id="cac97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cac97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac97-122">Authorization</span></span>|<span data-ttu-id="cac97-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cac97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cac97-124">接受</span><span class="sxs-lookup"><span data-stu-id="cac97-124">Accept</span></span>|<span data-ttu-id="cac97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cac97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cac97-126">Request body</span></span>
<span data-ttu-id="cac97-127">在请求正文中，提供 deviceCompliancePolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cac97-127">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="cac97-128">下表显示创建 deviceCompliancePolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cac97-128">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="cac97-129">属性</span><span class="sxs-lookup"><span data-stu-id="cac97-129">Property</span></span>|<span data-ttu-id="cac97-130">类型</span><span class="sxs-lookup"><span data-stu-id="cac97-130">Type</span></span>|<span data-ttu-id="cac97-131">说明</span><span class="sxs-lookup"><span data-stu-id="cac97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac97-132">id</span><span class="sxs-lookup"><span data-stu-id="cac97-132">id</span></span>|<span data-ttu-id="cac97-133">String</span><span class="sxs-lookup"><span data-stu-id="cac97-133">String</span></span>|<span data-ttu-id="cac97-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cac97-134">Key of the entity.</span></span>|
|<span data-ttu-id="cac97-135">target</span><span class="sxs-lookup"><span data-stu-id="cac97-135">target</span></span>|[<span data-ttu-id="cac97-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cac97-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cac97-137">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="cac97-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="cac97-138">响应</span><span class="sxs-lookup"><span data-stu-id="cac97-138">Response</span></span>
<span data-ttu-id="cac97-139">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cac97-139">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac97-140">示例</span><span class="sxs-lookup"><span data-stu-id="cac97-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="cac97-141">请求</span><span class="sxs-lookup"><span data-stu-id="cac97-141">Request</span></span>
<span data-ttu-id="cac97-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cac97-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cac97-143">响应</span><span class="sxs-lookup"><span data-stu-id="cac97-143">Response</span></span>
<span data-ttu-id="cac97-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cac97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









