---
title: 创建聊天
description: 创建新的聊天对象。
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1fc781b35a144057c2d6f3baae3c718b86a30e0
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896492"
---
# <a name="create-chat"></a><span data-ttu-id="c3de9-103">创建聊天</span><span class="sxs-lookup"><span data-stu-id="c3de9-103">Create chat</span></span>
<span data-ttu-id="c3de9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3de9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3de9-105">创建新的 [聊天](../resources/chat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3de9-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3de9-106">权限</span><span class="sxs-lookup"><span data-stu-id="c3de9-106">Permissions</span></span>
<span data-ttu-id="c3de9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3de9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3de9-109">Permission type</span></span>|<span data-ttu-id="c3de9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3de9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3de9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3de9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3de9-112">Chat.Create、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3de9-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="c3de9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3de9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3de9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3de9-114">Not supported.</span></span> |
|<span data-ttu-id="c3de9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3de9-115">Application</span></span> | <span data-ttu-id="c3de9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3de9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3de9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3de9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="c3de9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3de9-118">Request headers</span></span>
|<span data-ttu-id="c3de9-119">名称</span><span class="sxs-lookup"><span data-stu-id="c3de9-119">Name</span></span>|<span data-ttu-id="c3de9-120">说明</span><span class="sxs-lookup"><span data-stu-id="c3de9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3de9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3de9-121">Authorization</span></span>|<span data-ttu-id="c3de9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3de9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3de9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3de9-124">Content-Type</span></span>|<span data-ttu-id="c3de9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c3de9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3de9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3de9-127">Request body</span></span>
<span data-ttu-id="c3de9-128">在请求正文中，提供 chat 对象的 JSON [表示](../resources/chat.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="c3de9-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="c3de9-129">下表列出了创建聊天对象所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3de9-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="c3de9-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3de9-130">Property</span></span>|<span data-ttu-id="c3de9-131">类型</span><span class="sxs-lookup"><span data-stu-id="c3de9-131">Type</span></span>|<span data-ttu-id="c3de9-132">说明</span><span class="sxs-lookup"><span data-stu-id="c3de9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3de9-133">topic</span><span class="sxs-lookup"><span data-stu-id="c3de9-133">topic</span></span>|<span data-ttu-id="c3de9-134"> (可选) 字符串</span><span class="sxs-lookup"><span data-stu-id="c3de9-134">(Optional) String</span></span>|<span data-ttu-id="c3de9-135">聊天的标题。</span><span class="sxs-lookup"><span data-stu-id="c3de9-135">The title of the chat.</span></span> <span data-ttu-id="c3de9-136">只有在聊天类型为时，才能提供聊天 `group` 标题。</span><span class="sxs-lookup"><span data-stu-id="c3de9-136">The chat title can be provided only if the chat is of `group` type.</span></span>|
|<span data-ttu-id="c3de9-137">chatType</span><span class="sxs-lookup"><span data-stu-id="c3de9-137">chatType</span></span>|[<span data-ttu-id="c3de9-138">chatType</span><span class="sxs-lookup"><span data-stu-id="c3de9-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="c3de9-139">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="c3de9-139">Specifies the type of chat.</span></span> <span data-ttu-id="c3de9-140">可能的值是： `group` 和 `oneOnOne` 。</span><span class="sxs-lookup"><span data-stu-id="c3de9-140">Possible values are: `group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="c3de9-141">members</span><span class="sxs-lookup"><span data-stu-id="c3de9-141">members</span></span>|<span data-ttu-id="c3de9-142">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3de9-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="c3de9-143">应该添加的对话成员列表。</span><span class="sxs-lookup"><span data-stu-id="c3de9-143">List of conversation members that should be added.</span></span> <span data-ttu-id="c3de9-144">必须在此列表中指定将参与聊天的每一个用户（包括发起创建请求的用户）。</span><span class="sxs-lookup"><span data-stu-id="c3de9-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|

## <a name="response"></a><span data-ttu-id="c3de9-145">响应</span><span class="sxs-lookup"><span data-stu-id="c3de9-145">Response</span></span>

<span data-ttu-id="c3de9-146">如果成功，此方法在响应正文中返回 201 Created 响应代码和新建的聊天资源。</span><span class="sxs-lookup"><span data-stu-id="c3de9-146">If successful, this method returns a 201 Created response code and the newly created **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3de9-147">示例</span><span class="sxs-lookup"><span data-stu-id="c3de9-147">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="c3de9-148">示例 1：创建一对一聊天</span><span class="sxs-lookup"><span data-stu-id="c3de9-148">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="c3de9-149">请求</span><span class="sxs-lookup"><span data-stu-id="c3de9-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c3de9-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3de9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "oneOnOne",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c3de9-151">C#</span><span class="sxs-lookup"><span data-stu-id="c3de9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chat-oneonone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3de9-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3de9-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chat-oneonone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3de9-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3de9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chat-oneonone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3de9-154">Java</span><span class="sxs-lookup"><span data-stu-id="c3de9-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chat-oneonone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a><span data-ttu-id="c3de9-155">响应</span><span class="sxs-lookup"><span data-stu-id="c3de9-155">Response</span></span>
><span data-ttu-id="c3de9-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c3de9-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2020-12-04T23:10:28.51Z",
    "lastUpdatedDateTime": "2020-12-04T23:10:28.51Z",
    "chatType": "oneOnOne",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="c3de9-157">示例 2：创建群聊</span><span class="sxs-lookup"><span data-stu-id="c3de9-157">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="c3de9-158">请求</span><span class="sxs-lookup"><span data-stu-id="c3de9-158">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c3de9-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3de9-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chat_group"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "group",
  "topic": "Group chat title",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c3de9-160">C#</span><span class="sxs-lookup"><span data-stu-id="c3de9-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chat-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3de9-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3de9-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chat-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3de9-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3de9-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chat-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3de9-163">Java</span><span class="sxs-lookup"><span data-stu-id="c3de9-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chat-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a><span data-ttu-id="c3de9-164">响应</span><span class="sxs-lookup"><span data-stu-id="c3de9-164">Response</span></span>
><span data-ttu-id="c3de9-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c3de9-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:11:16.175Z",
    "chatType": "group",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A1c5b01696d2e4a179c292bc9cf04e63b@thread.v2/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

