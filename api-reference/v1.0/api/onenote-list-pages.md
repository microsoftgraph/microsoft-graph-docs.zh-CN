---
title: 列出页面
description: 检索 page 对象的列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 22daf1f67fee7cc495bd0d4996d6291f3d75e2be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511311"
---
# <a name="list-pages"></a><span data-ttu-id="18109-103">列出页面</span><span class="sxs-lookup"><span data-stu-id="18109-103">List pages</span></span>

<span data-ttu-id="18109-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18109-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18109-105">检索[page](../resources/page.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="18109-105">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="18109-106">权限</span><span class="sxs-lookup"><span data-stu-id="18109-106">Permissions</span></span>
<span data-ttu-id="18109-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18109-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18109-109">Permission type</span></span>      | <span data-ttu-id="18109-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18109-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18109-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18109-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18109-112">请参阅 "注意，"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="18109-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="18109-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18109-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18109-114">注意： Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="18109-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="18109-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18109-115">Application</span></span> | <span data-ttu-id="18109-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18109-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18109-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18109-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18109-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="18109-118">Optional query parameters</span></span>
<span data-ttu-id="18109-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="18109-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="18109-120">页面的默认查询返回订购的前20个页面`lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="18109-120">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="18109-121">如果默认查询返回20个以上`@odata.nextLink`的页面，则该响应包含可用于对结果集进行分页的。</span><span class="sxs-lookup"><span data-stu-id="18109-121">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="18109-122">`top`请求返回的最大页面数为100。</span><span class="sxs-lookup"><span data-stu-id="18109-122">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="18109-123">默认响应将展开`parentSection`并选择节的`id`、 `displayName`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="18109-123">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="18109-124">页面`expand`的`parentNotebook`有效值为和`parentSection`。</span><span class="sxs-lookup"><span data-stu-id="18109-124">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18109-125">请求头</span><span class="sxs-lookup"><span data-stu-id="18109-125">Request headers</span></span>
| <span data-ttu-id="18109-126">名称</span><span class="sxs-lookup"><span data-stu-id="18109-126">Name</span></span>       | <span data-ttu-id="18109-127">类型</span><span class="sxs-lookup"><span data-stu-id="18109-127">Type</span></span> | <span data-ttu-id="18109-128">说明</span><span class="sxs-lookup"><span data-stu-id="18109-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18109-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="18109-129">Authorization</span></span>  | <span data-ttu-id="18109-130">string</span><span class="sxs-lookup"><span data-stu-id="18109-130">string</span></span>  | <span data-ttu-id="18109-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18109-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18109-133">接受</span><span class="sxs-lookup"><span data-stu-id="18109-133">Accept</span></span> | <span data-ttu-id="18109-134">string</span><span class="sxs-lookup"><span data-stu-id="18109-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="18109-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="18109-135">Request body</span></span>
<span data-ttu-id="18109-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18109-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18109-137">响应</span><span class="sxs-lookup"><span data-stu-id="18109-137">Response</span></span>

<span data-ttu-id="18109-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和[page](../resources/page.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="18109-138">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18109-139">示例</span><span class="sxs-lookup"><span data-stu-id="18109-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18109-140">请求</span><span class="sxs-lookup"><span data-stu-id="18109-140">Request</span></span>
<span data-ttu-id="18109-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18109-141">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="18109-142">响应</span><span class="sxs-lookup"><span data-stu-id="18109-142">Response</span></span>
<span data-ttu-id="18109-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18109-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
