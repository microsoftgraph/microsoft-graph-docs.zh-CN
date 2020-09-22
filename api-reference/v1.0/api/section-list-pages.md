---
title: 列出页面
description: 从指定分区中检索 page 对象的列表。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: b2b91e3983876f5c7ffd24adfb8b6539afb0b421
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088907"
---
# <a name="list-pages"></a><span data-ttu-id="5b324-103">列出页面</span><span class="sxs-lookup"><span data-stu-id="5b324-103">List pages</span></span>

<span data-ttu-id="5b324-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b324-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b324-105">从指定分区中检索 [page](../resources/page.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5b324-105">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b324-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b324-106">Permissions</span></span>
<span data-ttu-id="5b324-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b324-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b324-109">Permission type</span></span>      | <span data-ttu-id="5b324-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b324-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b324-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b324-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b324-112">请参阅 "注意，"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="5b324-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b324-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b324-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b324-114">注意： Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="5b324-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5b324-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b324-115">Application</span></span> | <span data-ttu-id="5b324-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b324-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b324-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b324-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b324-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5b324-118">Optional query parameters</span></span>
<span data-ttu-id="5b324-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5b324-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5b324-120">页面的默认查询返回订购的前20个页面 `lastModifiedTime desc` 。</span><span class="sxs-lookup"><span data-stu-id="5b324-120">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="5b324-121">如果默认查询返回20个以上的页面，则该响应包含 `@odata.nextLink` 可用于对结果集进行分页的。</span><span class="sxs-lookup"><span data-stu-id="5b324-121">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="5b324-122">请求返回的最大页面数 `top` 为100。</span><span class="sxs-lookup"><span data-stu-id="5b324-122">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="5b324-123">默认响应将展开 `parentSection` 并选择节的 `id` 、 `name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="5b324-123">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="5b324-124">`expand`页面的有效值为 `parentNotebook` 和 `parentSection` 。</span><span class="sxs-lookup"><span data-stu-id="5b324-124">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b324-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b324-125">Request headers</span></span>
| <span data-ttu-id="5b324-126">名称</span><span class="sxs-lookup"><span data-stu-id="5b324-126">Name</span></span>       | <span data-ttu-id="5b324-127">类型</span><span class="sxs-lookup"><span data-stu-id="5b324-127">Type</span></span> | <span data-ttu-id="5b324-128">说明</span><span class="sxs-lookup"><span data-stu-id="5b324-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b324-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b324-129">Authorization</span></span>  | <span data-ttu-id="5b324-130">string</span><span class="sxs-lookup"><span data-stu-id="5b324-130">string</span></span>  | <span data-ttu-id="5b324-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b324-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b324-133">接受</span><span class="sxs-lookup"><span data-stu-id="5b324-133">Accept</span></span> | <span data-ttu-id="5b324-134">string</span><span class="sxs-lookup"><span data-stu-id="5b324-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5b324-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b324-135">Request body</span></span>
<span data-ttu-id="5b324-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b324-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b324-137">响应</span><span class="sxs-lookup"><span data-stu-id="5b324-137">Response</span></span>

<span data-ttu-id="5b324-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [page](../resources/page.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5b324-138">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b324-139">示例</span><span class="sxs-lookup"><span data-stu-id="5b324-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b324-140">请求</span><span class="sxs-lookup"><span data-stu-id="5b324-140">Request</span></span>
<span data-ttu-id="5b324-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b324-141">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="5b324-142">响应</span><span class="sxs-lookup"><span data-stu-id="5b324-142">Response</span></span>
<span data-ttu-id="5b324-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b324-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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

