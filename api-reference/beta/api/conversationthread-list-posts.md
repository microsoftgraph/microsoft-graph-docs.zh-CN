---
title: 列出帖子
description: '获取指定线程的帖子。 您可以指定父对话和线程，或， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9275540b933a87f266d040e25c37ab22e0371736
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970883"
---
# <a name="list-posts"></a><span data-ttu-id="17b6d-104">列出帖子</span><span class="sxs-lookup"><span data-stu-id="17b6d-104">List posts</span></span>

> <span data-ttu-id="17b6d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="17b6d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17b6d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17b6d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17b6d-p103">获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="17b6d-p103">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="17b6d-109">权限</span><span class="sxs-lookup"><span data-stu-id="17b6d-109">Permissions</span></span>
<span data-ttu-id="17b6d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17b6d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17b6d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="17b6d-112">Permission type</span></span>      | <span data-ttu-id="17b6d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17b6d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17b6d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17b6d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="17b6d-115">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="17b6d-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="17b6d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17b6d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17b6d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="17b6d-117">Not supported.</span></span>    |
|<span data-ttu-id="17b6d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="17b6d-118">Application</span></span> | <span data-ttu-id="17b6d-119">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="17b6d-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17b6d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17b6d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="17b6d-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17b6d-121">Optional query parameters</span></span>
<span data-ttu-id="17b6d-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="17b6d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="17b6d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="17b6d-123">Request headers</span></span>
| <span data-ttu-id="17b6d-124">标头</span><span class="sxs-lookup"><span data-stu-id="17b6d-124">Header</span></span>       | <span data-ttu-id="17b6d-125">值</span><span class="sxs-lookup"><span data-stu-id="17b6d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17b6d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="17b6d-126">Authorization</span></span>  | <span data-ttu-id="17b6d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17b6d-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17b6d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="17b6d-129">Request body</span></span>
<span data-ttu-id="17b6d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17b6d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17b6d-131">响应</span><span class="sxs-lookup"><span data-stu-id="17b6d-131">Response</span></span>

<span data-ttu-id="17b6d-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="17b6d-132">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17b6d-133">示例</span><span class="sxs-lookup"><span data-stu-id="17b6d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17b6d-134">请求</span><span class="sxs-lookup"><span data-stu-id="17b6d-134">Request</span></span>
<span data-ttu-id="17b6d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17b6d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="17b6d-136">响应</span><span class="sxs-lookup"><span data-stu-id="17b6d-136">Response</span></span>
<span data-ttu-id="17b6d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17b6d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
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
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
