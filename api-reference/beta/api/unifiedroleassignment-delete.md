---
title: 删除 unifiedRoleAssignment
description: 删除 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 01ce2f1aa786c0f62147a370c00f6aed4d9d0bc6
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351032"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="9ea36-103">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9ea36-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="9ea36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ea36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea36-105">删除 [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ea36-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea36-106">权限</span><span class="sxs-lookup"><span data-stu-id="9ea36-106">Permissions</span></span>

<span data-ttu-id="9ea36-107">根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。</span><span class="sxs-lookup"><span data-stu-id="9ea36-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="9ea36-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ea36-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="9ea36-109">对于 Azure AD (提供程序) 目录</span><span class="sxs-lookup"><span data-stu-id="9ea36-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="9ea36-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ea36-110">Permission type</span></span>      | <span data-ttu-id="9ea36-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ea36-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ea36-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea36-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ea36-113">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9ea36-113">RoleManagement.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="9ea36-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea36-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ea36-115">Not supported.</span></span>    |
|<span data-ttu-id="9ea36-116">Application</span><span class="sxs-lookup"><span data-stu-id="9ea36-116">Application</span></span> | <span data-ttu-id="9ea36-117">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9ea36-117">RoleManagement.ReadWrite.Directory</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="9ea36-118">对于权利管理提供程序</span><span class="sxs-lookup"><span data-stu-id="9ea36-118">For Entitlement management provider</span></span>

|<span data-ttu-id="9ea36-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ea36-119">Permission type</span></span>      | <span data-ttu-id="9ea36-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ea36-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ea36-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea36-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ea36-122">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea36-122">EntitlementManagement.ReadWrite.All</span></span>  |
|<span data-ttu-id="9ea36-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea36-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ea36-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ea36-124">Not supported.</span></span>    |
|<span data-ttu-id="9ea36-125">Application</span><span class="sxs-lookup"><span data-stu-id="9ea36-125">Application</span></span> | <span data-ttu-id="9ea36-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ea36-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ea36-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ea36-127">HTTP request</span></span>

<span data-ttu-id="9ea36-128">从角色分配中删除一个目录：</span><span class="sxs-lookup"><span data-stu-id="9ea36-128">Remove a role assignment from a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="9ea36-129">从角色分配管理提供程序中删除以下权限：</span><span class="sxs-lookup"><span data-stu-id="9ea36-129">Remove a role assignment from the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/entitlementManagement/roleAssignments/{id}
```


## <a name="request-headers"></a><span data-ttu-id="9ea36-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ea36-130">Request headers</span></span>

| <span data-ttu-id="9ea36-131">名称</span><span class="sxs-lookup"><span data-stu-id="9ea36-131">Name</span></span>          | <span data-ttu-id="9ea36-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ea36-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9ea36-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ea36-133">Authorization</span></span> | <span data-ttu-id="9ea36-134">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9ea36-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ea36-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ea36-135">Request body</span></span>

<span data-ttu-id="9ea36-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ea36-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ea36-137">响应</span><span class="sxs-lookup"><span data-stu-id="9ea36-137">Response</span></span>

<span data-ttu-id="9ea36-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9ea36-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea36-140">示例</span><span class="sxs-lookup"><span data-stu-id="9ea36-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ea36-141">请求</span><span class="sxs-lookup"><span data-stu-id="9ea36-141">Request</span></span>

<span data-ttu-id="9ea36-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ea36-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ea36-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ea36-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="9ea36-144">C#</span><span class="sxs-lookup"><span data-stu-id="9ea36-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ea36-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ea36-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ea36-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ea36-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ea36-147">Java</span><span class="sxs-lookup"><span data-stu-id="9ea36-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ea36-148">响应</span><span class="sxs-lookup"><span data-stu-id="9ea36-148">Response</span></span>

<span data-ttu-id="9ea36-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ea36-149">The following is an example of the response.</span></span>

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


