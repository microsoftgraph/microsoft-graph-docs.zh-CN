---
title: 更新 approvalStep
description: 对 approvalStep 对象应用批准或拒绝决定。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b8ef436a9319e7a670e0aa5bdc728b39b53c2709
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942519"
---
# <a name="update-approvalstep"></a><span data-ttu-id="15e1c-103">更新 approvalStep</span><span class="sxs-lookup"><span data-stu-id="15e1c-103">Update approvalStep</span></span>

<span data-ttu-id="15e1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15e1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15e1c-105">对 approvalStep 对象应用 [批准或拒绝](../resources/approvalStep.md) 决定。</span><span class="sxs-lookup"><span data-stu-id="15e1c-105">Apply approve or deny decision on an [approvalStep](../resources/approvalStep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="15e1c-106">权限</span><span class="sxs-lookup"><span data-stu-id="15e1c-106">Permissions</span></span>

<span data-ttu-id="15e1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15e1c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="15e1c-109">Permission type</span></span>                        | <span data-ttu-id="15e1c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15e1c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15e1c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15e1c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="15e1c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15e1c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="15e1c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15e1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15e1c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="15e1c-114">Not supported.</span></span> |
| <span data-ttu-id="15e1c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="15e1c-115">Application</span></span>                            | <span data-ttu-id="15e1c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="15e1c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15e1c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15e1c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="15e1c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="15e1c-118">Request headers</span></span>

| <span data-ttu-id="15e1c-119">名称</span><span class="sxs-lookup"><span data-stu-id="15e1c-119">Name</span></span>      |<span data-ttu-id="15e1c-120">说明</span><span class="sxs-lookup"><span data-stu-id="15e1c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15e1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="15e1c-121">Authorization</span></span> | <span data-ttu-id="15e1c-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="15e1c-122">Bearer \{token\}.</span></span> <span data-ttu-id="15e1c-123">必填。</span><span class="sxs-lookup"><span data-stu-id="15e1c-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15e1c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="15e1c-124">Request body</span></span>

<span data-ttu-id="15e1c-125">下表显示了此方法所需的属性。</span><span class="sxs-lookup"><span data-stu-id="15e1c-125">The following table shows the properties that are required for this method.</span></span>

| <span data-ttu-id="15e1c-126">属性</span><span class="sxs-lookup"><span data-stu-id="15e1c-126">Property</span></span>       | <span data-ttu-id="15e1c-127">类型</span><span class="sxs-lookup"><span data-stu-id="15e1c-127">Type</span></span>    |<span data-ttu-id="15e1c-128">说明</span><span class="sxs-lookup"><span data-stu-id="15e1c-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15e1c-129">reviewResult</span><span class="sxs-lookup"><span data-stu-id="15e1c-129">reviewResult</span></span> | <span data-ttu-id="15e1c-130">String</span><span class="sxs-lookup"><span data-stu-id="15e1c-130">String</span></span> | <span data-ttu-id="15e1c-131">审批者的决定。</span><span class="sxs-lookup"><span data-stu-id="15e1c-131">Decision of the approver.</span></span> <span data-ttu-id="15e1c-132">可取值为：`Approve`、`Deny`。</span><span class="sxs-lookup"><span data-stu-id="15e1c-132">Possible values are: `Approve`, `Deny`.</span></span>|
| <span data-ttu-id="15e1c-133">justification</span><span class="sxs-lookup"><span data-stu-id="15e1c-133">justification</span></span> | <span data-ttu-id="15e1c-134">String</span><span class="sxs-lookup"><span data-stu-id="15e1c-134">String</span></span> | <span data-ttu-id="15e1c-135">与审批者的决定相关的理由。</span><span class="sxs-lookup"><span data-stu-id="15e1c-135">Justification related to the approver's decision.</span></span> |


## <a name="response"></a><span data-ttu-id="15e1c-136">响应</span><span class="sxs-lookup"><span data-stu-id="15e1c-136">Response</span></span>

<span data-ttu-id="15e1c-137">如果成功，此方法在响应 `204 No Content` 正文中返回 响应代码。</span><span class="sxs-lookup"><span data-stu-id="15e1c-137">If successful, this method returns a `204 No Content` response code in the response body.</span></span> <span data-ttu-id="15e1c-138">但是，如果调用方没有适当的权限，该方法将返回 响应代码，或者如果未找到审批 `403 Forbidden` ID，则该方法返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="15e1c-138">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code, or if the approval id is not found, the method returns `404 Not found`.</span></span> <span data-ttu-id="15e1c-139">如果请求已在同一审批阶段由另一个审批者批准，该方法在响应 `409 Conflict` 正文中返回。</span><span class="sxs-lookup"><span data-stu-id="15e1c-139">If the request has already been approved by another approver in the same approval stage, the method returns `409 Conflict` in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15e1c-140">示例</span><span class="sxs-lookup"><span data-stu-id="15e1c-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15e1c-141">请求</span><span class="sxs-lookup"><span data-stu-id="15e1c-141">Request</span></span>

<span data-ttu-id="15e1c-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15e1c-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="15e1c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="15e1c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="objective-c"></a>[<span data-ttu-id="15e1c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15e1c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstep-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="15e1c-145">响应</span><span class="sxs-lookup"><span data-stu-id="15e1c-145">Response</span></span>

<span data-ttu-id="15e1c-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="15e1c-146">The following is an example of the response.</span></span>

> <span data-ttu-id="15e1c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="15e1c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-Type: application/json
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
