---
title: 获取 conversationMember
description: 检索聊天成员。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a2c539b7240060a6434f5ece01dc242ae948a5f4
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379272"
---
# <a name="get-conversationmember"></a><span data-ttu-id="62707-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="62707-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62707-104">从[聊天](../resources/chat.md)中检索 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="62707-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62707-105">权限</span><span class="sxs-lookup"><span data-stu-id="62707-105">Permissions</span></span>

<span data-ttu-id="62707-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62707-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="62707-108">Permission Type</span></span>|<span data-ttu-id="62707-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62707-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="62707-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62707-110">Delegated (work or school account)</span></span>|<span data-ttu-id="62707-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62707-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="62707-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62707-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62707-113">不支持</span><span class="sxs-lookup"><span data-stu-id="62707-113">Not supported</span></span>|
|<span data-ttu-id="62707-114">Application</span><span class="sxs-lookup"><span data-stu-id="62707-114">Application</span></span> |<span data-ttu-id="62707-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62707-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62707-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62707-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62707-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="62707-117">Optional query parameters</span></span>

<span data-ttu-id="62707-118">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="62707-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62707-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="62707-119">Request headers</span></span>

| <span data-ttu-id="62707-120">标头</span><span class="sxs-lookup"><span data-stu-id="62707-120">Header</span></span>       | <span data-ttu-id="62707-121">值</span><span class="sxs-lookup"><span data-stu-id="62707-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="62707-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62707-122">Authorization</span></span>  | <span data-ttu-id="62707-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62707-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62707-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="62707-125">Request body</span></span>

<span data-ttu-id="62707-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62707-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62707-127">响应</span><span class="sxs-lookup"><span data-stu-id="62707-127">Response</span></span>

<span data-ttu-id="62707-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62707-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62707-129">示例</span><span class="sxs-lookup"><span data-stu-id="62707-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="62707-130">请求</span><span class="sxs-lookup"><span data-stu-id="62707-130">Request</span></span>

<span data-ttu-id="62707-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62707-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="62707-132">响应</span><span class="sxs-lookup"><span data-stu-id="62707-132">Response</span></span>

<span data-ttu-id="62707-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="62707-133">Here is an example of the response.</span></span> 

><span data-ttu-id="62707-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62707-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "display-name-value"
}
```