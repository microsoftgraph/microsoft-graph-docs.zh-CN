---
title: 删除 unifiedRoleAssignmentMultiple
description: 删除 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 85d721888b3f64f77533e6c83c53c84c943ec824
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444852"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="a9a35-103">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a9a35-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="a9a35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9a35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9a35-105">删除 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9a35-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="a9a35-106">这适用于支持多个主体和范围的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a9a35-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="a9a35-107">Microsoft Intune 就是这样的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a9a35-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9a35-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a9a35-108">Permissions</span></span>

<span data-ttu-id="a9a35-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9a35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9a35-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9a35-111">Permission type</span></span> | <span data-ttu-id="a9a35-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9a35-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="a9a35-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9a35-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a9a35-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9a35-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="a9a35-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9a35-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9a35-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9a35-116">Not supported.</span></span> |
| <span data-ttu-id="a9a35-117">Application</span><span class="sxs-lookup"><span data-stu-id="a9a35-117">Application</span></span> | <span data-ttu-id="a9a35-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9a35-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9a35-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9a35-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9a35-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9a35-120">Request headers</span></span>

| <span data-ttu-id="a9a35-121">名称</span><span class="sxs-lookup"><span data-stu-id="a9a35-121">Name</span></span> | <span data-ttu-id="a9a35-122">说明</span><span class="sxs-lookup"><span data-stu-id="a9a35-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="a9a35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9a35-123">Authorization</span></span> | <span data-ttu-id="a9a35-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a9a35-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9a35-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9a35-125">Request body</span></span>

<span data-ttu-id="a9a35-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9a35-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9a35-127">响应</span><span class="sxs-lookup"><span data-stu-id="a9a35-127">Response</span></span>

<span data-ttu-id="a9a35-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9a35-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9a35-130">示例</span><span class="sxs-lookup"><span data-stu-id="a9a35-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9a35-131">请求</span><span class="sxs-lookup"><span data-stu-id="a9a35-131">Request</span></span>

<span data-ttu-id="a9a35-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9a35-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9a35-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9a35-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="a9a35-134">C#</span><span class="sxs-lookup"><span data-stu-id="a9a35-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9a35-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9a35-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9a35-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9a35-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9a35-137">Java</span><span class="sxs-lookup"><span data-stu-id="a9a35-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9a35-138">响应</span><span class="sxs-lookup"><span data-stu-id="a9a35-138">Response</span></span>

<span data-ttu-id="a9a35-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a9a35-139">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


