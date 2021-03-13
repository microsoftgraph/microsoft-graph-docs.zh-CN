---
author: swapnil1993
title: 删除 columnDefinition
description: 从内容类型中删除列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 65c96523d084911510e5ff337c096ccf73016f0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770992"
---
# <a name="delete-columndefinition"></a><span data-ttu-id="84bac-103">删除 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="84bac-103">Delete columnDefinition</span></span>
<span data-ttu-id="84bac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84bac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="84bac-105">从[列表或][columndefinition][网站内容][]类型[中删除][][列][contentType]。</span><span class="sxs-lookup"><span data-stu-id="84bac-105">Remove a [column][columndefinition] from a [list][] or a [site][] [content type][contentType].</span></span>


## <a name="permissions"></a><span data-ttu-id="84bac-106">权限</span><span class="sxs-lookup"><span data-stu-id="84bac-106">Permissions</span></span>
<span data-ttu-id="84bac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="84bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="84bac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="84bac-109">Permission type</span></span>      | <span data-ttu-id="84bac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84bac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84bac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84bac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84bac-112">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="84bac-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="84bac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84bac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84bac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="84bac-114">Not supported.</span></span>    |
|<span data-ttu-id="84bac-115">Application</span><span class="sxs-lookup"><span data-stu-id="84bac-115">Application</span></span> | <span data-ttu-id="84bac-116">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="84bac-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84bac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84bac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a><span data-ttu-id="84bac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="84bac-118">Request headers</span></span>
|<span data-ttu-id="84bac-119">名称</span><span class="sxs-lookup"><span data-stu-id="84bac-119">Name</span></span>|<span data-ttu-id="84bac-120">说明</span><span class="sxs-lookup"><span data-stu-id="84bac-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84bac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84bac-121">Authorization</span></span>|<span data-ttu-id="84bac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84bac-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84bac-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="84bac-124">Request body</span></span>
<span data-ttu-id="84bac-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84bac-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84bac-126">响应</span><span class="sxs-lookup"><span data-stu-id="84bac-126">Response</span></span>

<span data-ttu-id="84bac-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="84bac-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84bac-128">示例</span><span class="sxs-lookup"><span data-stu-id="84bac-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="84bac-129">请求</span><span class="sxs-lookup"><span data-stu-id="84bac-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="84bac-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="84bac-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[<span data-ttu-id="84bac-131">C#</span><span class="sxs-lookup"><span data-stu-id="84bac-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-columns-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84bac-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84bac-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-columns-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84bac-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84bac-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-columns-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84bac-134">Java</span><span class="sxs-lookup"><span data-stu-id="84bac-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-columns-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84bac-135">响应</span><span class="sxs-lookup"><span data-stu-id="84bac-135">Response</span></span>

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
