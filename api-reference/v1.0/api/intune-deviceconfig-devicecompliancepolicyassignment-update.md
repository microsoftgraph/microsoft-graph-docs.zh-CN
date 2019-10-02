---
title: 更新 deviceCompliancePolicyAssignment
description: 更新 deviceCompliancePolicyAssignment 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f3ec6c1f38cbe2b6130a4f8f9f4b3b97ae85117
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354173"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="ca92c-103">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ca92c-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="ca92c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca92c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca92c-105">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca92c-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca92c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca92c-106">Prerequisites</span></span>
<span data-ttu-id="ca92c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca92c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca92c-109">Permission type</span></span>|<span data-ttu-id="ca92c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca92c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca92c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca92c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca92c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca92c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca92c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca92c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca92c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca92c-114">Not supported.</span></span>|
|<span data-ttu-id="ca92c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca92c-115">Application</span></span>|<span data-ttu-id="ca92c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca92c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca92c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca92c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ca92c-118">请求头</span><span class="sxs-lookup"><span data-stu-id="ca92c-118">Request headers</span></span>
|<span data-ttu-id="ca92c-119">标头</span><span class="sxs-lookup"><span data-stu-id="ca92c-119">Header</span></span>|<span data-ttu-id="ca92c-120">值</span><span class="sxs-lookup"><span data-stu-id="ca92c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca92c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca92c-121">Authorization</span></span>|<span data-ttu-id="ca92c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca92c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca92c-123">接受</span><span class="sxs-lookup"><span data-stu-id="ca92c-123">Accept</span></span>|<span data-ttu-id="ca92c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ca92c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca92c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca92c-125">Request body</span></span>
<span data-ttu-id="ca92c-126">在请求正文中，提供 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca92c-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="ca92c-127">下表显示创建 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca92c-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="ca92c-128">属性</span><span class="sxs-lookup"><span data-stu-id="ca92c-128">Property</span></span>|<span data-ttu-id="ca92c-129">类型</span><span class="sxs-lookup"><span data-stu-id="ca92c-129">Type</span></span>|<span data-ttu-id="ca92c-130">说明</span><span class="sxs-lookup"><span data-stu-id="ca92c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca92c-131">id</span><span class="sxs-lookup"><span data-stu-id="ca92c-131">id</span></span>|<span data-ttu-id="ca92c-132">String</span><span class="sxs-lookup"><span data-stu-id="ca92c-132">String</span></span>|<span data-ttu-id="ca92c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ca92c-133">Key of the entity.</span></span>|
|<span data-ttu-id="ca92c-134">target</span><span class="sxs-lookup"><span data-stu-id="ca92c-134">target</span></span>|[<span data-ttu-id="ca92c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ca92c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ca92c-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="ca92c-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ca92c-137">响应</span><span class="sxs-lookup"><span data-stu-id="ca92c-137">Response</span></span>
<span data-ttu-id="ca92c-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca92c-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca92c-139">示例</span><span class="sxs-lookup"><span data-stu-id="ca92c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca92c-140">请求</span><span class="sxs-lookup"><span data-stu-id="ca92c-140">Request</span></span>
<span data-ttu-id="ca92c-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca92c-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ca92c-142">响应</span><span class="sxs-lookup"><span data-stu-id="ca92c-142">Response</span></span>
<span data-ttu-id="ca92c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca92c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




