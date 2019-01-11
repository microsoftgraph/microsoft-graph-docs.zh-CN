---
title: 获取对话线程
description: 获取 thread 对象。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 72ca77aa21a40ddeba84f6977b160996f94869b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838043"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="80450-103">获取对话线程</span><span class="sxs-lookup"><span data-stu-id="80450-103">Get conversation thread</span></span>
<span data-ttu-id="80450-104">获取 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80450-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80450-105">权限</span><span class="sxs-lookup"><span data-stu-id="80450-105">Permissions</span></span>
<span data-ttu-id="80450-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80450-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="80450-108">Permission type</span></span>      | <span data-ttu-id="80450-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80450-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80450-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80450-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80450-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80450-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="80450-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80450-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80450-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="80450-113">Not supported.</span></span>    |
|<span data-ttu-id="80450-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="80450-114">Application</span></span> | <span data-ttu-id="80450-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80450-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80450-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80450-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80450-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80450-117">Optional query parameters</span></span>
<span data-ttu-id="80450-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80450-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80450-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="80450-119">Request headers</span></span>
| <span data-ttu-id="80450-120">标头</span><span class="sxs-lookup"><span data-stu-id="80450-120">Header</span></span>       | <span data-ttu-id="80450-121">值</span><span class="sxs-lookup"><span data-stu-id="80450-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80450-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80450-122">Authorization</span></span>  | <span data-ttu-id="80450-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80450-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80450-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80450-125">Request body</span></span>
<span data-ttu-id="80450-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80450-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80450-127">响应</span><span class="sxs-lookup"><span data-stu-id="80450-127">Response</span></span>
<span data-ttu-id="80450-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80450-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80450-129">示例</span><span class="sxs-lookup"><span data-stu-id="80450-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="80450-130">请求</span><span class="sxs-lookup"><span data-stu-id="80450-130">Request</span></span>
<span data-ttu-id="80450-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80450-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="80450-132">响应</span><span class="sxs-lookup"><span data-stu-id="80450-132">Response</span></span>
<span data-ttu-id="80450-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80450-133">The following is an example of the response.</span></span>
><span data-ttu-id="80450-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="80450-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
