---
title: 列出 conversationMembers
description: 检索聊天或频道成员的列表。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8efb0b6c6647f48bf64de04a25a564ae0b3a00e8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700877"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="10ccd-103">列出 conversationMembers</span><span class="sxs-lookup"><span data-stu-id="10ccd-103">List conversationMembers</span></span>

<span data-ttu-id="10ccd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ccd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10ccd-105">列出[聊天](../resources/chatmessage.md)或[频道](../resources/channel.md)中的所有[对话成员](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="10ccd-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10ccd-106">权限</span><span class="sxs-lookup"><span data-stu-id="10ccd-106">Permissions</span></span>

<span data-ttu-id="10ccd-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ccd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="10ccd-109">Permission Type</span></span>|<span data-ttu-id="10ccd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10ccd-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="10ccd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10ccd-111">Delegated (work or school account)</span></span>| <span data-ttu-id="10ccd-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10ccd-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="10ccd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10ccd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ccd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ccd-114">Not supported.</span></span>|
|<span data-ttu-id="10ccd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="10ccd-115">Application</span></span>| <span data-ttu-id="10ccd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ccd-116">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="10ccd-117">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="10ccd-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="10ccd-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="10ccd-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="10ccd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10ccd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10ccd-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10ccd-120">Optional query parameters</span></span>

<span data-ttu-id="10ccd-121">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10ccd-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ccd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="10ccd-122">Request headers</span></span>

| <span data-ttu-id="10ccd-123">标头</span><span class="sxs-lookup"><span data-stu-id="10ccd-123">Header</span></span>       | <span data-ttu-id="10ccd-124">值</span><span class="sxs-lookup"><span data-stu-id="10ccd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10ccd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ccd-125">Authorization</span></span>  | <span data-ttu-id="10ccd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10ccd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10ccd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="10ccd-128">Request body</span></span>

<span data-ttu-id="10ccd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10ccd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ccd-130">响应</span><span class="sxs-lookup"><span data-stu-id="10ccd-130">Response</span></span>

<span data-ttu-id="10ccd-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="10ccd-131">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ccd-132">示例</span><span class="sxs-lookup"><span data-stu-id="10ccd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="10ccd-133">请求</span><span class="sxs-lookup"><span data-stu-id="10ccd-133">Request</span></span>

<span data-ttu-id="10ccd-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="10ccd-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/chats/{id}/members
```

### <a name="response"></a><span data-ttu-id="10ccd-135">响应</span><span class="sxs-lookup"><span data-stu-id="10ccd-135">Response</span></span>

<span data-ttu-id="10ccd-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="10ccd-136">The following is an example of the response.</span></span>

><span data-ttu-id="10ccd-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="10ccd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
