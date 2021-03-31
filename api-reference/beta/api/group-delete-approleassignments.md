---
title: 从组中删除 appRoleAssignment
description: 删除已授予组的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: f352bcddfc08dd91e819eebc2b6803bb01eb779e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468896"
---
# <a name="delete-an-approleassignment-granted-to-a-group"></a><span data-ttu-id="d0d4f-103">删除授予组的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d0d4f-103">Delete an appRoleAssignment granted to a group</span></span>

<span data-ttu-id="d0d4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0d4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0d4f-105">删除[已授予组的 appRoleAssignment。](../resources/approleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d0d4f-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a group has been granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0d4f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0d4f-106">Permissions</span></span>

<span data-ttu-id="d0d4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0d4f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0d4f-109">Permission type</span></span>      | <span data-ttu-id="d0d4f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0d4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0d4f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0d4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0d4f-112">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0d4f-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0d4f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0d4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0d4f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-114">Not supported.</span></span>    |
|<span data-ttu-id="d0d4f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0d4f-115">Application</span></span> | <span data-ttu-id="d0d4f-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0d4f-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0d4f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0d4f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="d0d4f-118">作为最佳实践，我们建议通过资源服务主体的关系（而不是分配的用户、组或服务主体的关系）删除应用程序 `appRoleAssignedTo`  `appRoleAssignments` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0d4f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0d4f-119">Request headers</span></span>

| <span data-ttu-id="d0d4f-120">名称</span><span class="sxs-lookup"><span data-stu-id="d0d4f-120">Name</span></span>       | <span data-ttu-id="d0d4f-121">类型</span><span class="sxs-lookup"><span data-stu-id="d0d4f-121">Type</span></span> | <span data-ttu-id="d0d4f-122">说明</span><span class="sxs-lookup"><span data-stu-id="d0d4f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0d4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0d4f-123">Authorization</span></span>  | <span data-ttu-id="d0d4f-124">string</span><span class="sxs-lookup"><span data-stu-id="d0d4f-124">string</span></span>  | <span data-ttu-id="d0d4f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0d4f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0d4f-127">Request body</span></span>

<span data-ttu-id="d0d4f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0d4f-129">响应</span><span class="sxs-lookup"><span data-stu-id="d0d4f-129">Response</span></span>

<span data-ttu-id="d0d4f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0d4f-132">示例</span><span class="sxs-lookup"><span data-stu-id="d0d4f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0d4f-133">请求</span><span class="sxs-lookup"><span data-stu-id="d0d4f-133">Request</span></span>

<span data-ttu-id="d0d4f-134">下面是一个请求删除应用示例角色分配。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0d4f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0d4f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/groups/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="d0d4f-136">C#</span><span class="sxs-lookup"><span data-stu-id="d0d4f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0d4f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0d4f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0d4f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0d4f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0d4f-139">Java</span><span class="sxs-lookup"><span data-stu-id="d0d4f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0d4f-140">响应</span><span class="sxs-lookup"><span data-stu-id="d0d4f-140">Response</span></span>

<span data-ttu-id="d0d4f-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d0d4f-141">The following is an example of the response.</span></span>

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

