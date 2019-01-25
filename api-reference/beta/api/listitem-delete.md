---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 13c6504753eb5987db8c0282ef2f59bca72a8d43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530144"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="f7ebc-102">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="f7ebc-102">Delete an item from a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7ebc-103">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="f7ebc-105">权限</span><span class="sxs-lookup"><span data-stu-id="f7ebc-105">Permissions</span></span>

<span data-ttu-id="f7ebc-106">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="f7ebc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ebc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7ebc-109">Permission type</span></span>      | <span data-ttu-id="f7ebc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7ebc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7ebc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ebc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7ebc-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ebc-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7ebc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ebc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7ebc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-114">Not supported.</span></span>    |
|<span data-ttu-id="f7ebc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7ebc-115">Application</span></span> | <span data-ttu-id="f7ebc-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ebc-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7ebc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7ebc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f7ebc-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f7ebc-118">Optional request headers</span></span>

| <span data-ttu-id="f7ebc-119">名称</span><span class="sxs-lookup"><span data-stu-id="f7ebc-119">Name</span></span>       | <span data-ttu-id="f7ebc-120">值</span><span class="sxs-lookup"><span data-stu-id="f7ebc-120">Value</span></span> | <span data-ttu-id="f7ebc-121">说明</span><span class="sxs-lookup"><span data-stu-id="f7ebc-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="f7ebc-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="f7ebc-122">_if-match_</span></span> | <span data-ttu-id="f7ebc-123">etag</span><span class="sxs-lookup"><span data-stu-id="f7ebc-123">etag</span></span>  | <span data-ttu-id="f7ebc-124">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="f7ebc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7ebc-125">Request body</span></span>

<span data-ttu-id="f7ebc-126">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="f7ebc-127">示例</span><span class="sxs-lookup"><span data-stu-id="f7ebc-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="f7ebc-128">响应</span><span class="sxs-lookup"><span data-stu-id="f7ebc-128">Response</span></span>

<span data-ttu-id="f7ebc-129">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="f7ebc-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
