---
title: 列出页面
description: 从指定分区中检索 page 对象列表。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8d5aae356a703968ca05317e653cad5b9a931161
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951367"
---
# <a name="list-pages"></a><span data-ttu-id="9939a-103">列出页面</span><span class="sxs-lookup"><span data-stu-id="9939a-103">List pages</span></span>

<span data-ttu-id="9939a-104">从指定分区中检索 [page](../resources/page.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9939a-104">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="9939a-105">权限</span><span class="sxs-lookup"><span data-stu-id="9939a-105">Permissions</span></span>
<span data-ttu-id="9939a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9939a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9939a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9939a-108">Permission type</span></span>      | <span data-ttu-id="9939a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9939a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9939a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9939a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9939a-111">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9939a-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9939a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9939a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9939a-113">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9939a-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9939a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9939a-114">Application</span></span> | <span data-ttu-id="9939a-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9939a-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9939a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9939a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9939a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9939a-117">Optional query parameters</span></span>
<span data-ttu-id="9939a-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9939a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9939a-p102">对页面的默认查询返回按照 `lastModifiedTime desc` 排序的前 20 个页面。如果默认查询返回的页面超过 20 个，响应将包含 `@odata.nextLink`，可以使用它逐页查看结果集。`top` 请求最多可返回 100 个页面。</span><span class="sxs-lookup"><span data-stu-id="9939a-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="9939a-p103">默认响应将展开 `parentSection` 并选择分区的 `id`、`name`、和 `self` 属性。页面的有效 `expand` 值为 `parentNotebook` 和 `parentSection`。</span><span class="sxs-lookup"><span data-stu-id="9939a-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9939a-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="9939a-124">Request headers</span></span>
| <span data-ttu-id="9939a-125">名称</span><span class="sxs-lookup"><span data-stu-id="9939a-125">Name</span></span>       | <span data-ttu-id="9939a-126">类型</span><span class="sxs-lookup"><span data-stu-id="9939a-126">Type</span></span> | <span data-ttu-id="9939a-127">说明</span><span class="sxs-lookup"><span data-stu-id="9939a-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9939a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9939a-128">Authorization</span></span>  | <span data-ttu-id="9939a-129">string</span><span class="sxs-lookup"><span data-stu-id="9939a-129">string</span></span>  | <span data-ttu-id="9939a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9939a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9939a-132">Accept</span><span class="sxs-lookup"><span data-stu-id="9939a-132">Accept</span></span> | <span data-ttu-id="9939a-133">string</span><span class="sxs-lookup"><span data-stu-id="9939a-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9939a-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="9939a-134">Request body</span></span>
<span data-ttu-id="9939a-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9939a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9939a-136">响应</span><span class="sxs-lookup"><span data-stu-id="9939a-136">Response</span></span>

<span data-ttu-id="9939a-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [page](../resources/page.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9939a-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9939a-138">示例</span><span class="sxs-lookup"><span data-stu-id="9939a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9939a-139">请求</span><span class="sxs-lookup"><span data-stu-id="9939a-139">Request</span></span>
<span data-ttu-id="9939a-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9939a-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="9939a-141">响应</span><span class="sxs-lookup"><span data-stu-id="9939a-141">Response</span></span>
<span data-ttu-id="9939a-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9939a-142">Here is an example of the response.</span></span> <span data-ttu-id="9939a-143">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9939a-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="9939a-144">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9939a-144">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
    {
      "title": "title-value",
      "createdByAppId": "createdByAppId-value",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      },
      "contentUrl": "contentUrl-value",
      "content": "content-value",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
