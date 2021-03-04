---
title: 删除 unifiedRoleAssignment
description: 删除 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 865d18f0278084ecf884ead909374eeccaaace54
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444883"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="40029-103">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="40029-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="40029-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40029-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40029-105">删除 [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40029-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40029-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="40029-106">Permissions</span></span>

<span data-ttu-id="40029-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40029-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40029-109">Permission type</span></span>                        | <span data-ttu-id="40029-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40029-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="40029-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40029-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40029-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="40029-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="40029-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40029-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40029-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40029-114">Not supported.</span></span> |
| <span data-ttu-id="40029-115">Application</span><span class="sxs-lookup"><span data-stu-id="40029-115">Application</span></span>                            | <span data-ttu-id="40029-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="40029-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="40029-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40029-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40029-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="40029-118">Request headers</span></span>

| <span data-ttu-id="40029-119">名称</span><span class="sxs-lookup"><span data-stu-id="40029-119">Name</span></span>          | <span data-ttu-id="40029-120">说明</span><span class="sxs-lookup"><span data-stu-id="40029-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="40029-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40029-121">Authorization</span></span> | <span data-ttu-id="40029-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="40029-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="40029-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="40029-123">Request body</span></span>

<span data-ttu-id="40029-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40029-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40029-125">响应</span><span class="sxs-lookup"><span data-stu-id="40029-125">Response</span></span>

<span data-ttu-id="40029-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="40029-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40029-128">示例</span><span class="sxs-lookup"><span data-stu-id="40029-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="40029-129">请求</span><span class="sxs-lookup"><span data-stu-id="40029-129">Request</span></span>

<span data-ttu-id="40029-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40029-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40029-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="40029-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="40029-132">C#</span><span class="sxs-lookup"><span data-stu-id="40029-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40029-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40029-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40029-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40029-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40029-135">Java</span><span class="sxs-lookup"><span data-stu-id="40029-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40029-136">响应</span><span class="sxs-lookup"><span data-stu-id="40029-136">Response</span></span>

<span data-ttu-id="40029-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40029-137">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


