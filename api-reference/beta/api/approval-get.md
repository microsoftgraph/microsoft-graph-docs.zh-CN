---
title: 获取审批
description: 检索审批对象的属性。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: da034f07aa83a483417161e0524661d97ca327e9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942598"
---
# <a name="get-approval"></a><span data-ttu-id="d2036-103">获取审批</span><span class="sxs-lookup"><span data-stu-id="d2036-103">Get approval</span></span>

<span data-ttu-id="d2036-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2036-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2036-105">检索 [审批对象的属性](../resources/approval.md) 。</span><span class="sxs-lookup"><span data-stu-id="d2036-105">Retrieve the properties of an [approval](../resources/approval.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2036-106">权限</span><span class="sxs-lookup"><span data-stu-id="d2036-106">Permissions</span></span>

<span data-ttu-id="d2036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2036-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2036-109">Permission type</span></span>                        | <span data-ttu-id="d2036-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2036-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2036-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2036-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2036-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2036-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d2036-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2036-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2036-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2036-114">Not supported.</span></span> |
| <span data-ttu-id="d2036-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2036-115">Application</span></span>                            | <span data-ttu-id="d2036-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2036-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2036-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2036-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2036-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2036-118">Request headers</span></span>

| <span data-ttu-id="d2036-119">名称</span><span class="sxs-lookup"><span data-stu-id="d2036-119">Name</span></span>      |<span data-ttu-id="d2036-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2036-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2036-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2036-121">Authorization</span></span> | <span data-ttu-id="d2036-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="d2036-122">Bearer \{token\}.</span></span> <span data-ttu-id="d2036-123">必填。</span><span class="sxs-lookup"><span data-stu-id="d2036-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2036-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2036-124">Request body</span></span>

<span data-ttu-id="d2036-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2036-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2036-126">响应</span><span class="sxs-lookup"><span data-stu-id="d2036-126">Response</span></span>

<span data-ttu-id="d2036-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/approval.md)请求的审批对象。</span><span class="sxs-lookup"><span data-stu-id="d2036-127">If successful, this method returns a `200 OK` response code and the requested [approval](../resources/approval.md) object in the response body.</span></span> <span data-ttu-id="d2036-128">但是，如果调用方没有正确的权限，该方法将返回 响应 `403 Forbidden` 代码。</span><span class="sxs-lookup"><span data-stu-id="d2036-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d2036-129">示例</span><span class="sxs-lookup"><span data-stu-id="d2036-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2036-130">请求</span><span class="sxs-lookup"><span data-stu-id="d2036-130">Request</span></span>

<span data-ttu-id="d2036-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d2036-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d2036-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2036-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approval"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489
```
# <a name="c"></a>[<span data-ttu-id="d2036-133">C#</span><span class="sxs-lookup"><span data-stu-id="d2036-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2036-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2036-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2036-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2036-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2036-136">Java</span><span class="sxs-lookup"><span data-stu-id="d2036-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d2036-137">响应</span><span class="sxs-lookup"><span data-stu-id="d2036-137">Response</span></span>

<span data-ttu-id="d2036-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2036-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d2036-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d2036-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


