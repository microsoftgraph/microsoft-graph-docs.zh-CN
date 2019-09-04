---
title: 获取对话
description: 检索 conversation 对象的属性和关系。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f56f27e561b5d94748a6f269abe5ad377d9c295c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721402"
---
# <a name="get-conversation"></a><span data-ttu-id="8db32-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="8db32-103">Get conversation</span></span>

<span data-ttu-id="8db32-104">检索 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8db32-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8db32-105">权限</span><span class="sxs-lookup"><span data-stu-id="8db32-105">Permissions</span></span>
<span data-ttu-id="8db32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8db32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8db32-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8db32-108">Permission type</span></span>      | <span data-ttu-id="8db32-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8db32-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8db32-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8db32-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8db32-111">Group. 全部, Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="8db32-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="8db32-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8db32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8db32-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8db32-113">Not supported.</span></span>    |
|<span data-ttu-id="8db32-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8db32-114">Application</span></span> | <span data-ttu-id="8db32-115">Group. 全部, Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="8db32-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8db32-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8db32-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="8db32-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8db32-117">Optional query parameters</span></span>
<span data-ttu-id="8db32-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8db32-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8db32-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8db32-119">Request headers</span></span>
| <span data-ttu-id="8db32-120">标头</span><span class="sxs-lookup"><span data-stu-id="8db32-120">Header</span></span>       | <span data-ttu-id="8db32-121">值</span><span class="sxs-lookup"><span data-stu-id="8db32-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8db32-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8db32-122">Authorization</span></span>  | <span data-ttu-id="8db32-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8db32-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8db32-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8db32-125">Request body</span></span>
<span data-ttu-id="8db32-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8db32-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8db32-127">响应</span><span class="sxs-lookup"><span data-stu-id="8db32-127">Response</span></span>

<span data-ttu-id="8db32-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8db32-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8db32-129">示例</span><span class="sxs-lookup"><span data-stu-id="8db32-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8db32-130">请求</span><span class="sxs-lookup"><span data-stu-id="8db32-130">Request</span></span>
<span data-ttu-id="8db32-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8db32-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8db32-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8db32-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8db32-133">C#</span><span class="sxs-lookup"><span data-stu-id="8db32-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8db32-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8db32-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8db32-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="8db32-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8db32-136">Java</span><span class="sxs-lookup"><span data-stu-id="8db32-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8db32-137">响应</span><span class="sxs-lookup"><span data-stu-id="8db32-137">Response</span></span>
<span data-ttu-id="8db32-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8db32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
