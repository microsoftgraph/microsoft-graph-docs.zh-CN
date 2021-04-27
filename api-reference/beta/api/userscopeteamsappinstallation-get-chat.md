---
title: 获取用户和 teamsApp 之间的聊天
description: 检索指定用户与应用之间的一对一Teams聊天。
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cde0931caf5509c9782e7da9fdb4691eafa4eb67
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052577"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="db89a-103">获取用户和 teamsApp 之间的聊天</span><span class="sxs-lookup"><span data-stu-id="db89a-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="db89a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db89a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db89a-105">检索[指定用户的](../resources/chat.md)聊天[和Teams](../resources/user.md)[应用](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="db89a-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db89a-106">权限</span><span class="sxs-lookup"><span data-stu-id="db89a-106">Permissions</span></span>

<span data-ttu-id="db89a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db89a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db89a-109">Permission type</span></span>      | <span data-ttu-id="db89a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db89a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db89a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db89a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db89a-112">TeamsAppInstallation.ReadForUser、TeamsAppInstallation.ReadWriteSelfForUser、TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="db89a-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="db89a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db89a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db89a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db89a-114">Not supported.</span></span>    |
|<span data-ttu-id="db89a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db89a-115">Application</span></span> | <span data-ttu-id="db89a-116">TeamsAppInstallation.ReadForUser.All、TeamsAppInstallation.ReadWriteSelfForUser.All、TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="db89a-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db89a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db89a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db89a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db89a-118">Optional query parameters</span></span>

<span data-ttu-id="db89a-119">此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db89a-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db89a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db89a-120">Request headers</span></span>

| <span data-ttu-id="db89a-121">标头</span><span class="sxs-lookup"><span data-stu-id="db89a-121">Header</span></span>       | <span data-ttu-id="db89a-122">值</span><span class="sxs-lookup"><span data-stu-id="db89a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db89a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db89a-123">Authorization</span></span>  | <span data-ttu-id="db89a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db89a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db89a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db89a-126">Request body</span></span>

<span data-ttu-id="db89a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db89a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db89a-128">响应</span><span class="sxs-lookup"><span data-stu-id="db89a-128">Response</span></span>

<span data-ttu-id="db89a-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [chat](../resources/chat.md) 对象的实例。</span><span class="sxs-lookup"><span data-stu-id="db89a-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db89a-130">示例</span><span class="sxs-lookup"><span data-stu-id="db89a-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="db89a-131">示例 1：列出指定用户与应用之间的一对一Teams聊天</span><span class="sxs-lookup"><span data-stu-id="db89a-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="db89a-132">请求</span><span class="sxs-lookup"><span data-stu-id="db89a-132">Request</span></span>

<span data-ttu-id="db89a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db89a-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db89a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db89a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```
# <a name="c"></a>[<span data-ttu-id="db89a-135">C#</span><span class="sxs-lookup"><span data-stu-id="db89a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-chat-teamsapps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db89a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db89a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-chat-teamsapps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db89a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db89a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-chat-teamsapps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db89a-138">Java</span><span class="sxs-lookup"><span data-stu-id="db89a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-chat-teamsapps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db89a-139">响应</span><span class="sxs-lookup"><span data-stu-id="db89a-139">Response</span></span>

<span data-ttu-id="db89a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db89a-140">The following is an example of the response.</span></span>
><span data-ttu-id="db89a-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db89a-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
