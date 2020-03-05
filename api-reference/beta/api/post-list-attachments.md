---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 51be738bc631fad1df61b6fd9e570b0b1a088cd8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455483"
---
# <a name="list-attachments"></a><span data-ttu-id="69b32-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="69b32-103">List attachments</span></span>

<span data-ttu-id="69b32-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="69b32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69b32-105">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="69b32-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="69b32-106">权限</span><span class="sxs-lookup"><span data-stu-id="69b32-106">Permissions</span></span>
<span data-ttu-id="69b32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69b32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69b32-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69b32-109">Permission type</span></span>      | <span data-ttu-id="69b32-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69b32-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69b32-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69b32-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69b32-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b32-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69b32-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69b32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69b32-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="69b32-114">Not supported.</span></span>    |
|<span data-ttu-id="69b32-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="69b32-115">Application</span></span> | <span data-ttu-id="69b32-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b32-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69b32-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69b32-117">HTTP request</span></span>
<span data-ttu-id="69b32-118">在组的[conversationThread](../resources/conversationthread.md)中获取[帖子](../resources/post.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="69b32-118">Get the attachments for a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="69b32-119">指定父[对话](../resources/conversation.md)是可选的。</span><span class="sxs-lookup"><span data-stu-id="69b32-119">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69b32-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69b32-120">Optional query parameters</span></span>
<span data-ttu-id="69b32-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69b32-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="69b32-122">特别是，您可以使用 $expand 查询参数将所有发布附件添加到其余的 post 属性中。</span><span class="sxs-lookup"><span data-stu-id="69b32-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="69b32-123">例如：</span><span class="sxs-lookup"><span data-stu-id="69b32-123">For example:</span></span>

<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="69b32-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="69b32-124">Request headers</span></span>
| <span data-ttu-id="69b32-125">标头</span><span class="sxs-lookup"><span data-stu-id="69b32-125">Header</span></span>       | <span data-ttu-id="69b32-126">值</span><span class="sxs-lookup"><span data-stu-id="69b32-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69b32-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="69b32-127">Authorization</span></span>  | <span data-ttu-id="69b32-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69b32-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69b32-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="69b32-130">Request body</span></span>
<span data-ttu-id="69b32-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69b32-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69b32-132">响应</span><span class="sxs-lookup"><span data-stu-id="69b32-132">Response</span></span>

<span data-ttu-id="69b32-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69b32-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69b32-134">示例</span><span class="sxs-lookup"><span data-stu-id="69b32-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69b32-135">请求</span><span class="sxs-lookup"><span data-stu-id="69b32-135">Request</span></span>
<span data-ttu-id="69b32-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69b32-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69b32-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="69b32-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_beta",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJfolA==","AAMkADJ-aHAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments
```
# <a name="c"></a>[<span data-ttu-id="69b32-138">C#</span><span class="sxs-lookup"><span data-stu-id="69b32-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69b32-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69b32-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69b32-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69b32-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69b32-141">响应</span><span class="sxs-lookup"><span data-stu-id="69b32-141">Response</span></span>
<span data-ttu-id="69b32-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69b32-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
