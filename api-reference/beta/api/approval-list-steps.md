---
title: 列出 approvalSteps
description: 列出与审批对象关联的审批步骤。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 797d2715dd2c273c5673e608a4794fc0c56a6f45
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961357"
---
# <a name="list-approvalsteps"></a><span data-ttu-id="d28bd-103">列出 approvalSteps</span><span class="sxs-lookup"><span data-stu-id="d28bd-103">List approvalSteps</span></span>

<span data-ttu-id="d28bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d28bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28bd-105">在[Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，列出与审批对象关联的[approvalStep](../resources/approvalstep.md)对象。 [](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="d28bd-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), lists the [approvalStep](../resources/approvalstep.md) objects associated with an [approval](../resources/approval.md) object.</span></span>  <span data-ttu-id="d28bd-106">此调用由审批者进行，提供访问包分配请求 [的标识符](../resources/accesspackageassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="d28bd-106">This call can be made by an approver, providing the identifier of the [access package assignment request](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d28bd-107">权限</span><span class="sxs-lookup"><span data-stu-id="d28bd-107">Permissions</span></span>

<span data-ttu-id="d28bd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d28bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d28bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d28bd-110">Permission type</span></span>                        | <span data-ttu-id="d28bd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d28bd-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d28bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d28bd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d28bd-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d28bd-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d28bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d28bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d28bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d28bd-115">Not supported.</span></span> |
| <span data-ttu-id="d28bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d28bd-116">Application</span></span>                            | <span data-ttu-id="d28bd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d28bd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d28bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d28bd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps
```

## <a name="request-headers"></a><span data-ttu-id="d28bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d28bd-119">Request headers</span></span>

| <span data-ttu-id="d28bd-120">名称</span><span class="sxs-lookup"><span data-stu-id="d28bd-120">Name</span></span>      |<span data-ttu-id="d28bd-121">说明</span><span class="sxs-lookup"><span data-stu-id="d28bd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d28bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d28bd-122">Authorization</span></span> | <span data-ttu-id="d28bd-123">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="d28bd-123">Bearer \{token\}.</span></span> <span data-ttu-id="d28bd-124">必需。</span><span class="sxs-lookup"><span data-stu-id="d28bd-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d28bd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d28bd-125">Request body</span></span>

<span data-ttu-id="d28bd-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d28bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d28bd-127">响应</span><span class="sxs-lookup"><span data-stu-id="d28bd-127">Response</span></span>

<span data-ttu-id="d28bd-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [approvalStep](../resources/approvalstep.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d28bd-128">If successful, this method returns a `200 OK` response code and a collection of the [approvalStep](../resources/approvalstep.md) objects in the response body.</span></span> <span data-ttu-id="d28bd-129">但是，如果调用方没有正确的权限，该方法将返回 响应 `403 Forbidden` 代码。</span><span class="sxs-lookup"><span data-stu-id="d28bd-129">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d28bd-130">示例</span><span class="sxs-lookup"><span data-stu-id="d28bd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d28bd-131">请求</span><span class="sxs-lookup"><span data-stu-id="d28bd-131">Request</span></span>

<span data-ttu-id="d28bd-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d28bd-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d28bd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d28bd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps
```
# <a name="c"></a>[<span data-ttu-id="d28bd-134">C#</span><span class="sxs-lookup"><span data-stu-id="d28bd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d28bd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d28bd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d28bd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d28bd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d28bd-137">Java</span><span class="sxs-lookup"><span data-stu-id="d28bd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d28bd-138">响应</span><span class="sxs-lookup"><span data-stu-id="d28bd-138">Response</span></span>

<span data-ttu-id="d28bd-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d28bd-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d28bd-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d28bd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
            "displayName": null,
            "reviewedDateTime": null,
            "reviewResult": "NotReviewed",
            "status": "InProgress",
            "assignedToMe": true,
            "justification": "",
            "reviewedBy": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List approvalstep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


