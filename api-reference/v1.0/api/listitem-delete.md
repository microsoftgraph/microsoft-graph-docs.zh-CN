---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 80ecd3a9079e52ee9908f0211d0e283d993869b2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612965"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="d9606-102">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="d9606-102">Delete an item from a list</span></span>

<span data-ttu-id="d9606-103">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="d9606-103">Removes an item from a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="d9606-105">权限</span><span class="sxs-lookup"><span data-stu-id="d9606-105">Permissions</span></span>

<span data-ttu-id="d9606-106">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="d9606-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="d9606-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9606-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9606-109">Permission type</span></span>      | <span data-ttu-id="d9606-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9606-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9606-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9606-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9606-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9606-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9606-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9606-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9606-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9606-114">Not supported.</span></span>    |
|<span data-ttu-id="d9606-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9606-115">Application</span></span> | <span data-ttu-id="d9606-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9606-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9606-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9606-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="d9606-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d9606-118">Optional request headers</span></span>

| <span data-ttu-id="d9606-119">名称</span><span class="sxs-lookup"><span data-stu-id="d9606-119">Name</span></span>       | <span data-ttu-id="d9606-120">值</span><span class="sxs-lookup"><span data-stu-id="d9606-120">Value</span></span> | <span data-ttu-id="d9606-121">说明</span><span class="sxs-lookup"><span data-stu-id="d9606-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="d9606-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="d9606-122">_if-match_</span></span> | <span data-ttu-id="d9606-123">etag</span><span class="sxs-lookup"><span data-stu-id="d9606-123">etag</span></span>  | <span data-ttu-id="d9606-124">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="d9606-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="d9606-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9606-125">Request body</span></span>

<span data-ttu-id="d9606-126">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9606-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="d9606-127">示例</span><span class="sxs-lookup"><span data-stu-id="d9606-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="d9606-128">响应</span><span class="sxs-lookup"><span data-stu-id="d9606-128">Response</span></span>

<span data-ttu-id="d9606-129">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="d9606-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d9606-130">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d9606-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d9606-131">语言</span><span class="sxs-lookup"><span data-stu-id="d9606-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9606-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9606-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-site-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
