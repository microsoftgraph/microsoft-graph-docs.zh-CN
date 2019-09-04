---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1a2f0fa080792ac7aad25ccb14c8f03bae11706d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725610"
---
# <a name="list-attachments"></a><span data-ttu-id="b1a1a-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="b1a1a-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1a1a-104">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1a1a-105">权限</span><span class="sxs-lookup"><span data-stu-id="b1a1a-105">Permissions</span></span>
<span data-ttu-id="b1a1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a1a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1a1a-108">Permission type</span></span>      | <span data-ttu-id="b1a1a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1a1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1a1a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1a1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1a1a-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a1a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1a1a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1a1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1a1a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-113">Not supported.</span></span>    |
|<span data-ttu-id="b1a1a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1a1a-114">Application</span></span> | <span data-ttu-id="b1a1a-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a1a-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1a1a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1a1a-116">HTTP request</span></span>
<span data-ttu-id="b1a1a-117">在组的[conversationThread](../resources/conversationthread.md)中获取[帖子](../resources/post.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-117">Get the attachments for a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="b1a1a-118">指定父[对话](../resources/conversation.md)是可选的。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-118">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1a1a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b1a1a-119">Optional query parameters</span></span>
<span data-ttu-id="b1a1a-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b1a1a-121">特别是, 您可以使用 $expand 查询参数将所有发布附件添加到其余的 post 属性中。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-121">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="b1a1a-122">例如：</span><span class="sxs-lookup"><span data-stu-id="b1a1a-122">For example:</span></span>

<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="b1a1a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1a1a-123">Request headers</span></span>
| <span data-ttu-id="b1a1a-124">标头</span><span class="sxs-lookup"><span data-stu-id="b1a1a-124">Header</span></span>       | <span data-ttu-id="b1a1a-125">值</span><span class="sxs-lookup"><span data-stu-id="b1a1a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1a1a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1a1a-126">Authorization</span></span>  | <span data-ttu-id="b1a1a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1a1a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1a1a-129">Request body</span></span>
<span data-ttu-id="b1a1a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1a1a-131">响应</span><span class="sxs-lookup"><span data-stu-id="b1a1a-131">Response</span></span>

<span data-ttu-id="b1a1a-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1a1a-133">示例</span><span class="sxs-lookup"><span data-stu-id="b1a1a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1a1a-134">请求</span><span class="sxs-lookup"><span data-stu-id="b1a1a-134">Request</span></span>
<span data-ttu-id="b1a1a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1a1a-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b1a1a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_beta",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJfolA==","AAMkADJ-aHAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1a1a-137">C#</span><span class="sxs-lookup"><span data-stu-id="b1a1a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1a1a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1a1a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1a1a-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="b1a1a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1a1a-140">响应</span><span class="sxs-lookup"><span data-stu-id="b1a1a-140">Response</span></span>
<span data-ttu-id="b1a1a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1a1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
