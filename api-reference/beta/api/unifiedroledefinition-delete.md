---
title: 删除 unifiedRoleDefinition
description: 删除 unifiedRoleDefinition 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 86c020c5baeba9e492fd975df3ba1bc67aa5adc8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968995"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="0a398-103">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0a398-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="0a398-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a398-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a398-105">删除 [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a398-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a398-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a398-106">Permissions</span></span>

<span data-ttu-id="0a398-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a398-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a398-109">Permission type</span></span>                        | <span data-ttu-id="0a398-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a398-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a398-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a398-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a398-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="0a398-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="0a398-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a398-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a398-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a398-114">Not supported.</span></span> |
| <span data-ttu-id="0a398-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a398-115">Application</span></span>                            | <span data-ttu-id="0a398-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="0a398-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a398-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a398-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="0a398-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a398-118">Request headers</span></span>

| <span data-ttu-id="0a398-119">名称</span><span class="sxs-lookup"><span data-stu-id="0a398-119">Name</span></span>          | <span data-ttu-id="0a398-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a398-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0a398-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a398-121">Authorization</span></span> | <span data-ttu-id="0a398-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0a398-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a398-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a398-123">Request body</span></span>

<span data-ttu-id="0a398-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a398-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a398-125">响应</span><span class="sxs-lookup"><span data-stu-id="0a398-125">Response</span></span>

<span data-ttu-id="0a398-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0a398-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a398-128">示例</span><span class="sxs-lookup"><span data-stu-id="0a398-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a398-129">请求</span><span class="sxs-lookup"><span data-stu-id="0a398-129">Request</span></span>

<span data-ttu-id="0a398-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a398-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a398-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a398-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="0a398-132">C#</span><span class="sxs-lookup"><span data-stu-id="0a398-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a398-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a398-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a398-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a398-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a398-135">响应</span><span class="sxs-lookup"><span data-stu-id="0a398-135">Response</span></span>

<span data-ttu-id="0a398-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a398-136">The following is an example of the response.</span></span>

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


