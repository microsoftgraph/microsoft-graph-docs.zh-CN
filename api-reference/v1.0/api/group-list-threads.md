---
title: 列出线程
description: 获取某个组的所有线程。
author: dkershaw10
ms.openlocfilehash: 8052ec02a2f9bfbcec0a12681463f3e33cb0f12d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311799"
---
# <a name="list-threads"></a><span data-ttu-id="1c0b8-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="1c0b8-103">List threads</span></span>
<span data-ttu-id="1c0b8-104">获取某个组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-104">Get all the threads of a group.</span></span>

><span data-ttu-id="1c0b8-105">注意：还可以 [获取会话的所有线程](conversation-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c0b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="1c0b8-106">Permissions</span></span>
<span data-ttu-id="1c0b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c0b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c0b8-109">Permission type</span></span>      | <span data-ttu-id="1c0b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c0b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c0b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c0b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c0b8-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c0b8-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c0b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c0b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c0b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-114">Not supported.</span></span>    |
|<span data-ttu-id="1c0b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c0b8-115">Application</span></span> | <span data-ttu-id="1c0b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c0b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c0b8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c0b8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1c0b8-118">Optional query parameters</span></span>
<span data-ttu-id="1c0b8-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c0b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c0b8-120">Request headers</span></span>
| <span data-ttu-id="1c0b8-121">标头</span><span class="sxs-lookup"><span data-stu-id="1c0b8-121">Header</span></span>       | <span data-ttu-id="1c0b8-122">值</span><span class="sxs-lookup"><span data-stu-id="1c0b8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c0b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c0b8-123">Authorization</span></span>  | <span data-ttu-id="1c0b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c0b8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c0b8-126">Request body</span></span>
<span data-ttu-id="1c0b8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c0b8-128">响应</span><span class="sxs-lookup"><span data-stu-id="1c0b8-128">Response</span></span>
<span data-ttu-id="1c0b8-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c0b8-130">示例</span><span class="sxs-lookup"><span data-stu-id="1c0b8-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1c0b8-131">请求</span><span class="sxs-lookup"><span data-stu-id="1c0b8-131">Request</span></span>
<span data-ttu-id="1c0b8-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="1c0b8-133">响应</span><span class="sxs-lookup"><span data-stu-id="1c0b8-133">Response</span></span>
<span data-ttu-id="1c0b8-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-134">The following is an example of the response.</span></span>
><span data-ttu-id="1c0b8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c0b8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
