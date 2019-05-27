---
title: 列出 conversationMembers
description: 检索聊天成员。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 0004b3e08fde52514b300b998b8d576ed496bd01
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379271"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="185e9-103">列出 conversationMembers</span><span class="sxs-lookup"><span data-stu-id="185e9-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="185e9-104">列出[聊天](../resources/chat.md)中的所有[对话成员](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="185e9-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="185e9-105">权限</span><span class="sxs-lookup"><span data-stu-id="185e9-105">Permissions</span></span>

<span data-ttu-id="185e9-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="185e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="185e9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="185e9-108">Permission Type</span></span>|<span data-ttu-id="185e9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="185e9-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="185e9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="185e9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="185e9-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="185e9-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="185e9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="185e9-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="185e9-113">不支持</span><span class="sxs-lookup"><span data-stu-id="185e9-113">Not supported</span></span>|
|<span data-ttu-id="185e9-114">Application</span><span class="sxs-lookup"><span data-stu-id="185e9-114">Application</span></span>| <span data-ttu-id="185e9-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="185e9-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="185e9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="185e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="185e9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="185e9-117">Optional query parameters</span></span>

<span data-ttu-id="185e9-118">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="185e9-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="185e9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="185e9-119">Request headers</span></span>

| <span data-ttu-id="185e9-120">标头</span><span class="sxs-lookup"><span data-stu-id="185e9-120">Header</span></span>       | <span data-ttu-id="185e9-121">值</span><span class="sxs-lookup"><span data-stu-id="185e9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="185e9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="185e9-122">Authorization</span></span>  | <span data-ttu-id="185e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="185e9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="185e9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="185e9-125">Request body</span></span>

<span data-ttu-id="185e9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="185e9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="185e9-127">响应</span><span class="sxs-lookup"><span data-stu-id="185e9-127">Response</span></span>

<span data-ttu-id="185e9-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="185e9-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="185e9-129">示例</span><span class="sxs-lookup"><span data-stu-id="185e9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="185e9-130">请求</span><span class="sxs-lookup"><span data-stu-id="185e9-130">Request</span></span>

<span data-ttu-id="185e9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="185e9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```

##### <a name="response"></a><span data-ttu-id="185e9-132">响应</span><span class="sxs-lookup"><span data-stu-id="185e9-132">Response</span></span>

<span data-ttu-id="185e9-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="185e9-133">Here is an example of the response.</span></span>

><span data-ttu-id="185e9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="185e9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
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