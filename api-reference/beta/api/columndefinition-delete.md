---
author: swapnil1993
title: 删除 columnDefinition
description: 从网站、列表或内容类型中删除列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 771123af410d5c0c63038f6d032e5c56874d058f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952233"
---
# <a name="delete-columndefinition"></a><span data-ttu-id="a9e23-103">删除 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="a9e23-103">Delete columnDefinition</span></span>
<span data-ttu-id="a9e23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9e23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="a9e23-105">从[网站、][columndefinition]列表[或][][内容类型][]中删除[列][contentType]。</span><span class="sxs-lookup"><span data-stu-id="a9e23-105">Remove a [column][columndefinition] from a [site][], [list][] or [content type][contentType].</span></span>


## <a name="permissions"></a><span data-ttu-id="a9e23-106">权限</span><span class="sxs-lookup"><span data-stu-id="a9e23-106">Permissions</span></span>
<span data-ttu-id="a9e23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a9e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="a9e23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9e23-109">Permission type</span></span>      | <span data-ttu-id="a9e23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9e23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9e23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9e23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9e23-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a9e23-112">Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="a9e23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9e23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9e23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9e23-114">Not supported.</span></span>    |
|<span data-ttu-id="a9e23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9e23-115">Application</span></span> | <span data-ttu-id="a9e23-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a9e23-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9e23-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9e23-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/columns/{column-id}
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a><span data-ttu-id="a9e23-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9e23-118">Request headers</span></span>
|<span data-ttu-id="a9e23-119">名称</span><span class="sxs-lookup"><span data-stu-id="a9e23-119">Name</span></span>|<span data-ttu-id="a9e23-120">说明</span><span class="sxs-lookup"><span data-stu-id="a9e23-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a9e23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9e23-121">Authorization</span></span>|<span data-ttu-id="a9e23-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9e23-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9e23-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9e23-124">Request body</span></span>
<span data-ttu-id="a9e23-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9e23-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9e23-126">响应</span><span class="sxs-lookup"><span data-stu-id="a9e23-126">Response</span></span>

<span data-ttu-id="a9e23-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a9e23-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9e23-128">示例</span><span class="sxs-lookup"><span data-stu-id="a9e23-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9e23-129">请求</span><span class="sxs-lookup"><span data-stu-id="a9e23-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a9e23-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9e23-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[<span data-ttu-id="a9e23-131">C#</span><span class="sxs-lookup"><span data-stu-id="a9e23-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-columns-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9e23-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9e23-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-columns-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9e23-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9e23-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-columns-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9e23-134">Java</span><span class="sxs-lookup"><span data-stu-id="a9e23-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-columns-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9e23-135">响应</span><span class="sxs-lookup"><span data-stu-id="a9e23-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[columndefinition]: ../resources/columndefinition.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
