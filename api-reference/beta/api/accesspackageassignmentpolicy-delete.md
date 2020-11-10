---
title: 删除 accessPackageAssignmentPolicy
description: 删除 accessPackageAssignmentPolicy。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 042a0389308e1f68171bea3586daf6ced7a7a090
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952212"
---
# <a name="delete-accesspackageassignmentpolicy"></a><span data-ttu-id="d9b76-103">删除 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="d9b76-103">Delete accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="d9b76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9b76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9b76-105">在 " [AZURE AD 权限管理](../resources/entitlementmanagement-root.md)" 中，删除 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="d9b76-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), delete an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9b76-106">权限</span><span class="sxs-lookup"><span data-stu-id="d9b76-106">Permissions</span></span>

<span data-ttu-id="d9b76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9b76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9b76-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9b76-109">Permission type</span></span>                        | <span data-ttu-id="d9b76-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9b76-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9b76-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9b76-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9b76-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9b76-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d9b76-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9b76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9b76-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9b76-114">Not supported.</span></span> |
| <span data-ttu-id="d9b76-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9b76-115">Application</span></span>                            | <span data-ttu-id="d9b76-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9b76-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9b76-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9b76-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d9b76-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9b76-118">Request headers</span></span>

| <span data-ttu-id="d9b76-119">名称</span><span class="sxs-lookup"><span data-stu-id="d9b76-119">Name</span></span>          | <span data-ttu-id="d9b76-120">说明</span><span class="sxs-lookup"><span data-stu-id="d9b76-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d9b76-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9b76-121">Authorization</span></span> | <span data-ttu-id="d9b76-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="d9b76-122">Bearer \{token\}.</span></span> <span data-ttu-id="d9b76-123">必填。</span><span class="sxs-lookup"><span data-stu-id="d9b76-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9b76-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9b76-124">Request body</span></span>

<span data-ttu-id="d9b76-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9b76-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9b76-126">响应</span><span class="sxs-lookup"><span data-stu-id="d9b76-126">Response</span></span>

<span data-ttu-id="d9b76-127">如果成功，此方法将返回204无内容响应代码。</span><span class="sxs-lookup"><span data-stu-id="d9b76-127">If successful, this method returns a 204 No Content response code.</span></span> <span data-ttu-id="d9b76-128">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d9b76-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9b76-129">示例</span><span class="sxs-lookup"><span data-stu-id="d9b76-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9b76-130">请求</span><span class="sxs-lookup"><span data-stu-id="d9b76-130">Request</span></span>

<span data-ttu-id="d9b76-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9b76-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9b76-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9b76-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackageassignmentpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="d9b76-133">C#</span><span class="sxs-lookup"><span data-stu-id="d9b76-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9b76-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9b76-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9b76-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9b76-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9b76-136">Java</span><span class="sxs-lookup"><span data-stu-id="d9b76-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9b76-137">响应</span><span class="sxs-lookup"><span data-stu-id="d9b76-137">Response</span></span>

<span data-ttu-id="d9b76-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9b76-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


