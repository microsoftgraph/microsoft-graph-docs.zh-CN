---
title: 更新 approvalStep
description: 对 approvalStep 对象应用批准或拒绝决定。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 16c2796e94678b4ca0362c3be86268f69cdbcedb
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760752"
---
# <a name="update-approvalstep"></a><span data-ttu-id="e0b5e-103">更新 approvalStep</span><span class="sxs-lookup"><span data-stu-id="e0b5e-103">Update approvalStep</span></span>

<span data-ttu-id="e0b5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0b5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0b5e-105">对 approvalStep 对象应用 [批准或拒绝](../resources/approvalStep.md) 决定。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-105">Apply approve or deny decision on an [approvalStep](../resources/approvalStep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0b5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0b5e-106">Permissions</span></span>

<span data-ttu-id="e0b5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0b5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0b5e-109">Permission type</span></span>                        | <span data-ttu-id="e0b5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0b5e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0b5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0b5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0b5e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b5e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e0b5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0b5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0b5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-114">Not supported.</span></span> |
| <span data-ttu-id="e0b5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0b5e-115">Application</span></span>                            | <span data-ttu-id="e0b5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0b5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0b5e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0b5e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0b5e-118">Request headers</span></span>

| <span data-ttu-id="e0b5e-119">名称</span><span class="sxs-lookup"><span data-stu-id="e0b5e-119">Name</span></span>      |<span data-ttu-id="e0b5e-120">说明</span><span class="sxs-lookup"><span data-stu-id="e0b5e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0b5e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0b5e-121">Authorization</span></span> | <span data-ttu-id="e0b5e-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-122">Bearer \{token\}.</span></span> <span data-ttu-id="e0b5e-123">必需。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0b5e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0b5e-124">Request body</span></span>

<span data-ttu-id="e0b5e-125">下表显示了此方法所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-125">The following table shows the properties that are required for this method.</span></span>

| <span data-ttu-id="e0b5e-126">属性</span><span class="sxs-lookup"><span data-stu-id="e0b5e-126">Property</span></span>       | <span data-ttu-id="e0b5e-127">类型</span><span class="sxs-lookup"><span data-stu-id="e0b5e-127">Type</span></span>    |<span data-ttu-id="e0b5e-128">说明</span><span class="sxs-lookup"><span data-stu-id="e0b5e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0b5e-129">reviewResult</span><span class="sxs-lookup"><span data-stu-id="e0b5e-129">reviewResult</span></span> | <span data-ttu-id="e0b5e-130">String</span><span class="sxs-lookup"><span data-stu-id="e0b5e-130">String</span></span> | <span data-ttu-id="e0b5e-131">审批者的决定。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-131">Decision of the approver.</span></span> <span data-ttu-id="e0b5e-132">可取值为：`Approve`、`Deny`。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-132">Possible values are: `Approve`, `Deny`.</span></span>|
| <span data-ttu-id="e0b5e-133">justification</span><span class="sxs-lookup"><span data-stu-id="e0b5e-133">justification</span></span> | <span data-ttu-id="e0b5e-134">String</span><span class="sxs-lookup"><span data-stu-id="e0b5e-134">String</span></span> | <span data-ttu-id="e0b5e-135">与审批者的决定相关的理由。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-135">Justification related to the approver's decision.</span></span> |


## <a name="response"></a><span data-ttu-id="e0b5e-136">响应</span><span class="sxs-lookup"><span data-stu-id="e0b5e-136">Response</span></span>

<span data-ttu-id="e0b5e-137">如果成功，此方法在响应 `204 No Content` 正文中返回 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-137">If successful, this method returns a `204 No Content` response code in the response body.</span></span> <span data-ttu-id="e0b5e-138">但是，如果调用方没有适当的权限，该方法将返回 响应代码，或者如果未找到审批 `403 Forbidden` ID，则该方法返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-138">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code, or if the approval id is not found, the method returns `404 Not found`.</span></span> <span data-ttu-id="e0b5e-139">如果请求已在同一审批阶段由另一个审批者批准，该方法在响应 `409 Conflict` 正文中返回。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-139">If the request has already been approved by another approver in the same approval stage, the method returns `409 Conflict` in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0b5e-140">示例</span><span class="sxs-lookup"><span data-stu-id="e0b5e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0b5e-141">请求</span><span class="sxs-lookup"><span data-stu-id="e0b5e-141">Request</span></span>

<span data-ttu-id="e0b5e-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
---


### <a name="response"></a><span data-ttu-id="e0b5e-143">响应</span><span class="sxs-lookup"><span data-stu-id="e0b5e-143">Response</span></span>

<span data-ttu-id="e0b5e-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-144">The following is an example of the response.</span></span>

> <span data-ttu-id="e0b5e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0b5e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
