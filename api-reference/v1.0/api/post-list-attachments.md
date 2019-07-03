---
title: 列出附件
description: 检索附加到帖子的 attachment 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 07132554471016b5776a258d0ee6555b3d782d66
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454396"
---
# <a name="list-attachments"></a><span data-ttu-id="d568c-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="d568c-103">List attachments</span></span>

<span data-ttu-id="d568c-104">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d568c-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="d568c-105">权限</span><span class="sxs-lookup"><span data-stu-id="d568c-105">Permissions</span></span>
<span data-ttu-id="d568c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d568c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d568c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d568c-108">Permission type</span></span>      | <span data-ttu-id="d568c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d568c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d568c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d568c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d568c-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d568c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d568c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d568c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d568c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d568c-113">Not supported.</span></span>    |
|<span data-ttu-id="d568c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d568c-114">Application</span></span> | <span data-ttu-id="d568c-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d568c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d568c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d568c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d568c-117">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d568c-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d568c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d568c-118">Optional query parameters</span></span>
<span data-ttu-id="d568c-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d568c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d568c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d568c-120">Request headers</span></span>
| <span data-ttu-id="d568c-121">标头</span><span class="sxs-lookup"><span data-stu-id="d568c-121">Header</span></span>       | <span data-ttu-id="d568c-122">值</span><span class="sxs-lookup"><span data-stu-id="d568c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d568c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d568c-123">Authorization</span></span>  | <span data-ttu-id="d568c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d568c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d568c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d568c-126">Request body</span></span>
<span data-ttu-id="d568c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d568c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d568c-128">响应</span><span class="sxs-lookup"><span data-stu-id="d568c-128">Response</span></span>

<span data-ttu-id="d568c-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d568c-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d568c-130">示例</span><span class="sxs-lookup"><span data-stu-id="d568c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d568c-131">请求</span><span class="sxs-lookup"><span data-stu-id="d568c-131">Request</span></span>
<span data-ttu-id="d568c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d568c-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d568c-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d568c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d568c-134">C#</span><span class="sxs-lookup"><span data-stu-id="d568c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d568c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d568c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d568c-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="d568c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d568c-137">响应</span><span class="sxs-lookup"><span data-stu-id="d568c-137">Response</span></span>
<span data-ttu-id="d568c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d568c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
