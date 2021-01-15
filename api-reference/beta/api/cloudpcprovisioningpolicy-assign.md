---
title: cloudPcProvisioningPolicy：assign
description: 将云电脑预配策略分配给你的组。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4b6acff15539c2a1b42f66547289621a7e87d7b5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872742"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="d94ca-103">cloudPcProvisioningPolicy：assign</span><span class="sxs-lookup"><span data-stu-id="d94ca-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="d94ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d94ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d94ca-105">将 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="d94ca-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="d94ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="d94ca-106">Permissions</span></span>

<span data-ttu-id="d94ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d94ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d94ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d94ca-109">Permission type</span></span>|<span data-ttu-id="d94ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d94ca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d94ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d94ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d94ca-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d94ca-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d94ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d94ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d94ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d94ca-114">Not supported.</span></span>|
|<span data-ttu-id="d94ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d94ca-115">Application</span></span>|<span data-ttu-id="d94ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d94ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d94ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d94ca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d94ca-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d94ca-118">Request headers</span></span>

|<span data-ttu-id="d94ca-119">名称</span><span class="sxs-lookup"><span data-stu-id="d94ca-119">Name</span></span>|<span data-ttu-id="d94ca-120">说明</span><span class="sxs-lookup"><span data-stu-id="d94ca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d94ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d94ca-121">Authorization</span></span>|<span data-ttu-id="d94ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d94ca-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d94ca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d94ca-124">Content-Type</span></span>|<span data-ttu-id="d94ca-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d94ca-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d94ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d94ca-127">Request body</span></span>

<span data-ttu-id="d94ca-128">在请求正文中，提供 [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d94ca-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="d94ca-129">下表显示创建 [cloudPcProvisioningPolicyAssignment 时所需的属性](../resources/cloudpcprovisioningpolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d94ca-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="d94ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="d94ca-130">Property</span></span>|<span data-ttu-id="d94ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="d94ca-131">Type</span></span>|<span data-ttu-id="d94ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="d94ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d94ca-133">id</span><span class="sxs-lookup"><span data-stu-id="d94ca-133">id</span></span>|<span data-ttu-id="d94ca-134">String</span><span class="sxs-lookup"><span data-stu-id="d94ca-134">String</span></span>|<span data-ttu-id="d94ca-135">设置策略分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="d94ca-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="d94ca-136">如果目标是用户组，则 ID 显示为 {policyId}_{groupId}。</span><span class="sxs-lookup"><span data-stu-id="d94ca-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="d94ca-137">target</span><span class="sxs-lookup"><span data-stu-id="d94ca-137">target</span></span>|[<span data-ttu-id="d94ca-138">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d94ca-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="d94ca-139">预配策略的分配目标。</span><span class="sxs-lookup"><span data-stu-id="d94ca-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="d94ca-140">目前，唯一支持的目标为用户组。</span><span class="sxs-lookup"><span data-stu-id="d94ca-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="d94ca-141">响应</span><span class="sxs-lookup"><span data-stu-id="d94ca-141">Response</span></span>

<span data-ttu-id="d94ca-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d94ca-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d94ca-143">示例</span><span class="sxs-lookup"><span data-stu-id="d94ca-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d94ca-144">请求</span><span class="sxs-lookup"><span data-stu-id="d94ca-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d94ca-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d94ca-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="d94ca-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d94ca-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d94ca-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d94ca-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d94ca-148">响应</span><span class="sxs-lookup"><span data-stu-id="d94ca-148">Response</span></span>

<span data-ttu-id="d94ca-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d94ca-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
