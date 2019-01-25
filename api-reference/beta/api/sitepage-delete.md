---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: 从 SharePoint 网站中删除页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513023"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="74ce2-102">从网站的网站的页面列表中删除页</span><span class="sxs-lookup"><span data-stu-id="74ce2-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ce2-103">从[网站][]中网站的页面[列表][]中删除[sitePage][] 。</span><span class="sxs-lookup"><span data-stu-id="74ce2-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="74ce2-107">权限</span><span class="sxs-lookup"><span data-stu-id="74ce2-107">Permissions</span></span>

<span data-ttu-id="74ce2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74ce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="74ce2-110">**注意：** 若要删除项，用户必须已授予对要删除的项目的应用程序写入访问。</span><span class="sxs-lookup"><span data-stu-id="74ce2-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="74ce2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74ce2-111">Permission type</span></span>      | <span data-ttu-id="74ce2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74ce2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74ce2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74ce2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="74ce2-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ce2-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="74ce2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74ce2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74ce2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74ce2-116">Not supported.</span></span>    |
|<span data-ttu-id="74ce2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74ce2-117">Application</span></span> | <span data-ttu-id="74ce2-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ce2-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74ce2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74ce2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="74ce2-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="74ce2-120">Optional request headers</span></span>

| <span data-ttu-id="74ce2-121">名称</span><span class="sxs-lookup"><span data-stu-id="74ce2-121">Name</span></span>       | <span data-ttu-id="74ce2-122">值</span><span class="sxs-lookup"><span data-stu-id="74ce2-122">Value</span></span> | <span data-ttu-id="74ce2-123">说明</span><span class="sxs-lookup"><span data-stu-id="74ce2-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="74ce2-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="74ce2-124">_if-match_</span></span> | <span data-ttu-id="74ce2-125">etag</span><span class="sxs-lookup"><span data-stu-id="74ce2-125">etag</span></span>  | <span data-ttu-id="74ce2-126">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="74ce2-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="74ce2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74ce2-127">Request body</span></span>

<span data-ttu-id="74ce2-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="74ce2-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="74ce2-129">响应</span><span class="sxs-lookup"><span data-stu-id="74ce2-129">Response</span></span>

<span data-ttu-id="74ce2-130">如果成功，此呼叫将返回`204 No Content`以指示已删除资源和没有要返回的响应。</span><span class="sxs-lookup"><span data-stu-id="74ce2-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="74ce2-131">示例</span><span class="sxs-lookup"><span data-stu-id="74ce2-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="74ce2-132">请求</span><span class="sxs-lookup"><span data-stu-id="74ce2-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="74ce2-133">响应</span><span class="sxs-lookup"><span data-stu-id="74ce2-133">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
