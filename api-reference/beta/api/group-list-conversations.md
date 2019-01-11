---
title: 列出对话
description: 检索此组中的会话列表。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4ef148acd4a3d98a0e5d9c3ad75b5ab3cd0d1489
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823840"
---
# <a name="list-conversations"></a><span data-ttu-id="f524c-103">列出对话</span><span class="sxs-lookup"><span data-stu-id="f524c-103">List conversations</span></span>

> <span data-ttu-id="f524c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f524c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f524c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f524c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f524c-106">检索此组中的[对话](../resources/conversation.md)列表。</span><span class="sxs-lookup"><span data-stu-id="f524c-106">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f524c-107">权限</span><span class="sxs-lookup"><span data-stu-id="f524c-107">Permissions</span></span>
<span data-ttu-id="f524c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f524c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f524c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f524c-110">Permission type</span></span>      | <span data-ttu-id="f524c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f524c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f524c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f524c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f524c-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f524c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f524c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f524c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f524c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f524c-115">Not supported.</span></span>    |
|<span data-ttu-id="f524c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f524c-116">Application</span></span> | <span data-ttu-id="f524c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f524c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f524c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f524c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f524c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f524c-119">Optional query parameters</span></span>
<span data-ttu-id="f524c-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f524c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f524c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f524c-121">Request headers</span></span>
| <span data-ttu-id="f524c-122">标头</span><span class="sxs-lookup"><span data-stu-id="f524c-122">Header</span></span>       | <span data-ttu-id="f524c-123">值</span><span class="sxs-lookup"><span data-stu-id="f524c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f524c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f524c-124">Authorization</span></span>  | <span data-ttu-id="f524c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f524c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f524c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f524c-127">Request body</span></span>
<span data-ttu-id="f524c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f524c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f524c-129">响应</span><span class="sxs-lookup"><span data-stu-id="f524c-129">Response</span></span>
<span data-ttu-id="f524c-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f524c-130">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f524c-131">示例</span><span class="sxs-lookup"><span data-stu-id="f524c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f524c-132">请求</span><span class="sxs-lookup"><span data-stu-id="f524c-132">Request</span></span>
<span data-ttu-id="f524c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f524c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="f524c-134">响应</span><span class="sxs-lookup"><span data-stu-id="f524c-134">Response</span></span>
<span data-ttu-id="f524c-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f524c-135">The following is an example of the response.</span></span>
><span data-ttu-id="f524c-136">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f524c-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f524c-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f524c-137">All the properties will be returned from an actual call.</span></span>
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
