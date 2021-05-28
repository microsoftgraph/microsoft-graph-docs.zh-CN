---
title: 获取对话线程
description: 获取 thread 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 27a5f78272936c94e4dcac113949b5eae836382e
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682010"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="df6c5-103">获取对话线程</span><span class="sxs-lookup"><span data-stu-id="df6c5-103">Get conversation thread</span></span>

<span data-ttu-id="df6c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df6c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df6c5-105">获取 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df6c5-105">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df6c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="df6c5-106">Permissions</span></span>
<span data-ttu-id="df6c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df6c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df6c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df6c5-109">Permission type</span></span>      | <span data-ttu-id="df6c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df6c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df6c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df6c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df6c5-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df6c5-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df6c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df6c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df6c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df6c5-114">Not supported.</span></span>    |
|<span data-ttu-id="df6c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df6c5-115">Application</span></span> | <span data-ttu-id="df6c5-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df6c5-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df6c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df6c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df6c5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="df6c5-118">Optional query parameters</span></span>
<span data-ttu-id="df6c5-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="df6c5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df6c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df6c5-120">Request headers</span></span>
| <span data-ttu-id="df6c5-121">标头</span><span class="sxs-lookup"><span data-stu-id="df6c5-121">Header</span></span>       | <span data-ttu-id="df6c5-122">值</span><span class="sxs-lookup"><span data-stu-id="df6c5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df6c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df6c5-123">Authorization</span></span>  | <span data-ttu-id="df6c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df6c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df6c5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="df6c5-126">Request body</span></span>
<span data-ttu-id="df6c5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df6c5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df6c5-128">响应</span><span class="sxs-lookup"><span data-stu-id="df6c5-128">Response</span></span>
<span data-ttu-id="df6c5-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df6c5-129">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df6c5-130">示例</span><span class="sxs-lookup"><span data-stu-id="df6c5-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="df6c5-131">请求</span><span class="sxs-lookup"><span data-stu-id="df6c5-131">Request</span></span>
<span data-ttu-id="df6c5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df6c5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df6c5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df6c5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="df6c5-134">C#</span><span class="sxs-lookup"><span data-stu-id="df6c5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df6c5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df6c5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df6c5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df6c5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df6c5-137">Java</span><span class="sxs-lookup"><span data-stu-id="df6c5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df6c5-138">响应</span><span class="sxs-lookup"><span data-stu-id="df6c5-138">Response</span></span>
<span data-ttu-id="df6c5-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df6c5-139">The following is an example of the response.</span></span>
><span data-ttu-id="df6c5-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="df6c5-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

