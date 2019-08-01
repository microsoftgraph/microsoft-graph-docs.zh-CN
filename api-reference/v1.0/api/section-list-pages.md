---
title: 列出页面
description: 从指定分区中检索 page 对象的列表。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 8b1150c0470db5bc7d361b962432f8e78e87e7f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021478"
---
# <a name="list-pages"></a><span data-ttu-id="ac3aa-103">列出页面</span><span class="sxs-lookup"><span data-stu-id="ac3aa-103">List pages</span></span>

<span data-ttu-id="ac3aa-104">从指定分区中检索[page](../resources/page.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-104">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac3aa-105">权限</span><span class="sxs-lookup"><span data-stu-id="ac3aa-105">Permissions</span></span>
<span data-ttu-id="ac3aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac3aa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac3aa-108">Permission type</span></span>      | <span data-ttu-id="ac3aa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac3aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac3aa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac3aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac3aa-111">请参阅 "注意,"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="ac3aa-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac3aa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac3aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac3aa-113">注意: Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="ac3aa-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ac3aa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac3aa-114">Application</span></span> | <span data-ttu-id="ac3aa-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac3aa-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac3aa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac3aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ac3aa-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ac3aa-117">Optional query parameters</span></span>
<span data-ttu-id="ac3aa-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ac3aa-119">页面的默认查询返回订购的前20个页面`lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-119">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="ac3aa-120">如果默认查询返回20个以上`@odata.nextLink`的页面, 则该响应包含可用于对结果集进行分页的。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-120">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="ac3aa-121">`top`请求返回的最大页面数为100。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-121">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="ac3aa-122">默认响应将展开`parentSection`并选择节的`id`、 `name`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-122">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="ac3aa-123">页面`expand`的`parentNotebook`有效值为和`parentSection`。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-123">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac3aa-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac3aa-124">Request headers</span></span>
| <span data-ttu-id="ac3aa-125">名称</span><span class="sxs-lookup"><span data-stu-id="ac3aa-125">Name</span></span>       | <span data-ttu-id="ac3aa-126">类型</span><span class="sxs-lookup"><span data-stu-id="ac3aa-126">Type</span></span> | <span data-ttu-id="ac3aa-127">说明</span><span class="sxs-lookup"><span data-stu-id="ac3aa-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ac3aa-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac3aa-128">Authorization</span></span>  | <span data-ttu-id="ac3aa-129">string</span><span class="sxs-lookup"><span data-stu-id="ac3aa-129">string</span></span>  | <span data-ttu-id="ac3aa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac3aa-132">接受</span><span class="sxs-lookup"><span data-stu-id="ac3aa-132">Accept</span></span> | <span data-ttu-id="ac3aa-133">string</span><span class="sxs-lookup"><span data-stu-id="ac3aa-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ac3aa-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac3aa-134">Request body</span></span>
<span data-ttu-id="ac3aa-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac3aa-136">响应</span><span class="sxs-lookup"><span data-stu-id="ac3aa-136">Response</span></span>

<span data-ttu-id="ac3aa-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[page](../resources/page.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac3aa-138">示例</span><span class="sxs-lookup"><span data-stu-id="ac3aa-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac3aa-139">请求</span><span class="sxs-lookup"><span data-stu-id="ac3aa-139">Request</span></span>
<span data-ttu-id="ac3aa-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="ac3aa-141">响应</span><span class="sxs-lookup"><span data-stu-id="ac3aa-141">Response</span></span>
<span data-ttu-id="ac3aa-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac3aa-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
