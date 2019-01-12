---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 690b4ab540982dc9b7febcd1ea302afbcf8429ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916297"
---
# <a name="list-attachments"></a><span data-ttu-id="75a57-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="75a57-103">List attachments</span></span>

> <span data-ttu-id="75a57-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="75a57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75a57-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="75a57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75a57-106">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="75a57-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="75a57-107">权限</span><span class="sxs-lookup"><span data-stu-id="75a57-107">Permissions</span></span>
<span data-ttu-id="75a57-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75a57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a57-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75a57-110">Permission type</span></span>      | <span data-ttu-id="75a57-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75a57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75a57-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75a57-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75a57-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a57-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75a57-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75a57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75a57-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75a57-115">Not supported.</span></span>    |
|<span data-ttu-id="75a57-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="75a57-116">Application</span></span> | <span data-ttu-id="75a57-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a57-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75a57-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75a57-118">HTTP request</span></span>
<span data-ttu-id="75a57-119"><!-- { "blockType": "ignored" } -->[发布](../resources/post.md)[线程](../resources/conversationthread.md)属于组的[对话](../resources/conversation.md)中的附件。</span><span class="sxs-lookup"><span data-stu-id="75a57-119"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="75a57-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75a57-120">Optional query parameters</span></span>
<span data-ttu-id="75a57-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75a57-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="75a57-122">具体而言，您可以使用 $展开查询参数，以包括整个文章附件内嵌与 post 属性的其余部分。</span><span class="sxs-lookup"><span data-stu-id="75a57-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="75a57-123">例如：</span><span class="sxs-lookup"><span data-stu-id="75a57-123">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="75a57-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="75a57-124">Request headers</span></span>
| <span data-ttu-id="75a57-125">标头</span><span class="sxs-lookup"><span data-stu-id="75a57-125">Header</span></span>       | <span data-ttu-id="75a57-126">值</span><span class="sxs-lookup"><span data-stu-id="75a57-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75a57-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="75a57-127">Authorization</span></span>  | <span data-ttu-id="75a57-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75a57-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75a57-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="75a57-130">Request body</span></span>
<span data-ttu-id="75a57-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75a57-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75a57-132">响应</span><span class="sxs-lookup"><span data-stu-id="75a57-132">Response</span></span>

<span data-ttu-id="75a57-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="75a57-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75a57-134">示例</span><span class="sxs-lookup"><span data-stu-id="75a57-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75a57-135">请求</span><span class="sxs-lookup"><span data-stu-id="75a57-135">Request</span></span>
<span data-ttu-id="75a57-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75a57-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="75a57-137">响应</span><span class="sxs-lookup"><span data-stu-id="75a57-137">Response</span></span>
<span data-ttu-id="75a57-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75a57-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
