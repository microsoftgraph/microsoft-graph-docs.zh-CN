---
title: 获取对话
description: 检索 conversation 对象的属性和关系。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 45e8b4e8a3d4397a62d1161a145608447f38d5cf
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591244"
---
# <a name="get-conversation"></a><span data-ttu-id="9137c-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="9137c-103">Get conversation</span></span>

<span data-ttu-id="9137c-104">检索 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9137c-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9137c-105">权限</span><span class="sxs-lookup"><span data-stu-id="9137c-105">Permissions</span></span>
<span data-ttu-id="9137c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9137c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9137c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9137c-108">Permission type</span></span>      | <span data-ttu-id="9137c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9137c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9137c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9137c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9137c-111">Group。全部, Group。 Read。 All</span><span class="sxs-lookup"><span data-stu-id="9137c-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="9137c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9137c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9137c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9137c-113">Not supported.</span></span>    |
|<span data-ttu-id="9137c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9137c-114">Application</span></span> | <span data-ttu-id="9137c-115">Group。全部, Group。 Read。 All</span><span class="sxs-lookup"><span data-stu-id="9137c-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9137c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9137c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="9137c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9137c-117">Optional query parameters</span></span>
<span data-ttu-id="9137c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9137c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9137c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9137c-119">Request headers</span></span>
| <span data-ttu-id="9137c-120">标头</span><span class="sxs-lookup"><span data-stu-id="9137c-120">Header</span></span>       | <span data-ttu-id="9137c-121">值</span><span class="sxs-lookup"><span data-stu-id="9137c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9137c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9137c-122">Authorization</span></span>  | <span data-ttu-id="9137c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9137c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9137c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9137c-125">Request body</span></span>
<span data-ttu-id="9137c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9137c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9137c-127">响应</span><span class="sxs-lookup"><span data-stu-id="9137c-127">Response</span></span>

<span data-ttu-id="9137c-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9137c-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9137c-129">示例</span><span class="sxs-lookup"><span data-stu-id="9137c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9137c-130">请求</span><span class="sxs-lookup"><span data-stu-id="9137c-130">Request</span></span>
<span data-ttu-id="9137c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9137c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="9137c-132">响应</span><span class="sxs-lookup"><span data-stu-id="9137c-132">Response</span></span>
<span data-ttu-id="9137c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9137c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9137c-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9137c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9137c-137">语言</span><span class="sxs-lookup"><span data-stu-id="9137c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9137c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9137c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
