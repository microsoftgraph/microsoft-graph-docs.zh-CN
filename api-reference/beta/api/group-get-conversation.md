---
title: 获取对话
description: 获取 conversation 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3031d613a06102bad85346a93c903533bf9fb1a0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720618"
---
# <a name="get-conversation"></a><span data-ttu-id="9decc-103">获取对话</span><span class="sxs-lookup"><span data-stu-id="9decc-103">Get conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9decc-104">获取 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9decc-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9decc-105">权限</span><span class="sxs-lookup"><span data-stu-id="9decc-105">Permissions</span></span>
<span data-ttu-id="9decc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9decc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9decc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9decc-108">Permission type</span></span>      | <span data-ttu-id="9decc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9decc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9decc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9decc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9decc-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9decc-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9decc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9decc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9decc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9decc-113">Not supported.</span></span>    |
|<span data-ttu-id="9decc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9decc-114">Application</span></span> | <span data-ttu-id="9decc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9decc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9decc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9decc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9decc-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9decc-117">Optional query parameters</span></span>
<span data-ttu-id="9decc-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9decc-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9decc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9decc-119">Request headers</span></span>
| <span data-ttu-id="9decc-120">标头</span><span class="sxs-lookup"><span data-stu-id="9decc-120">Header</span></span>       | <span data-ttu-id="9decc-121">值</span><span class="sxs-lookup"><span data-stu-id="9decc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9decc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9decc-122">Authorization</span></span>  | <span data-ttu-id="9decc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9decc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9decc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9decc-125">Request body</span></span>
<span data-ttu-id="9decc-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9decc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9decc-127">响应</span><span class="sxs-lookup"><span data-stu-id="9decc-127">Response</span></span>
<span data-ttu-id="9decc-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9decc-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9decc-129">示例</span><span class="sxs-lookup"><span data-stu-id="9decc-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9decc-130">请求</span><span class="sxs-lookup"><span data-stu-id="9decc-130">Request</span></span>
<span data-ttu-id="9decc-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9decc-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9decc-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9decc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9decc-133">C#</span><span class="sxs-lookup"><span data-stu-id="9decc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9decc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9decc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9decc-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="9decc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9decc-136">响应</span><span class="sxs-lookup"><span data-stu-id="9decc-136">Response</span></span>
<span data-ttu-id="9decc-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9decc-137">The following is an example of the response.</span></span>
><span data-ttu-id="9decc-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9decc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
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
