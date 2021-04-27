---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 86ea62f245e36bee9a3499946f7a3eb80249d368
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049147"
---
# <a name="list-attachments"></a><span data-ttu-id="63bfc-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="63bfc-103">List attachments</span></span>

<span data-ttu-id="63bfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63bfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63bfc-105">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="63bfc-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="63bfc-106">权限</span><span class="sxs-lookup"><span data-stu-id="63bfc-106">Permissions</span></span>
<span data-ttu-id="63bfc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63bfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63bfc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63bfc-109">Permission type</span></span>      | <span data-ttu-id="63bfc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63bfc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63bfc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63bfc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63bfc-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bfc-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63bfc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63bfc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63bfc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63bfc-114">Not supported.</span></span>    |
|<span data-ttu-id="63bfc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="63bfc-115">Application</span></span> | <span data-ttu-id="63bfc-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bfc-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63bfc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63bfc-117">HTTP request</span></span>
<span data-ttu-id="63bfc-118">获取对话 [中帖子](../resources/post.md) 的附件 [组](../resources/conversationthread.md) 线程。</span><span class="sxs-lookup"><span data-stu-id="63bfc-118">Get the attachments for a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="63bfc-119">指定父 [对话是可选的](../resources/conversation.md) 。</span><span class="sxs-lookup"><span data-stu-id="63bfc-119">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63bfc-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63bfc-120">Optional query parameters</span></span>
<span data-ttu-id="63bfc-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63bfc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="63bfc-122">具体而言，您可以使用 $expand 查询参数，以将所有内联帖子附件与发布属性的其余部分一起包含。</span><span class="sxs-lookup"><span data-stu-id="63bfc-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="63bfc-123">例如：</span><span class="sxs-lookup"><span data-stu-id="63bfc-123">For example:</span></span>

<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="63bfc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="63bfc-124">Request headers</span></span>
| <span data-ttu-id="63bfc-125">标头</span><span class="sxs-lookup"><span data-stu-id="63bfc-125">Header</span></span>       | <span data-ttu-id="63bfc-126">值</span><span class="sxs-lookup"><span data-stu-id="63bfc-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63bfc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="63bfc-127">Authorization</span></span>  | <span data-ttu-id="63bfc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63bfc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63bfc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="63bfc-130">Request body</span></span>
<span data-ttu-id="63bfc-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63bfc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63bfc-132">响应</span><span class="sxs-lookup"><span data-stu-id="63bfc-132">Response</span></span>

<span data-ttu-id="63bfc-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="63bfc-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63bfc-134">示例</span><span class="sxs-lookup"><span data-stu-id="63bfc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63bfc-135">请求</span><span class="sxs-lookup"><span data-stu-id="63bfc-135">Request</span></span>
<span data-ttu-id="63bfc-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63bfc-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63bfc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="63bfc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_beta",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJfolA==","AAMkADJ-aHAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments
```
# <a name="c"></a>[<span data-ttu-id="63bfc-138">C#</span><span class="sxs-lookup"><span data-stu-id="63bfc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63bfc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63bfc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63bfc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63bfc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63bfc-141">Java</span><span class="sxs-lookup"><span data-stu-id="63bfc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63bfc-142">响应</span><span class="sxs-lookup"><span data-stu-id="63bfc-142">Response</span></span>
<span data-ttu-id="63bfc-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63bfc-143">Here is an example of the response.</span></span> <span data-ttu-id="63bfc-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63bfc-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "post_get_attachments_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('1848753d-185d-4c08-a4e4-6ee40521d115')/threads('AAQkADJfolA%3D%3D')/posts('AAMkADJ-aHAAA%3D')/attachments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.fileAttachment",
            "id": "AAMkADJ-aHAAABEgAQAO5ZYuLGBmNFnelXXQqAN6I=",
            "lastModifiedDateTime": "2019-08-23T01:53:41Z",
            "name": "FileAsAttachment.txt",
            "contentType": "text/plain",
            "size": 244,
            "isInline": false,
            "contentId": null,
            "contentLocation": null,
            "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
