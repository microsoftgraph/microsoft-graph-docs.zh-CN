---
title: 获取审批步骤
description: 检索 approvalStep 对象的属性。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f55ead753f23862f48e9c89703cc38010f8fbe99
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048048"
---
# <a name="get-approvalstep"></a><span data-ttu-id="f0ed4-103">获取审批步骤</span><span class="sxs-lookup"><span data-stu-id="f0ed4-103">Get approvalStep</span></span>

<span data-ttu-id="f0ed4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0ed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0ed4-105">检索 [approvalStep 对象](../resources/approvalstep.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-105">Retrieve the properties of an [approvalStep](../resources/approvalstep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0ed4-106">权限</span><span class="sxs-lookup"><span data-stu-id="f0ed4-106">Permissions</span></span>

<span data-ttu-id="f0ed4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0ed4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0ed4-109">Permission type</span></span>                        | <span data-ttu-id="f0ed4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0ed4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0ed4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0ed4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0ed4-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0ed4-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f0ed4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0ed4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ed4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-114">Not supported.</span></span> |
| <span data-ttu-id="f0ed4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0ed4-115">Application</span></span>                            | <span data-ttu-id="f0ed4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0ed4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0ed4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0ed4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0ed4-118">Request headers</span></span>

| <span data-ttu-id="f0ed4-119">名称</span><span class="sxs-lookup"><span data-stu-id="f0ed4-119">Name</span></span>      |<span data-ttu-id="f0ed4-120">说明</span><span class="sxs-lookup"><span data-stu-id="f0ed4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0ed4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ed4-121">Authorization</span></span> | <span data-ttu-id="f0ed4-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0ed4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0ed4-124">Request body</span></span>

<span data-ttu-id="f0ed4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0ed4-126">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed4-126">Response</span></span>

<span data-ttu-id="f0ed4-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [approvalStep](../resources/approvalstep.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-127">If successful, this method returns a `200 OK` response code and the [approvalStep](../resources/approvalstep.md) object in the response body.</span></span> <span data-ttu-id="f0ed4-128">但是，如果调用方没有正确的权限，该方法将返回 响应 `403 Forbidden` 代码。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f0ed4-129">示例</span><span class="sxs-lookup"><span data-stu-id="f0ed4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0ed4-130">请求</span><span class="sxs-lookup"><span data-stu-id="f0ed4-130">Request</span></span>

<span data-ttu-id="f0ed4-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-131">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="f0ed4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0ed4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="c"></a>[<span data-ttu-id="f0ed4-133">C#</span><span class="sxs-lookup"><span data-stu-id="f0ed4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0ed4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0ed4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0ed4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0ed4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0ed4-136">Java</span><span class="sxs-lookup"><span data-stu-id="f0ed4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="f0ed4-137">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed4-137">Response</span></span>

<span data-ttu-id="f0ed4-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f0ed4-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


