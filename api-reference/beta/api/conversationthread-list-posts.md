---
title: 列出帖子
description: '获取指定线程的帖子。 您可以指定父对话和线程，或， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6ab9658753baceed8b983eb493957503179f5865
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517244"
---
# <a name="list-posts"></a><span data-ttu-id="daa47-104">列出帖子</span><span class="sxs-lookup"><span data-stu-id="daa47-104">List posts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daa47-p102">获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="daa47-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="daa47-107">权限</span><span class="sxs-lookup"><span data-stu-id="daa47-107">Permissions</span></span>
<span data-ttu-id="daa47-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="daa47-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daa47-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="daa47-110">Permission type</span></span>      | <span data-ttu-id="daa47-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="daa47-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daa47-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="daa47-112">Delegated (work or school account)</span></span> | <span data-ttu-id="daa47-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa47-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="daa47-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="daa47-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daa47-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="daa47-115">Not supported.</span></span>    |
|<span data-ttu-id="daa47-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="daa47-116">Application</span></span> | <span data-ttu-id="daa47-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa47-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="daa47-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="daa47-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="daa47-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="daa47-119">Optional query parameters</span></span>
<span data-ttu-id="daa47-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="daa47-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="daa47-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="daa47-121">Request headers</span></span>
| <span data-ttu-id="daa47-122">标头</span><span class="sxs-lookup"><span data-stu-id="daa47-122">Header</span></span>       | <span data-ttu-id="daa47-123">值</span><span class="sxs-lookup"><span data-stu-id="daa47-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="daa47-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="daa47-124">Authorization</span></span>  | <span data-ttu-id="daa47-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="daa47-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="daa47-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="daa47-127">Request body</span></span>
<span data-ttu-id="daa47-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="daa47-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daa47-129">响应</span><span class="sxs-lookup"><span data-stu-id="daa47-129">Response</span></span>

<span data-ttu-id="daa47-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="daa47-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="daa47-131">示例</span><span class="sxs-lookup"><span data-stu-id="daa47-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="daa47-132">请求</span><span class="sxs-lookup"><span data-stu-id="daa47-132">Request</span></span>
<span data-ttu-id="daa47-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="daa47-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="daa47-134">响应</span><span class="sxs-lookup"><span data-stu-id="daa47-134">Response</span></span>
<span data-ttu-id="daa47-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="daa47-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-list-posts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
