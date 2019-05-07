---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e6182c864a421330f6168582611bc9adb6d1e7b3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608557"
---
# <a name="list-attachments"></a><span data-ttu-id="b5150-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="b5150-103">List attachments</span></span>

<span data-ttu-id="b5150-104">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="b5150-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5150-105">权限</span><span class="sxs-lookup"><span data-stu-id="b5150-105">Permissions</span></span>
<span data-ttu-id="b5150-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5150-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5150-108">Permission type</span></span>      | <span data-ttu-id="b5150-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5150-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5150-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5150-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5150-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5150-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5150-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5150-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5150-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5150-113">Not supported.</span></span>    |
|<span data-ttu-id="b5150-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5150-114">Application</span></span> | <span data-ttu-id="b5150-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5150-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5150-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5150-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b5150-117">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="b5150-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5150-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5150-118">Optional query parameters</span></span>
<span data-ttu-id="b5150-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5150-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5150-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5150-120">Request headers</span></span>
| <span data-ttu-id="b5150-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5150-121">Header</span></span>       | <span data-ttu-id="b5150-122">值</span><span class="sxs-lookup"><span data-stu-id="b5150-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5150-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5150-123">Authorization</span></span>  | <span data-ttu-id="b5150-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5150-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5150-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5150-126">Request body</span></span>
<span data-ttu-id="b5150-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5150-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5150-128">响应</span><span class="sxs-lookup"><span data-stu-id="b5150-128">Response</span></span>

<span data-ttu-id="b5150-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b5150-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5150-130">示例</span><span class="sxs-lookup"><span data-stu-id="b5150-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5150-131">请求</span><span class="sxs-lookup"><span data-stu-id="b5150-131">Request</span></span>
<span data-ttu-id="b5150-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5150-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="b5150-133">响应</span><span class="sxs-lookup"><span data-stu-id="b5150-133">Response</span></span>
<span data-ttu-id="b5150-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5150-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5150-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b5150-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5150-138">语言</span><span class="sxs-lookup"><span data-stu-id="b5150-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5150-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5150-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
