---
title: 删除授予用户的 appRoleAssignment
description: 删除已授予用户的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 2f0e0b06c4dd48c321094539d5cf9fd02d44f96f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468812"
---
# <a name="delete-an-approleassignment-granted-to-a-user"></a><span data-ttu-id="f2e31-103">删除授予用户的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f2e31-103">Delete an appRoleAssignment granted to a user</span></span>

<span data-ttu-id="f2e31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2e31-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2e31-105">删除[已授予用户的 appRoleAssignment。](../resources/approleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f2e31-105">Delete an [appRoleAssignment](../resources/approleassignment.md) that has been granted to a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2e31-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2e31-106">Permissions</span></span>

<span data-ttu-id="f2e31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2e31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2e31-109">Permission type</span></span>      | <span data-ttu-id="f2e31-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2e31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2e31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2e31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2e31-112">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2e31-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2e31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2e31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2e31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2e31-114">Not supported.</span></span>    |
|<span data-ttu-id="f2e31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2e31-115">Application</span></span> | <span data-ttu-id="f2e31-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e31-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2e31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2e31-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="f2e31-118">作为最佳实践，我们建议通过资源服务主体的关系（而不是分配的用户、组或服务主体的关系）删除应用程序 `appRoleAssignedTo`  `appRoleAssignments` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="f2e31-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2e31-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2e31-119">Request headers</span></span>

| <span data-ttu-id="f2e31-120">名称</span><span class="sxs-lookup"><span data-stu-id="f2e31-120">Name</span></span>       | <span data-ttu-id="f2e31-121">类型</span><span class="sxs-lookup"><span data-stu-id="f2e31-121">Type</span></span> | <span data-ttu-id="f2e31-122">说明</span><span class="sxs-lookup"><span data-stu-id="f2e31-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2e31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e31-123">Authorization</span></span>  | <span data-ttu-id="f2e31-124">string</span><span class="sxs-lookup"><span data-stu-id="f2e31-124">string</span></span>  | <span data-ttu-id="f2e31-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2e31-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2e31-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2e31-127">Request body</span></span>

<span data-ttu-id="f2e31-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2e31-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2e31-129">响应</span><span class="sxs-lookup"><span data-stu-id="f2e31-129">Response</span></span>

<span data-ttu-id="f2e31-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f2e31-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2e31-132">示例</span><span class="sxs-lookup"><span data-stu-id="f2e31-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2e31-133">请求</span><span class="sxs-lookup"><span data-stu-id="f2e31-133">Request</span></span>

<span data-ttu-id="f2e31-134">下面是一个请求删除应用示例角色分配。</span><span class="sxs-lookup"><span data-stu-id="f2e31-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2e31-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2e31-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="f2e31-136">C#</span><span class="sxs-lookup"><span data-stu-id="f2e31-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2e31-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2e31-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2e31-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2e31-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2e31-139">Java</span><span class="sxs-lookup"><span data-stu-id="f2e31-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2e31-140">响应</span><span class="sxs-lookup"><span data-stu-id="f2e31-140">Response</span></span>

<span data-ttu-id="f2e31-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2e31-141">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

