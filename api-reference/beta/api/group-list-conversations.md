---
title: 列出对话
description: 检索此组中的会话列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4a548144e7db3cd3bf7732437784fd8fa51a21f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985338"
---
# <a name="list-conversations"></a><span data-ttu-id="89ff4-103">列出对话</span><span class="sxs-lookup"><span data-stu-id="89ff4-103">List conversations</span></span>

> <span data-ttu-id="89ff4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89ff4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89ff4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89ff4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89ff4-106">检索此组中的[对话](../resources/conversation.md)列表。</span><span class="sxs-lookup"><span data-stu-id="89ff4-106">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ff4-107">权限</span><span class="sxs-lookup"><span data-stu-id="89ff4-107">Permissions</span></span>
<span data-ttu-id="89ff4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89ff4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ff4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="89ff4-110">Permission type</span></span>      | <span data-ttu-id="89ff4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89ff4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ff4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89ff4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89ff4-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ff4-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="89ff4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89ff4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89ff4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="89ff4-115">Not supported.</span></span>    |
|<span data-ttu-id="89ff4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="89ff4-116">Application</span></span> | <span data-ttu-id="89ff4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="89ff4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89ff4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89ff4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89ff4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89ff4-119">Optional query parameters</span></span>
<span data-ttu-id="89ff4-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="89ff4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89ff4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="89ff4-121">Request headers</span></span>
| <span data-ttu-id="89ff4-122">标头</span><span class="sxs-lookup"><span data-stu-id="89ff4-122">Header</span></span>       | <span data-ttu-id="89ff4-123">值</span><span class="sxs-lookup"><span data-stu-id="89ff4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89ff4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89ff4-124">Authorization</span></span>  | <span data-ttu-id="89ff4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89ff4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89ff4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89ff4-127">Request body</span></span>
<span data-ttu-id="89ff4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89ff4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89ff4-129">响应</span><span class="sxs-lookup"><span data-stu-id="89ff4-129">Response</span></span>
<span data-ttu-id="89ff4-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="89ff4-130">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ff4-131">示例</span><span class="sxs-lookup"><span data-stu-id="89ff4-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="89ff4-132">请求</span><span class="sxs-lookup"><span data-stu-id="89ff4-132">Request</span></span>
<span data-ttu-id="89ff4-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89ff4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="89ff4-134">响应</span><span class="sxs-lookup"><span data-stu-id="89ff4-134">Response</span></span>
<span data-ttu-id="89ff4-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89ff4-135">The following is an example of the response.</span></span>
><span data-ttu-id="89ff4-136">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89ff4-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89ff4-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89ff4-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
