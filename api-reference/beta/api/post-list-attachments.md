---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
ms.openlocfilehash: 57fd3c5bde221017900f44baa5ee2506cd85c495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049439"
---
# <a name="list-attachments"></a><span data-ttu-id="c8b8b-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="c8b8b-103">List attachments</span></span>

> <span data-ttu-id="c8b8b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8b8b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8b8b-106">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8b8b-107">权限</span><span class="sxs-lookup"><span data-stu-id="c8b8b-107">Permissions</span></span>
<span data-ttu-id="c8b8b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8b8b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8b8b-110">Permission type</span></span>      | <span data-ttu-id="c8b8b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8b8b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8b8b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8b8b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c8b8b-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8b8b-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c8b8b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8b8b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8b8b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-115">Not supported.</span></span>    |
|<span data-ttu-id="c8b8b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8b8b-116">Application</span></span> | <span data-ttu-id="c8b8b-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8b8b-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8b8b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8b8b-118">HTTP request</span></span>
<span data-ttu-id="c8b8b-119"><!-- { "blockType": "ignored" } -->[发布](../resources/post.md)[线程](../resources/conversationthread.md)属于组的[对话](../resources/conversation.md)中的附件。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-119"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8b8b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c8b8b-120">Optional query parameters</span></span>
<span data-ttu-id="c8b8b-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c8b8b-122">具体而言，您可以使用 $展开查询参数，以包括整个文章附件内嵌与 post 属性的其余部分。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="c8b8b-123">例如：</span><span class="sxs-lookup"><span data-stu-id="c8b8b-123">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="c8b8b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8b8b-124">Request headers</span></span>
| <span data-ttu-id="c8b8b-125">标头</span><span class="sxs-lookup"><span data-stu-id="c8b8b-125">Header</span></span>       | <span data-ttu-id="c8b8b-126">值</span><span class="sxs-lookup"><span data-stu-id="c8b8b-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8b8b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8b8b-127">Authorization</span></span>  | <span data-ttu-id="c8b8b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8b8b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8b8b-130">Request body</span></span>
<span data-ttu-id="c8b8b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8b8b-132">响应</span><span class="sxs-lookup"><span data-stu-id="c8b8b-132">Response</span></span>

<span data-ttu-id="c8b8b-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8b8b-134">示例</span><span class="sxs-lookup"><span data-stu-id="c8b8b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8b8b-135">请求</span><span class="sxs-lookup"><span data-stu-id="c8b8b-135">Request</span></span>
<span data-ttu-id="c8b8b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="c8b8b-137">响应</span><span class="sxs-lookup"><span data-stu-id="c8b8b-137">Response</span></span>
<span data-ttu-id="c8b8b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8b8b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
