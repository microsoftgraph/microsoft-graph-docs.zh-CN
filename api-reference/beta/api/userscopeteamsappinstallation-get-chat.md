---
title: 在用户和 teamsApp 之间获取聊天
description: 检索指定用户与团队应用程序之间的一对一聊天。
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f4d7d9e6534b13746824a2d7a0e4b19d826acb41
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597282"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="7e45b-103">在用户和 teamsApp 之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="7e45b-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="7e45b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e45b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e45b-105">检索指定[用户](../resources/user.md)和[团队应用程序](../resources/teamsapp.md)的[聊天](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="7e45b-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="7e45b-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e45b-106">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e45b-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7e45b-107">Optional query parameters</span></span>

<span data-ttu-id="7e45b-108">此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7e45b-108">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e45b-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e45b-109">Request headers</span></span>

| <span data-ttu-id="7e45b-110">标头</span><span class="sxs-lookup"><span data-stu-id="7e45b-110">Header</span></span>       | <span data-ttu-id="7e45b-111">值</span><span class="sxs-lookup"><span data-stu-id="7e45b-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e45b-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e45b-112">Authorization</span></span>  | <span data-ttu-id="7e45b-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e45b-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e45b-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e45b-115">Request body</span></span>

<span data-ttu-id="7e45b-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e45b-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e45b-117">响应</span><span class="sxs-lookup"><span data-stu-id="7e45b-117">Response</span></span>

<span data-ttu-id="7e45b-118">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [chat](../resources/chat.md) 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="7e45b-118">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e45b-119">示例</span><span class="sxs-lookup"><span data-stu-id="7e45b-119">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="7e45b-120">示例1：在指定的用户与团队应用程序之间列出一对一聊天</span><span class="sxs-lookup"><span data-stu-id="7e45b-120">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="7e45b-121">请求</span><span class="sxs-lookup"><span data-stu-id="7e45b-121">Request</span></span>

<span data-ttu-id="7e45b-122">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e45b-122">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}/chat
```

#### <a name="response"></a><span data-ttu-id="7e45b-123">响应</span><span class="sxs-lookup"><span data-stu-id="7e45b-123">Response</span></span>

<span data-ttu-id="7e45b-124">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e45b-124">The following is an example of the response.</span></span>
><span data-ttu-id="7e45b-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7e45b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
