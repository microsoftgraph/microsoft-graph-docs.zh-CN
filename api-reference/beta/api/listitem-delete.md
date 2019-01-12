---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1b61c9359ca349a7f7882a204e8e474aba00444b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968461"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="c7ebb-102">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="c7ebb-102">Delete an item from a list</span></span>

> <span data-ttu-id="c7ebb-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7ebb-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7ebb-105">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-105">Removes an item from a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="c7ebb-107">权限</span><span class="sxs-lookup"><span data-stu-id="c7ebb-107">Permissions</span></span>

<span data-ttu-id="c7ebb-108">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="c7ebb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ebb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7ebb-111">Permission type</span></span>      | <span data-ttu-id="c7ebb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7ebb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7ebb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7ebb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c7ebb-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ebb-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7ebb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7ebb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7ebb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-116">Not supported.</span></span>    |
|<span data-ttu-id="c7ebb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7ebb-117">Application</span></span> | <span data-ttu-id="c7ebb-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ebb-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7ebb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7ebb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c7ebb-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c7ebb-120">Optional request headers</span></span>

| <span data-ttu-id="c7ebb-121">名称</span><span class="sxs-lookup"><span data-stu-id="c7ebb-121">Name</span></span>       | <span data-ttu-id="c7ebb-122">值</span><span class="sxs-lookup"><span data-stu-id="c7ebb-122">Value</span></span> | <span data-ttu-id="c7ebb-123">说明</span><span class="sxs-lookup"><span data-stu-id="c7ebb-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="c7ebb-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="c7ebb-124">_if-match_</span></span> | <span data-ttu-id="c7ebb-125">etag</span><span class="sxs-lookup"><span data-stu-id="c7ebb-125">etag</span></span>  | <span data-ttu-id="c7ebb-126">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="c7ebb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7ebb-127">Request body</span></span>

<span data-ttu-id="c7ebb-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="c7ebb-129">示例</span><span class="sxs-lookup"><span data-stu-id="c7ebb-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="c7ebb-130">响应</span><span class="sxs-lookup"><span data-stu-id="c7ebb-130">Response</span></span>

<span data-ttu-id="c7ebb-131">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="c7ebb-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
