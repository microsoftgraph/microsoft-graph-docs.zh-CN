---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: 从 SharePoint 网站中删除页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b4ac336999484f6af97e41d08caa926fae4c055f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950022"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="3c085-102">从网站的网站的页面列表中删除页</span><span class="sxs-lookup"><span data-stu-id="3c085-102">Delete page from the site pages list of a site</span></span>

> <span data-ttu-id="3c085-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c085-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c085-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c085-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c085-105">从[网站][]中网站的页面[列表][]中删除[sitePage][] 。</span><span class="sxs-lookup"><span data-stu-id="3c085-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="3c085-109">权限</span><span class="sxs-lookup"><span data-stu-id="3c085-109">Permissions</span></span>

<span data-ttu-id="3c085-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c085-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="3c085-112">**注意：** 若要删除项，用户必须已授予对要删除的项目的应用程序写入访问。</span><span class="sxs-lookup"><span data-stu-id="3c085-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="3c085-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c085-113">Permission type</span></span>      | <span data-ttu-id="3c085-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c085-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c085-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c085-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3c085-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c085-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c085-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c085-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c085-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c085-118">Not supported.</span></span>    |
|<span data-ttu-id="3c085-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c085-119">Application</span></span> | <span data-ttu-id="3c085-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c085-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c085-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c085-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="3c085-122">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="3c085-122">Optional request headers</span></span>

| <span data-ttu-id="3c085-123">名称</span><span class="sxs-lookup"><span data-stu-id="3c085-123">Name</span></span>       | <span data-ttu-id="3c085-124">值</span><span class="sxs-lookup"><span data-stu-id="3c085-124">Value</span></span> | <span data-ttu-id="3c085-125">说明</span><span class="sxs-lookup"><span data-stu-id="3c085-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="3c085-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="3c085-126">_if-match_</span></span> | <span data-ttu-id="3c085-127">etag</span><span class="sxs-lookup"><span data-stu-id="3c085-127">etag</span></span>  | <span data-ttu-id="3c085-128">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="3c085-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="3c085-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c085-129">Request body</span></span>

<span data-ttu-id="3c085-130">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c085-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="3c085-131">响应</span><span class="sxs-lookup"><span data-stu-id="3c085-131">Response</span></span>

<span data-ttu-id="3c085-132">如果成功，此呼叫将返回`204 No Content`以指示已删除资源和没有要返回的响应。</span><span class="sxs-lookup"><span data-stu-id="3c085-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="3c085-133">示例</span><span class="sxs-lookup"><span data-stu-id="3c085-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="3c085-134">请求</span><span class="sxs-lookup"><span data-stu-id="3c085-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="3c085-135">响应</span><span class="sxs-lookup"><span data-stu-id="3c085-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
