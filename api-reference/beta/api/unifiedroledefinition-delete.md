---
title: 删除 unifiedRoleDefinition
description: 删除 unifiedRoleDefinition 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e64dfdc90152675b18bda72cc17effc57e1df681
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461589"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="14b65-103">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="14b65-103">Delete unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14b65-104">删除[unifiedRoleDefinition](../resources/unifiedRoleDefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14b65-104">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14b65-105">权限</span><span class="sxs-lookup"><span data-stu-id="14b65-105">Permissions</span></span>

<span data-ttu-id="14b65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14b65-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="14b65-108">Permission type</span></span>                        | <span data-ttu-id="14b65-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14b65-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14b65-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14b65-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="14b65-111">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="14b65-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="14b65-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14b65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14b65-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="14b65-113">Not supported.</span></span> |
| <span data-ttu-id="14b65-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="14b65-114">Application</span></span>                            | <span data-ttu-id="14b65-115">RoleManagement、RoleManagement、目录</span><span class="sxs-lookup"><span data-stu-id="14b65-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="14b65-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14b65-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="14b65-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="14b65-117">Request headers</span></span>

| <span data-ttu-id="14b65-118">名称</span><span class="sxs-lookup"><span data-stu-id="14b65-118">Name</span></span>          | <span data-ttu-id="14b65-119">说明</span><span class="sxs-lookup"><span data-stu-id="14b65-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="14b65-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b65-120">Authorization</span></span> | <span data-ttu-id="14b65-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="14b65-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14b65-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="14b65-122">Request body</span></span>

<span data-ttu-id="14b65-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14b65-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14b65-124">响应</span><span class="sxs-lookup"><span data-stu-id="14b65-124">Response</span></span>

<span data-ttu-id="14b65-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="14b65-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b65-127">示例</span><span class="sxs-lookup"><span data-stu-id="14b65-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="14b65-128">请求</span><span class="sxs-lookup"><span data-stu-id="14b65-128">Request</span></span>

<span data-ttu-id="14b65-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14b65-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="14b65-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="14b65-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="14b65-131">C#</span><span class="sxs-lookup"><span data-stu-id="14b65-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14b65-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14b65-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="14b65-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="14b65-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14b65-134">响应</span><span class="sxs-lookup"><span data-stu-id="14b65-134">Response</span></span>

<span data-ttu-id="14b65-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14b65-135">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
