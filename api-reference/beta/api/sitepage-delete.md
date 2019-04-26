---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: 从 SharePoint 网站中删除页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d5c38a5f5b96a100cfbae0eba30f957b079568e5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330140"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="38b71-102">从网站的 "网站页面" 列表中删除页面</span><span class="sxs-lookup"><span data-stu-id="38b71-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38b71-103">从[网站][]的 "网站页面"[列表][]中删除[sitePage][] 。</span><span class="sxs-lookup"><span data-stu-id="38b71-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="38b71-107">权限</span><span class="sxs-lookup"><span data-stu-id="38b71-107">Permissions</span></span>

<span data-ttu-id="38b71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38b71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="38b71-110">**注意:** 若要删除项, 用户必须已授予应用程序对要删除的项的写入权限。</span><span class="sxs-lookup"><span data-stu-id="38b71-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="38b71-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38b71-111">Permission type</span></span>      | <span data-ttu-id="38b71-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38b71-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38b71-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38b71-113">Delegated (work or school account)</span></span> | <span data-ttu-id="38b71-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38b71-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="38b71-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38b71-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38b71-116">Not supported.</span></span>    |
|<span data-ttu-id="38b71-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38b71-117">Application</span></span> | <span data-ttu-id="38b71-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38b71-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38b71-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38b71-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="38b71-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="38b71-120">Optional request headers</span></span>

| <span data-ttu-id="38b71-121">名称</span><span class="sxs-lookup"><span data-stu-id="38b71-121">Name</span></span>       | <span data-ttu-id="38b71-122">值</span><span class="sxs-lookup"><span data-stu-id="38b71-122">Value</span></span> | <span data-ttu-id="38b71-123">说明</span><span class="sxs-lookup"><span data-stu-id="38b71-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="38b71-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="38b71-124">_if-match_</span></span> | <span data-ttu-id="38b71-125">etag</span><span class="sxs-lookup"><span data-stu-id="38b71-125">etag</span></span>  | <span data-ttu-id="38b71-126">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="38b71-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="38b71-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38b71-127">Request body</span></span>

<span data-ttu-id="38b71-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="38b71-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="38b71-129">响应</span><span class="sxs-lookup"><span data-stu-id="38b71-129">Response</span></span>

<span data-ttu-id="38b71-130">如果成功, 此调用将返回`204 No Content`响应, 表示资源已被删除, 没有任何可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="38b71-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="38b71-131">示例</span><span class="sxs-lookup"><span data-stu-id="38b71-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="38b71-132">请求</span><span class="sxs-lookup"><span data-stu-id="38b71-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="38b71-133">响应</span><span class="sxs-lookup"><span data-stu-id="38b71-133">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": []
}
-->
