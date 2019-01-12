---
title: 列出页面
description: 检索 page 对象列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 7448672cdb736d84c6f0c24ea47d66a651026540
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979682"
---
# <a name="list-pages"></a><span data-ttu-id="2b86c-103">列出页面</span><span class="sxs-lookup"><span data-stu-id="2b86c-103">List pages</span></span>

> <span data-ttu-id="2b86c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2b86c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b86c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b86c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b86c-106">检索 [page](../resources/page.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="2b86c-106">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b86c-107">权限</span><span class="sxs-lookup"><span data-stu-id="2b86c-107">Permissions</span></span>
<span data-ttu-id="2b86c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b86c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b86c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b86c-110">Permission type</span></span>      | <span data-ttu-id="2b86c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b86c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b86c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b86c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b86c-113">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b86c-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b86c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b86c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b86c-115">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b86c-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2b86c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b86c-116">Application</span></span> | <span data-ttu-id="2b86c-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b86c-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b86c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b86c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b86c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2b86c-119">Optional query parameters</span></span>
<span data-ttu-id="2b86c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2b86c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2b86c-p103">对页面的默认查询返回按照 `lastModifiedTime desc` 排序的前 20 个页面。如果默认查询返回的页面超过 20 个，响应将包含 `@odata.nextLink`，可以使用它逐页查看结果集。`top` 请求最多可返回 100 个页面。</span><span class="sxs-lookup"><span data-stu-id="2b86c-p103">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="2b86c-p104">默认响应将展开 `parentSection` 并选择分区的 `id`、`displayName`、和 `self` 属性。页面的有效 `expand` 值为 `parentNotebook` 和 `parentSection`。</span><span class="sxs-lookup"><span data-stu-id="2b86c-p104">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b86c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b86c-126">Request headers</span></span>
| <span data-ttu-id="2b86c-127">名称</span><span class="sxs-lookup"><span data-stu-id="2b86c-127">Name</span></span>       | <span data-ttu-id="2b86c-128">类型</span><span class="sxs-lookup"><span data-stu-id="2b86c-128">Type</span></span> | <span data-ttu-id="2b86c-129">说明</span><span class="sxs-lookup"><span data-stu-id="2b86c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b86c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b86c-130">Authorization</span></span>  | <span data-ttu-id="2b86c-131">string</span><span class="sxs-lookup"><span data-stu-id="2b86c-131">string</span></span>  | <span data-ttu-id="2b86c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b86c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b86c-134">Accept</span><span class="sxs-lookup"><span data-stu-id="2b86c-134">Accept</span></span> | <span data-ttu-id="2b86c-135">string</span><span class="sxs-lookup"><span data-stu-id="2b86c-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2b86c-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b86c-136">Request body</span></span>
<span data-ttu-id="2b86c-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b86c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b86c-138">响应</span><span class="sxs-lookup"><span data-stu-id="2b86c-138">Response</span></span>

<span data-ttu-id="2b86c-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [page](../resources/page.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b86c-139">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b86c-140">示例</span><span class="sxs-lookup"><span data-stu-id="2b86c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b86c-141">请求</span><span class="sxs-lookup"><span data-stu-id="2b86c-141">Request</span></span>
<span data-ttu-id="2b86c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b86c-142">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="2b86c-143">响应</span><span class="sxs-lookup"><span data-stu-id="2b86c-143">Response</span></span>
<span data-ttu-id="2b86c-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2b86c-144">Here is an example of the response.</span></span> <span data-ttu-id="2b86c-145">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2b86c-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="2b86c-146">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b86c-146">All of the properties will be returned from an actual call.</span></span>
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
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
