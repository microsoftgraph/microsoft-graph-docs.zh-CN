---
author: rahmit
description: 从网站的 "网站页面" 列表中删除 sitePage。
ms.date: 05/07/2018
title: 从 SharePoint 网站中删除页面
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d573553ee87b70adfd1f2cde575ce6182dedf8b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044485"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="4c3c8-103">从网站的 "网站页面" 列表中删除页面</span><span class="sxs-lookup"><span data-stu-id="4c3c8-103">Delete page from the site pages list of a site</span></span>

<span data-ttu-id="4c3c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c3c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c3c8-105">从[网站][]的 "网站页面"[列表][]中删除[sitePage][] 。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="4c3c8-109">权限</span><span class="sxs-lookup"><span data-stu-id="4c3c8-109">Permissions</span></span>

<span data-ttu-id="4c3c8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="4c3c8-112">**注意：** 若要删除项，用户必须已授予应用程序对要删除的项的写入权限。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="4c3c8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c3c8-113">Permission type</span></span>      | <span data-ttu-id="4c3c8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c3c8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c3c8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c3c8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4c3c8-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c3c8-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c3c8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c3c8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c3c8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-118">Not supported.</span></span>    |
|<span data-ttu-id="4c3c8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c3c8-119">Application</span></span> | <span data-ttu-id="4c3c8-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c3c8-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c3c8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c3c8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4c3c8-122">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4c3c8-122">Optional request headers</span></span>

| <span data-ttu-id="4c3c8-123">名称</span><span class="sxs-lookup"><span data-stu-id="4c3c8-123">Name</span></span>       | <span data-ttu-id="4c3c8-124">值</span><span class="sxs-lookup"><span data-stu-id="4c3c8-124">Value</span></span> | <span data-ttu-id="4c3c8-125">说明</span><span class="sxs-lookup"><span data-stu-id="4c3c8-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="4c3c8-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="4c3c8-126">_if-match_</span></span> | <span data-ttu-id="4c3c8-127">etag</span><span class="sxs-lookup"><span data-stu-id="4c3c8-127">etag</span></span>  | <span data-ttu-id="4c3c8-128">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="4c3c8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c3c8-129">Request body</span></span>

<span data-ttu-id="4c3c8-130">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="4c3c8-131">响应</span><span class="sxs-lookup"><span data-stu-id="4c3c8-131">Response</span></span>

<span data-ttu-id="4c3c8-132">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有任何可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="4c3c8-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="4c3c8-133">示例</span><span class="sxs-lookup"><span data-stu-id="4c3c8-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="4c3c8-134">请求</span><span class="sxs-lookup"><span data-stu-id="4c3c8-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="4c3c8-135">响应</span><span class="sxs-lookup"><span data-stu-id="4c3c8-135">Response</span></span>

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


