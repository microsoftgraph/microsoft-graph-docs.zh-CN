---
title: 列出页面
description: 从指定分区中检索 page 对象的列表。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e2e1f506883a177716d3b91519d1ce2a8f85f04d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336079"
---
# <a name="list-pages"></a><span data-ttu-id="97131-103">列出页面</span><span class="sxs-lookup"><span data-stu-id="97131-103">List pages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97131-104">从指定分区中检索[page](../resources/onenotepage.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="97131-104">Retrieve a list of [page](../resources/onenotepage.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="97131-105">权限</span><span class="sxs-lookup"><span data-stu-id="97131-105">Permissions</span></span>
<span data-ttu-id="97131-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97131-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="97131-108">Permission type</span></span>      | <span data-ttu-id="97131-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97131-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97131-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97131-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97131-111">请参阅 "注意,"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="97131-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="97131-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97131-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97131-113">注意: Read、notes。读写</span><span class="sxs-lookup"><span data-stu-id="97131-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="97131-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="97131-114">Application</span></span> | <span data-ttu-id="97131-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97131-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97131-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97131-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97131-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97131-117">Optional query parameters</span></span>
<span data-ttu-id="97131-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97131-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="97131-119">页面的默认查询返回订购的前20个页面`lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="97131-119">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="97131-120">如果默认查询返回20个以上`@odata.nextLink`的页面, 则该响应包含可用于对结果集进行分页的。</span><span class="sxs-lookup"><span data-stu-id="97131-120">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="97131-121">`top`请求返回的最大页面数为100。</span><span class="sxs-lookup"><span data-stu-id="97131-121">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="97131-122">默认响应将展开`parentSection`并选择节的`id`、 `name`和`self`属性。</span><span class="sxs-lookup"><span data-stu-id="97131-122">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="97131-123">页面`expand`的`parentNotebook`有效值为和`parentSection`。</span><span class="sxs-lookup"><span data-stu-id="97131-123">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97131-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="97131-124">Request headers</span></span>
| <span data-ttu-id="97131-125">名称</span><span class="sxs-lookup"><span data-stu-id="97131-125">Name</span></span>       | <span data-ttu-id="97131-126">类型</span><span class="sxs-lookup"><span data-stu-id="97131-126">Type</span></span> | <span data-ttu-id="97131-127">说明</span><span class="sxs-lookup"><span data-stu-id="97131-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97131-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="97131-128">Authorization</span></span>  | <span data-ttu-id="97131-129">string</span><span class="sxs-lookup"><span data-stu-id="97131-129">string</span></span>  | <span data-ttu-id="97131-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97131-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97131-132">接受</span><span class="sxs-lookup"><span data-stu-id="97131-132">Accept</span></span> | <span data-ttu-id="97131-133">string</span><span class="sxs-lookup"><span data-stu-id="97131-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="97131-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="97131-134">Request body</span></span>
<span data-ttu-id="97131-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97131-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97131-136">响应</span><span class="sxs-lookup"><span data-stu-id="97131-136">Response</span></span>

<span data-ttu-id="97131-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenotePage](../resources/onenotepage.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="97131-137">If successful, this method returns a `200 OK` response code and a collection of [onenotePage](../resources/onenotepage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97131-138">示例</span><span class="sxs-lookup"><span data-stu-id="97131-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97131-139">请求</span><span class="sxs-lookup"><span data-stu-id="97131-139">Request</span></span>
<span data-ttu-id="97131-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97131-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="97131-141">响应</span><span class="sxs-lookup"><span data-stu-id="97131-141">Response</span></span>
<span data-ttu-id="97131-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97131-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
<!--
{
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
