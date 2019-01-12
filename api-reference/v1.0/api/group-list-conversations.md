---
title: 列出对话
description: 检索此组中的会话列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3baae994c3cebdbb7cd1e8049c8c0d1aeefefc8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967324"
---
# <a name="list-conversations"></a><span data-ttu-id="5de1e-103">列出对话</span><span class="sxs-lookup"><span data-stu-id="5de1e-103">List conversations</span></span>
<span data-ttu-id="5de1e-104">检索此组中的[对话](../resources/conversation.md)列表。</span><span class="sxs-lookup"><span data-stu-id="5de1e-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5de1e-105">权限</span><span class="sxs-lookup"><span data-stu-id="5de1e-105">Permissions</span></span>
<span data-ttu-id="5de1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5de1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5de1e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5de1e-108">Permission type</span></span>      | <span data-ttu-id="5de1e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5de1e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5de1e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5de1e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5de1e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de1e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5de1e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5de1e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de1e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5de1e-113">Not supported.</span></span>    |
|<span data-ttu-id="5de1e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5de1e-114">Application</span></span> | <span data-ttu-id="5de1e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5de1e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de1e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5de1e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5de1e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5de1e-117">Optional query parameters</span></span>
<span data-ttu-id="5de1e-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5de1e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5de1e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5de1e-119">Request headers</span></span>
| <span data-ttu-id="5de1e-120">标头</span><span class="sxs-lookup"><span data-stu-id="5de1e-120">Header</span></span>       | <span data-ttu-id="5de1e-121">值</span><span class="sxs-lookup"><span data-stu-id="5de1e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5de1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5de1e-122">Authorization</span></span>  | <span data-ttu-id="5de1e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5de1e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5de1e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5de1e-125">Request body</span></span>
<span data-ttu-id="5de1e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5de1e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5de1e-127">响应</span><span class="sxs-lookup"><span data-stu-id="5de1e-127">Response</span></span>
<span data-ttu-id="5de1e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5de1e-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5de1e-129">示例</span><span class="sxs-lookup"><span data-stu-id="5de1e-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5de1e-130">请求</span><span class="sxs-lookup"><span data-stu-id="5de1e-130">Request</span></span>
<span data-ttu-id="5de1e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5de1e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="5de1e-132">响应</span><span class="sxs-lookup"><span data-stu-id="5de1e-132">Response</span></span>
<span data-ttu-id="5de1e-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5de1e-133">The following is an example of the response.</span></span>
><span data-ttu-id="5de1e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5de1e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "lastDeliveredDateTime": "datetime-value",
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
