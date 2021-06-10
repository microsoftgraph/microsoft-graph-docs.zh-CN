---
title: 删除 accessPackage
description: 删除 accessPackage。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 710bbd3e015af5109b95905d6db68061de1506f5
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868866"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="0fede-103">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="0fede-103">Delete accessPackage</span></span>

<span data-ttu-id="0fede-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fede-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fede-105">删除 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fede-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="0fede-106">如果访问包有任何 **accessPackageAssignment**，则不能删除该访问包。</span><span class="sxs-lookup"><span data-stu-id="0fede-106">You cannot delete an access package if it has any **accessPackageAssignment**.</span></span> <span data-ttu-id="0fede-107">若要删除访问包 [，请首先](accesspackageassignment-list.md) 查询是否有带筛选器的分配，以指示特定访问包，例如 `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` ：。</span><span class="sxs-lookup"><span data-stu-id="0fede-107">To delete the access package, first [query if there are any assignments](accesspackageassignment-list.md) with a filter to indicate the specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span> <span data-ttu-id="0fede-108">若要详细了解如何删除仍处于已传递状态的工作分配，请参阅删除 [工作分配](accesspackageassignmentrequest-post.md#example-4-remove-an-assignment)。</span><span class="sxs-lookup"><span data-stu-id="0fede-108">For more information on how to remove assignments that are still in the delivered state, see [Remove an assignment](accesspackageassignmentrequest-post.md#example-4-remove-an-assignment).</span></span>


## <a name="permissions"></a><span data-ttu-id="0fede-109">权限</span><span class="sxs-lookup"><span data-stu-id="0fede-109">Permissions</span></span>

<span data-ttu-id="0fede-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fede-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fede-112">Permission type</span></span>                        | <span data-ttu-id="0fede-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fede-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0fede-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fede-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fede-115">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fede-115">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0fede-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fede-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fede-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fede-117">Not supported.</span></span> |
| <span data-ttu-id="0fede-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fede-118">Application</span></span>                            | <span data-ttu-id="0fede-119">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fede-119">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fede-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fede-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0fede-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fede-121">Request headers</span></span>

| <span data-ttu-id="0fede-122">名称</span><span class="sxs-lookup"><span data-stu-id="0fede-122">Name</span></span>          | <span data-ttu-id="0fede-123">说明</span><span class="sxs-lookup"><span data-stu-id="0fede-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0fede-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fede-124">Authorization</span></span> | <span data-ttu-id="0fede-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="0fede-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fede-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fede-127">Request body</span></span>

<span data-ttu-id="0fede-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fede-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fede-129">响应</span><span class="sxs-lookup"><span data-stu-id="0fede-129">Response</span></span>

<span data-ttu-id="0fede-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0fede-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fede-132">示例</span><span class="sxs-lookup"><span data-stu-id="0fede-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0fede-133">请求</span><span class="sxs-lookup"><span data-stu-id="0fede-133">Request</span></span>

<span data-ttu-id="0fede-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0fede-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fede-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fede-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="0fede-136">C#</span><span class="sxs-lookup"><span data-stu-id="0fede-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fede-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fede-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fede-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fede-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fede-139">Java</span><span class="sxs-lookup"><span data-stu-id="0fede-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fede-140">响应</span><span class="sxs-lookup"><span data-stu-id="0fede-140">Response</span></span>

<span data-ttu-id="0fede-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0fede-141">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


