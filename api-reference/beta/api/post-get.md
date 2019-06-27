---
title: 获取帖子
description: '获取指定的线程中帖子的属性和关系。 您可以同时指定父 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: db98d6bdda0450ac98844e7cc3dcb1b9f7f4be3a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268220"
---
# <a name="get-post"></a><span data-ttu-id="fd165-104">获取帖子</span><span class="sxs-lookup"><span data-stu-id="fd165-104">Get post</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd165-p102">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="fd165-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="fd165-107">由于**帖子**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**帖子**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="fd165-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd165-108">权限</span><span class="sxs-lookup"><span data-stu-id="fd165-108">Permissions</span></span>
<span data-ttu-id="fd165-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd165-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd165-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd165-111">Permission type</span></span>      | <span data-ttu-id="fd165-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd165-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd165-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd165-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fd165-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd165-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd165-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd165-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd165-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd165-116">Not supported.</span></span>    |
|<span data-ttu-id="fd165-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd165-117">Application</span></span> | <span data-ttu-id="fd165-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd165-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd165-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd165-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd165-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fd165-120">Optional query parameters</span></span>
<span data-ttu-id="fd165-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fd165-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd165-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd165-122">Request headers</span></span>
| <span data-ttu-id="fd165-123">标头</span><span class="sxs-lookup"><span data-stu-id="fd165-123">Header</span></span>       | <span data-ttu-id="fd165-124">值</span><span class="sxs-lookup"><span data-stu-id="fd165-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd165-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd165-125">Authorization</span></span>  | <span data-ttu-id="fd165-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd165-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd165-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd165-128">Request body</span></span>
<span data-ttu-id="fd165-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fd165-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd165-130">响应</span><span class="sxs-lookup"><span data-stu-id="fd165-130">Response</span></span>

<span data-ttu-id="fd165-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd165-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd165-132">示例</span><span class="sxs-lookup"><span data-stu-id="fd165-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd165-133">请求</span><span class="sxs-lookup"><span data-stu-id="fd165-133">Request</span></span>
<span data-ttu-id="fd165-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd165-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="fd165-135">响应</span><span class="sxs-lookup"><span data-stu-id="fd165-135">Response</span></span>
<span data-ttu-id="fd165-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd165-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
    "id":"AQMkADgAAAIJbQAAAA==",
    "createdDateTime":"2018-01-11T17:36:17Z",
    "lastModifiedDateTime":"2018-01-11T17:36:17Z",
    "importance": "normal",
    "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
    "categories":[

    ],
    "receivedDateTime":"2018-01-11T17:36:17Z",
    "hasAttachments":false,
    "body":{
        "contentType":"html",
        "content":"<html><body></body></html>"
    },
    "from":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    },
    "sender":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd165-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fd165-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd165-140">C#</span><span class="sxs-lookup"><span data-stu-id="fd165-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd165-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="fd165-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fd165-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="fd165-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_post-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="fd165-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fd165-143">See also</span></span>

- [<span data-ttu-id="fd165-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fd165-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fd165-145">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fd165-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fd165-146">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fd165-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/post-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
