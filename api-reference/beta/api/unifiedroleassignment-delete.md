---
title: 删除 unifiedRoleAssignment
description: 删除 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 96bff141cc3f4dfb779335100a49a8fdf99edb00
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317068"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="6735b-103">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6735b-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="6735b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6735b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6735b-105">删除 [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6735b-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6735b-106">权限</span><span class="sxs-lookup"><span data-stu-id="6735b-106">Permissions</span></span>

<span data-ttu-id="6735b-107">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="6735b-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="6735b-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6735b-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6735b-109">支持的提供程序</span><span class="sxs-lookup"><span data-stu-id="6735b-109">Supported provider</span></span>      | <span data-ttu-id="6735b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6735b-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="6735b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6735b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6735b-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6735b-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="6735b-113">目录</span><span class="sxs-lookup"><span data-stu-id="6735b-113">Directory</span></span> | <span data-ttu-id="6735b-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6735b-114">RoleManagement.ReadWrite.Directory</span></span> | <span data-ttu-id="6735b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6735b-115">Not supported.</span></span>| <span data-ttu-id="6735b-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6735b-116">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="6735b-117">权利管理</span><span class="sxs-lookup"><span data-stu-id="6735b-117">Entitlement management</span></span> | <span data-ttu-id="6735b-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6735b-118">EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="6735b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6735b-119">Not supported.</span></span> | <span data-ttu-id="6735b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6735b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6735b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6735b-121">HTTP request</span></span>

<span data-ttu-id="6735b-122">从角色分配中删除一个目录：</span><span class="sxs-lookup"><span data-stu-id="6735b-122">Remove a role assignment from a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="6735b-123">从角色分配管理提供程序中删除以下权限：</span><span class="sxs-lookup"><span data-stu-id="6735b-123">Remove a role assignment from the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/entitlementManagement/roleAssignments/{id}
```


## <a name="request-headers"></a><span data-ttu-id="6735b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6735b-124">Request headers</span></span>

| <span data-ttu-id="6735b-125">名称</span><span class="sxs-lookup"><span data-stu-id="6735b-125">Name</span></span>          | <span data-ttu-id="6735b-126">说明</span><span class="sxs-lookup"><span data-stu-id="6735b-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6735b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6735b-127">Authorization</span></span> | <span data-ttu-id="6735b-128">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6735b-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6735b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6735b-129">Request body</span></span>

<span data-ttu-id="6735b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6735b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6735b-131">响应</span><span class="sxs-lookup"><span data-stu-id="6735b-131">Response</span></span>

<span data-ttu-id="6735b-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6735b-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6735b-134">示例</span><span class="sxs-lookup"><span data-stu-id="6735b-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6735b-135">请求</span><span class="sxs-lookup"><span data-stu-id="6735b-135">Request</span></span>

<span data-ttu-id="6735b-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6735b-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6735b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6735b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="6735b-138">C#</span><span class="sxs-lookup"><span data-stu-id="6735b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6735b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6735b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6735b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6735b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6735b-141">Java</span><span class="sxs-lookup"><span data-stu-id="6735b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6735b-142">响应</span><span class="sxs-lookup"><span data-stu-id="6735b-142">Response</span></span>

<span data-ttu-id="6735b-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6735b-143">The following is an example of the response.</span></span>

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


