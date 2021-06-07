---
title: 更新 deviceCompliancePolicyAssignment
description: 更新 deviceCompliancePolicyAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b0dce7e104b3aa472471f515854745fb888c53e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753950"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="c1bfd-103">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="c1bfd-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="c1bfd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1bfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1bfd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1bfd-106">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1bfd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1bfd-107">Prerequisites</span></span>
<span data-ttu-id="c1bfd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1bfd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1bfd-110">Permission type</span></span>|<span data-ttu-id="c1bfd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1bfd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1bfd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1bfd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1bfd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1bfd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1bfd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1bfd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1bfd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-115">Not supported.</span></span>|
|<span data-ttu-id="c1bfd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1bfd-116">Application</span></span>|<span data-ttu-id="c1bfd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1bfd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1bfd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1bfd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1bfd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1bfd-119">Request headers</span></span>
|<span data-ttu-id="c1bfd-120">标头</span><span class="sxs-lookup"><span data-stu-id="c1bfd-120">Header</span></span>|<span data-ttu-id="c1bfd-121">值</span><span class="sxs-lookup"><span data-stu-id="c1bfd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1bfd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1bfd-122">Authorization</span></span>|<span data-ttu-id="c1bfd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1bfd-124">接受</span><span class="sxs-lookup"><span data-stu-id="c1bfd-124">Accept</span></span>|<span data-ttu-id="c1bfd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1bfd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1bfd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1bfd-126">Request body</span></span>
<span data-ttu-id="c1bfd-127">在请求正文中，提供 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="c1bfd-128">下表显示创建 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="c1bfd-129">属性</span><span class="sxs-lookup"><span data-stu-id="c1bfd-129">Property</span></span>|<span data-ttu-id="c1bfd-130">类型</span><span class="sxs-lookup"><span data-stu-id="c1bfd-130">Type</span></span>|<span data-ttu-id="c1bfd-131">说明</span><span class="sxs-lookup"><span data-stu-id="c1bfd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1bfd-132">id</span><span class="sxs-lookup"><span data-stu-id="c1bfd-132">id</span></span>|<span data-ttu-id="c1bfd-133">String</span><span class="sxs-lookup"><span data-stu-id="c1bfd-133">String</span></span>|<span data-ttu-id="c1bfd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-134">Key of the entity.</span></span>|
|<span data-ttu-id="c1bfd-135">target</span><span class="sxs-lookup"><span data-stu-id="c1bfd-135">target</span></span>|[<span data-ttu-id="c1bfd-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c1bfd-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c1bfd-137">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="c1bfd-138">响应</span><span class="sxs-lookup"><span data-stu-id="c1bfd-138">Response</span></span>
<span data-ttu-id="c1bfd-139">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1bfd-140">示例</span><span class="sxs-lookup"><span data-stu-id="c1bfd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1bfd-141">请求</span><span class="sxs-lookup"><span data-stu-id="c1bfd-141">Request</span></span>
<span data-ttu-id="c1bfd-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 224

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="c1bfd-143">响应</span><span class="sxs-lookup"><span data-stu-id="c1bfd-143">Response</span></span>
<span data-ttu-id="c1bfd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1bfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```




