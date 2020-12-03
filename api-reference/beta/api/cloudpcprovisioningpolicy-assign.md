---
title: cloudPcProvisioningPolicy： assign
description: 将云电脑预配策略分配给你的组。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: cb6efee682b07d19c6638803aa24e1f489310282
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563434"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="90abc-103">cloudPcProvisioningPolicy： assign</span><span class="sxs-lookup"><span data-stu-id="90abc-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="90abc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90abc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90abc-105">将 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="90abc-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="90abc-106">权限</span><span class="sxs-lookup"><span data-stu-id="90abc-106">Permissions</span></span>

<span data-ttu-id="90abc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90abc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90abc-109">Permission type</span></span>|<span data-ttu-id="90abc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90abc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90abc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90abc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90abc-112">CloudPC</span><span class="sxs-lookup"><span data-stu-id="90abc-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="90abc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90abc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90abc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90abc-114">Not supported.</span></span>|
|<span data-ttu-id="90abc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90abc-115">Application</span></span>|<span data-ttu-id="90abc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90abc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90abc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90abc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="90abc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="90abc-118">Request headers</span></span>

|<span data-ttu-id="90abc-119">名称</span><span class="sxs-lookup"><span data-stu-id="90abc-119">Name</span></span>|<span data-ttu-id="90abc-120">说明</span><span class="sxs-lookup"><span data-stu-id="90abc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="90abc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90abc-121">Authorization</span></span>|<span data-ttu-id="90abc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90abc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="90abc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90abc-124">Content-Type</span></span>|<span data-ttu-id="90abc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="90abc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90abc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="90abc-127">Request body</span></span>

<span data-ttu-id="90abc-128">在请求正文中，提供 [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90abc-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="90abc-129">下表显示创建 [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90abc-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="90abc-130">属性</span><span class="sxs-lookup"><span data-stu-id="90abc-130">Property</span></span>|<span data-ttu-id="90abc-131">类型</span><span class="sxs-lookup"><span data-stu-id="90abc-131">Type</span></span>|<span data-ttu-id="90abc-132">说明</span><span class="sxs-lookup"><span data-stu-id="90abc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90abc-133">id</span><span class="sxs-lookup"><span data-stu-id="90abc-133">id</span></span>|<span data-ttu-id="90abc-134">String</span><span class="sxs-lookup"><span data-stu-id="90abc-134">String</span></span>|<span data-ttu-id="90abc-135">设置策略分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="90abc-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="90abc-136">如果 target 是用户组，则 ID 显示为 {policyId} _ {groupId}。</span><span class="sxs-lookup"><span data-stu-id="90abc-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="90abc-137">target</span><span class="sxs-lookup"><span data-stu-id="90abc-137">target</span></span>|[<span data-ttu-id="90abc-138">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="90abc-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="90abc-139">预配策略的分配目标。</span><span class="sxs-lookup"><span data-stu-id="90abc-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="90abc-140">目前，受支持的唯一目标是用户组。</span><span class="sxs-lookup"><span data-stu-id="90abc-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="90abc-141">响应</span><span class="sxs-lookup"><span data-stu-id="90abc-141">Response</span></span>

<span data-ttu-id="90abc-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="90abc-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="90abc-143">示例</span><span class="sxs-lookup"><span data-stu-id="90abc-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90abc-144">请求</span><span class="sxs-lookup"><span data-stu-id="90abc-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="90abc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="90abc-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_cloudpcprovisioningpolicy",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="90abc-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90abc-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90abc-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90abc-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90abc-148">响应</span><span class="sxs-lookup"><span data-stu-id="90abc-148">Response</span></span>

<span data-ttu-id="90abc-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90abc-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
