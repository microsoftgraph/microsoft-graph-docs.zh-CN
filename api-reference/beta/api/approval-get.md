---
title: 获取审批
description: 检索审批对象的属性。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 083064a405525a33855340bcf920900e3d70ca91
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961364"
---
# <a name="get-approval"></a><span data-ttu-id="61b14-103">获取审批</span><span class="sxs-lookup"><span data-stu-id="61b14-103">Get approval</span></span>

<span data-ttu-id="61b14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61b14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61b14-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索 [审批对象](../resources/approval.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="61b14-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieves the properties of an [approval](../resources/approval.md) object.</span></span>  <span data-ttu-id="61b14-106">此调用由审批者进行，提供访问包分配请求 [的标识符](../resources/accesspackageassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="61b14-106">This call can be made by an approver, providing the identifier of the [access package assignment request](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="61b14-107">权限</span><span class="sxs-lookup"><span data-stu-id="61b14-107">Permissions</span></span>

<span data-ttu-id="61b14-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61b14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61b14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61b14-110">Permission type</span></span>                        | <span data-ttu-id="61b14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61b14-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61b14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61b14-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="61b14-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61b14-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="61b14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61b14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61b14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61b14-115">Not supported.</span></span> |
| <span data-ttu-id="61b14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61b14-116">Application</span></span>                            | <span data-ttu-id="61b14-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="61b14-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61b14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61b14-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}
```

## <a name="request-headers"></a><span data-ttu-id="61b14-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="61b14-119">Request headers</span></span>

| <span data-ttu-id="61b14-120">名称</span><span class="sxs-lookup"><span data-stu-id="61b14-120">Name</span></span>      |<span data-ttu-id="61b14-121">说明</span><span class="sxs-lookup"><span data-stu-id="61b14-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61b14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61b14-122">Authorization</span></span> | <span data-ttu-id="61b14-123">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="61b14-123">Bearer \{token\}.</span></span> <span data-ttu-id="61b14-124">必需。</span><span class="sxs-lookup"><span data-stu-id="61b14-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61b14-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="61b14-125">Request body</span></span>

<span data-ttu-id="61b14-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61b14-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61b14-127">响应</span><span class="sxs-lookup"><span data-stu-id="61b14-127">Response</span></span>

<span data-ttu-id="61b14-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/approval.md)请求的审批对象。</span><span class="sxs-lookup"><span data-stu-id="61b14-128">If successful, this method returns a `200 OK` response code and the requested [approval](../resources/approval.md) object in the response body.</span></span> <span data-ttu-id="61b14-129">但是，如果调用方没有正确的权限，该方法将返回 响应 `403 Forbidden` 代码。</span><span class="sxs-lookup"><span data-stu-id="61b14-129">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="61b14-130">示例</span><span class="sxs-lookup"><span data-stu-id="61b14-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61b14-131">请求</span><span class="sxs-lookup"><span data-stu-id="61b14-131">Request</span></span>

<span data-ttu-id="61b14-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61b14-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="61b14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="61b14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approval"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489
```
# <a name="c"></a>[<span data-ttu-id="61b14-134">C#</span><span class="sxs-lookup"><span data-stu-id="61b14-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61b14-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61b14-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61b14-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61b14-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61b14-137">Java</span><span class="sxs-lookup"><span data-stu-id="61b14-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="61b14-138">响应</span><span class="sxs-lookup"><span data-stu-id="61b14-138">Response</span></span>

<span data-ttu-id="61b14-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61b14-139">The following is an example of the response.</span></span>

> <span data-ttu-id="61b14-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61b14-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approval"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "abd306ef-f7b2-4a10-9fd1-493454322489",
    "steps": [
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
  "description": "Get approval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


