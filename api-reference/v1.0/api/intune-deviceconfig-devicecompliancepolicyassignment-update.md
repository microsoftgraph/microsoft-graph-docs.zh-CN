---
title: 更新 deviceCompliancePolicyAssignment
description: 更新 deviceCompliancePolicyAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: 9319b3b429e9ddff67ee66ecb93e7111e5732db6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319108"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="d2938-103">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2938-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="d2938-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2938-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2938-105">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2938-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2938-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2938-106">Prerequisites</span></span>
<span data-ttu-id="d2938-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d2938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2938-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2938-109">Permission type</span></span>|<span data-ttu-id="d2938-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2938-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2938-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2938-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2938-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2938-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2938-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2938-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2938-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2938-114">Not supported.</span></span>|
|<span data-ttu-id="d2938-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2938-115">Application</span></span>|<span data-ttu-id="d2938-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2938-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2938-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2938-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d2938-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2938-118">Request headers</span></span>
|<span data-ttu-id="d2938-119">标头</span><span class="sxs-lookup"><span data-stu-id="d2938-119">Header</span></span>|<span data-ttu-id="d2938-120">值</span><span class="sxs-lookup"><span data-stu-id="d2938-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2938-121">授权</span><span class="sxs-lookup"><span data-stu-id="d2938-121">Authorization</span></span>|<span data-ttu-id="d2938-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2938-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2938-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d2938-123">Accept</span></span>|<span data-ttu-id="d2938-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d2938-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2938-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2938-125">Request body</span></span>
<span data-ttu-id="d2938-126">在请求正文中，提供 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2938-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="d2938-127">下表显示创建 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2938-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="d2938-128">属性</span><span class="sxs-lookup"><span data-stu-id="d2938-128">Property</span></span>|<span data-ttu-id="d2938-129">类型</span><span class="sxs-lookup"><span data-stu-id="d2938-129">Type</span></span>|<span data-ttu-id="d2938-130">说明</span><span class="sxs-lookup"><span data-stu-id="d2938-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2938-131">id</span><span class="sxs-lookup"><span data-stu-id="d2938-131">id</span></span>|<span data-ttu-id="d2938-132">String</span><span class="sxs-lookup"><span data-stu-id="d2938-132">String</span></span>|<span data-ttu-id="d2938-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2938-133">Key of the entity.</span></span>|
|<span data-ttu-id="d2938-134">target</span><span class="sxs-lookup"><span data-stu-id="d2938-134">target</span></span>|[<span data-ttu-id="d2938-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d2938-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d2938-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="d2938-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="d2938-137">响应</span><span class="sxs-lookup"><span data-stu-id="d2938-137">Response</span></span>
<span data-ttu-id="d2938-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2938-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2938-139">示例</span><span class="sxs-lookup"><span data-stu-id="d2938-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2938-140">请求</span><span class="sxs-lookup"><span data-stu-id="d2938-140">Request</span></span>
<span data-ttu-id="d2938-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2938-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2938-142">响应</span><span class="sxs-lookup"><span data-stu-id="d2938-142">Response</span></span>
<span data-ttu-id="d2938-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2938-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



