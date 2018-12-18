---
title: 获取对话线程
description: 获取 thread 对象。
author: dkershaw10
ms.openlocfilehash: 615a606bbe0e58da233642c55baccb3f05dc3dd6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347724"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="a6a22-103">获取对话线程</span><span class="sxs-lookup"><span data-stu-id="a6a22-103">Get conversation thread</span></span>

> <span data-ttu-id="a6a22-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a6a22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6a22-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a6a22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6a22-106">获取 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6a22-106">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6a22-107">权限</span><span class="sxs-lookup"><span data-stu-id="a6a22-107">Permissions</span></span>
<span data-ttu-id="a6a22-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a22-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6a22-110">Permission type</span></span>      | <span data-ttu-id="a6a22-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6a22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6a22-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6a22-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6a22-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a22-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6a22-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6a22-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6a22-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6a22-115">Not supported.</span></span>    |
|<span data-ttu-id="a6a22-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6a22-116">Application</span></span> | <span data-ttu-id="a6a22-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6a22-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6a22-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6a22-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6a22-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6a22-119">Optional query parameters</span></span>
<span data-ttu-id="a6a22-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a6a22-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6a22-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6a22-121">Request headers</span></span>
| <span data-ttu-id="a6a22-122">标头</span><span class="sxs-lookup"><span data-stu-id="a6a22-122">Header</span></span>       | <span data-ttu-id="a6a22-123">值</span><span class="sxs-lookup"><span data-stu-id="a6a22-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6a22-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6a22-124">Authorization</span></span>  | <span data-ttu-id="a6a22-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6a22-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6a22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6a22-127">Request body</span></span>
<span data-ttu-id="a6a22-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6a22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6a22-129">响应</span><span class="sxs-lookup"><span data-stu-id="a6a22-129">Response</span></span>
<span data-ttu-id="a6a22-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6a22-130">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a22-131">示例</span><span class="sxs-lookup"><span data-stu-id="a6a22-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a6a22-132">请求</span><span class="sxs-lookup"><span data-stu-id="a6a22-132">Request</span></span>
<span data-ttu-id="a6a22-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6a22-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="a6a22-134">响应</span><span class="sxs-lookup"><span data-stu-id="a6a22-134">Response</span></span>
<span data-ttu-id="a6a22-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a6a22-135">The following is an example of the response.</span></span>
><span data-ttu-id="a6a22-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a6a22-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
