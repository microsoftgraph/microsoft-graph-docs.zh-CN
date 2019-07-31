---
author: rahmit
description: 从网站的 "网站页面" 列表中删除 sitePage。
ms.date: 05/07/2018
title: 从 SharePoint 网站中删除页面
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bdf3dacabb99d5dfcfe47dcb954ff1cfd0b62ccb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977858"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="33331-103">从网站的 "网站页面" 列表中删除页面</span><span class="sxs-lookup"><span data-stu-id="33331-103">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33331-104">从[网站][]的 "网站页面"[列表][]中删除[sitePage][] 。</span><span class="sxs-lookup"><span data-stu-id="33331-104">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="33331-108">权限</span><span class="sxs-lookup"><span data-stu-id="33331-108">Permissions</span></span>

<span data-ttu-id="33331-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="33331-111">**注意:** 若要删除项, 用户必须已授予应用程序对要删除的项的写入权限。</span><span class="sxs-lookup"><span data-stu-id="33331-111">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="33331-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="33331-112">Permission type</span></span>      | <span data-ttu-id="33331-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33331-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33331-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33331-114">Delegated (work or school account)</span></span> | <span data-ttu-id="33331-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33331-115">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="33331-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33331-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33331-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="33331-117">Not supported.</span></span>    |
|<span data-ttu-id="33331-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="33331-118">Application</span></span> | <span data-ttu-id="33331-119">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33331-119">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33331-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33331-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="33331-121">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="33331-121">Optional request headers</span></span>

| <span data-ttu-id="33331-122">名称</span><span class="sxs-lookup"><span data-stu-id="33331-122">Name</span></span>       | <span data-ttu-id="33331-123">值</span><span class="sxs-lookup"><span data-stu-id="33331-123">Value</span></span> | <span data-ttu-id="33331-124">说明</span><span class="sxs-lookup"><span data-stu-id="33331-124">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="33331-125">_if-match_</span><span class="sxs-lookup"><span data-stu-id="33331-125">_if-match_</span></span> | <span data-ttu-id="33331-126">etag</span><span class="sxs-lookup"><span data-stu-id="33331-126">etag</span></span>  | <span data-ttu-id="33331-127">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="33331-127">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="33331-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="33331-128">Request body</span></span>

<span data-ttu-id="33331-129">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="33331-129">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="33331-130">响应</span><span class="sxs-lookup"><span data-stu-id="33331-130">Response</span></span>

<span data-ttu-id="33331-131">如果成功, 此调用将返回`204 No Content`响应, 表示资源已被删除, 没有任何可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="33331-131">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="33331-132">示例</span><span class="sxs-lookup"><span data-stu-id="33331-132">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="33331-133">请求</span><span class="sxs-lookup"><span data-stu-id="33331-133">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="33331-134">响应</span><span class="sxs-lookup"><span data-stu-id="33331-134">Response</span></span>

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
