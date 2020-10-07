---
title: 获取对话
description: 检索 conversation 对象的属性和关系。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: db4df5144178e78873d080eb9e1f153bee326468
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371612"
---
# <a name="get-conversation"></a><span data-ttu-id="22323-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="22323-103">Get conversation</span></span>

<span data-ttu-id="22323-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22323-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22323-105">检索 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22323-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="22323-106">权限</span><span class="sxs-lookup"><span data-stu-id="22323-106">Permissions</span></span>
<span data-ttu-id="22323-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22323-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22323-109">Permission type</span></span>      | <span data-ttu-id="22323-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22323-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22323-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22323-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22323-112">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="22323-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="22323-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22323-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22323-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22323-114">Not supported.</span></span>    |
|<span data-ttu-id="22323-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="22323-115">Application</span></span> | <span data-ttu-id="22323-116">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="22323-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22323-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22323-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="22323-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22323-118">Optional query parameters</span></span>
<span data-ttu-id="22323-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22323-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="22323-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22323-120">Request headers</span></span>
| <span data-ttu-id="22323-121">标头</span><span class="sxs-lookup"><span data-stu-id="22323-121">Header</span></span>       | <span data-ttu-id="22323-122">值</span><span class="sxs-lookup"><span data-stu-id="22323-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22323-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22323-123">Authorization</span></span>  | <span data-ttu-id="22323-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22323-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22323-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="22323-126">Request body</span></span>
<span data-ttu-id="22323-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22323-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22323-128">响应</span><span class="sxs-lookup"><span data-stu-id="22323-128">Response</span></span>

<span data-ttu-id="22323-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22323-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22323-130">示例</span><span class="sxs-lookup"><span data-stu-id="22323-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22323-131">请求</span><span class="sxs-lookup"><span data-stu-id="22323-131">Request</span></span>
<span data-ttu-id="22323-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22323-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22323-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22323-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="22323-134">C#</span><span class="sxs-lookup"><span data-stu-id="22323-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22323-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22323-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22323-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22323-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="22323-137">响应</span><span class="sxs-lookup"><span data-stu-id="22323-137">Response</span></span>
<span data-ttu-id="22323-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22323-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
