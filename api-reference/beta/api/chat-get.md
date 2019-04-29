---
title: 获取聊天
description: 检索一个聊天。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: fa0afdb1697d0905c28a70015f260acd7ed4d6f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327542"
---
# <a name="get-chat"></a><span data-ttu-id="71971-103">获取聊天</span><span class="sxs-lookup"><span data-stu-id="71971-103">Get chat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71971-104">检索一个[聊天](../resources/chat.md)（不含其消息）。</span><span class="sxs-lookup"><span data-stu-id="71971-104">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="71971-105">权限</span><span class="sxs-lookup"><span data-stu-id="71971-105">Permissions</span></span>

<span data-ttu-id="71971-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="71971-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="71971-108">Permission type</span></span>      | <span data-ttu-id="71971-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71971-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71971-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71971-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71971-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="71971-111">Chat.Read</span></span>   |
|<span data-ttu-id="71971-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71971-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71971-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="71971-113">Not supported.</span></span>    |
|<span data-ttu-id="71971-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="71971-114">Application</span></span> | <span data-ttu-id="71971-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71971-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="71971-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71971-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71971-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71971-117">Optional query parameters</span></span>

<span data-ttu-id="71971-118">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="71971-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71971-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71971-119">Request headers</span></span>

| <span data-ttu-id="71971-120">标头</span><span class="sxs-lookup"><span data-stu-id="71971-120">Header</span></span>       | <span data-ttu-id="71971-121">值</span><span class="sxs-lookup"><span data-stu-id="71971-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71971-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71971-122">Authorization</span></span>  | <span data-ttu-id="71971-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71971-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71971-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="71971-125">Request body</span></span>

<span data-ttu-id="71971-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71971-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71971-127">响应</span><span class="sxs-lookup"><span data-stu-id="71971-127">Response</span></span>

<span data-ttu-id="71971-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="71971-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71971-129">示例</span><span class="sxs-lookup"><span data-stu-id="71971-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71971-130">请求</span><span class="sxs-lookup"><span data-stu-id="71971-130">Request</span></span>
<span data-ttu-id="71971-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71971-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```

##### <a name="response"></a><span data-ttu-id="71971-132">响应</span><span class="sxs-lookup"><span data-stu-id="71971-132">Response</span></span>
<span data-ttu-id="71971-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71971-133">Here is an example of the response.</span></span> 

><span data-ttu-id="71971-134">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="71971-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="71971-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71971-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
