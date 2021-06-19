---
title: 创建聊天
description: 创建新的聊天对象。
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ea5de5a32754125c5016bee536c8b8d1802a8d1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030815"
---
# <a name="create-chat"></a><span data-ttu-id="6947e-103">创建聊天</span><span class="sxs-lookup"><span data-stu-id="6947e-103">Create chat</span></span>
<span data-ttu-id="6947e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6947e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6947e-105">创建新的 [聊天](../resources/chat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6947e-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6947e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6947e-106">Permissions</span></span>
<span data-ttu-id="6947e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6947e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6947e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6947e-109">Permission type</span></span>|<span data-ttu-id="6947e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6947e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6947e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6947e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6947e-112">Chat.Create、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6947e-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="6947e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6947e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6947e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6947e-114">Not supported.</span></span> |
|<span data-ttu-id="6947e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6947e-115">Application</span></span> | <span data-ttu-id="6947e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6947e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6947e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6947e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="6947e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6947e-118">Request headers</span></span>
|<span data-ttu-id="6947e-119">名称</span><span class="sxs-lookup"><span data-stu-id="6947e-119">Name</span></span>|<span data-ttu-id="6947e-120">说明</span><span class="sxs-lookup"><span data-stu-id="6947e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6947e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6947e-121">Authorization</span></span>|<span data-ttu-id="6947e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6947e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6947e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6947e-124">Content-Type</span></span>|<span data-ttu-id="6947e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6947e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6947e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6947e-127">Request body</span></span>
<span data-ttu-id="6947e-128">在请求正文中，提供 chat 对象的 JSON [表示](../resources/chat.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="6947e-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="6947e-129">下表列出了创建聊天对象所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6947e-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="6947e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6947e-130">Property</span></span>|<span data-ttu-id="6947e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6947e-131">Type</span></span>|<span data-ttu-id="6947e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6947e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6947e-133">topic</span><span class="sxs-lookup"><span data-stu-id="6947e-133">topic</span></span>|<span data-ttu-id="6947e-134"> (可选) 字符串</span><span class="sxs-lookup"><span data-stu-id="6947e-134">(Optional) String</span></span>|<span data-ttu-id="6947e-135">聊天的标题。</span><span class="sxs-lookup"><span data-stu-id="6947e-135">The title of the chat.</span></span> <span data-ttu-id="6947e-136">只有在聊天类型为时，才能提供聊天 `group` 标题。</span><span class="sxs-lookup"><span data-stu-id="6947e-136">The chat title can be provided only if the chat is of `group` type.</span></span>|
|<span data-ttu-id="6947e-137">chatType</span><span class="sxs-lookup"><span data-stu-id="6947e-137">chatType</span></span>|[<span data-ttu-id="6947e-138">chatType</span><span class="sxs-lookup"><span data-stu-id="6947e-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="6947e-139">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="6947e-139">Specifies the type of chat.</span></span> <span data-ttu-id="6947e-140">可能的值是： `group` 和 `oneOnOne` 。</span><span class="sxs-lookup"><span data-stu-id="6947e-140">Possible values are: `group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="6947e-141">members</span><span class="sxs-lookup"><span data-stu-id="6947e-141">members</span></span>|<span data-ttu-id="6947e-142">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6947e-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="6947e-143">应该添加的对话成员列表。</span><span class="sxs-lookup"><span data-stu-id="6947e-143">List of conversation members that should be added.</span></span> <span data-ttu-id="6947e-144">必须在此列表中指定将参与聊天的每一个用户（包括发起创建请求的用户）。</span><span class="sxs-lookup"><span data-stu-id="6947e-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|
|<span data-ttu-id="6947e-145">installedApps</span><span class="sxs-lookup"><span data-stu-id="6947e-145">installedApps</span></span>| <span data-ttu-id="6947e-146">[teamsApp](../resources/teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6947e-146">[teamsApp](../resources/teamsapp.md) collection</span></span>|<span data-ttu-id="6947e-147">聊天中应安装的应用列表。</span><span class="sxs-lookup"><span data-stu-id="6947e-147">List of apps that should be installed in the chat.</span></span>|

> <span data-ttu-id="6947e-148">**注意：** 目前，仅支持一个应用安装。</span><span class="sxs-lookup"><span data-stu-id="6947e-148">**Note:** Currently, only one app installation is supported.</span></span> <span data-ttu-id="6947e-149">如果请求中列出了多个应用安装，则响应将为 `Bad Request` 错误。</span><span class="sxs-lookup"><span data-stu-id="6947e-149">If multiple app installations are listed in the request, the response will be a `Bad Request` error.</span></span>

## <a name="response"></a><span data-ttu-id="6947e-150">响应</span><span class="sxs-lookup"><span data-stu-id="6947e-150">Response</span></span>

### <a name="response-for-creating-a-one-on-one-chat-without-installed-apps"></a><span data-ttu-id="6947e-151">在未安装应用的情况下创建一对一聊天的响应</span><span class="sxs-lookup"><span data-stu-id="6947e-151">Response for creating a one-on-one chat without installed apps</span></span>
<span data-ttu-id="6947e-152">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和[](../resources/chat.md)新建的聊天资源。</span><span class="sxs-lookup"><span data-stu-id="6947e-152">If successful, this method returns a `201 Created` response code and the newly created [chat](../resources/chat.md) resource in the response body.</span></span>

### <a name="response-for-creating-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="6947e-153">使用已安装的应用创建一对一聊天的响应</span><span class="sxs-lookup"><span data-stu-id="6947e-153">Response for creating a one-on-one chat with installed apps</span></span>
<span data-ttu-id="6947e-154">如果成功，此方法返回 响应 `202 Accepted` 代码和位置标头，其中包含 [teamsAsyncOperation 的链接](../resources/teamsasyncoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="6947e-154">If successful, this method returns a `202 Accepted` response code and Location header that contains a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="6947e-155">该链接可用于获取操作状态和详细信息。</span><span class="sxs-lookup"><span data-stu-id="6947e-155">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="6947e-156">有关详细信息，请参阅 [获取聊天操作](teamsasyncoperation-get.md#example-get-operation-on-chat)。</span><span class="sxs-lookup"><span data-stu-id="6947e-156">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="examples"></a><span data-ttu-id="6947e-157">示例</span><span class="sxs-lookup"><span data-stu-id="6947e-157">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="6947e-158">示例 1：创建一对一聊天</span><span class="sxs-lookup"><span data-stu-id="6947e-158">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="6947e-159">请求</span><span class="sxs-lookup"><span data-stu-id="6947e-159">Request</span></span>
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

---

#### <a name="response"></a><span data-ttu-id="6947e-160">响应</span><span class="sxs-lookup"><span data-stu-id="6947e-160">Response</span></span>
><span data-ttu-id="6947e-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6947e-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="6947e-162">示例 2：创建群聊</span><span class="sxs-lookup"><span data-stu-id="6947e-162">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="6947e-163">请求</span><span class="sxs-lookup"><span data-stu-id="6947e-163">Request</span></span>
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

---

#### <a name="response"></a><span data-ttu-id="6947e-164">响应</span><span class="sxs-lookup"><span data-stu-id="6947e-164">Response</span></span>
><span data-ttu-id="6947e-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6947e-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-create-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="6947e-166">示例 3：使用已安装的应用创建一对一聊天</span><span class="sxs-lookup"><span data-stu-id="6947e-166">Example 3: Create a one-on-one chat with installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="6947e-167">请求</span><span class="sxs-lookup"><span data-stu-id="6947e-167">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne_with_installed_apps"
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
  ],
  "installedApps": [
    {
      "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"
    }
  ]
}
```

---

#### <a name="response"></a><span data-ttu-id="6947e-168">响应</span><span class="sxs-lookup"><span data-stu-id="6947e-168">Response</span></span>
><span data-ttu-id="6947e-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6947e-169">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /chats('19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_bfb5bb25-3a8d-487d-9828-7875ced51a30@unq.gbl.spaces')/operations('2432b57b-0abd-43db-aa7b-16eadd115d34-861f06db-0208-4815-b67a-965df0d28b7f-10adc8a6-60db-42e2-9761-e56a7e4c7bc9')
```

<span data-ttu-id="6947e-170">异步操作已启动，响应包含 Location 标头，其中包含指向 [teamsAsyncOperation 的链接](../resources/teamsasyncoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="6947e-170">The async operation is initiated, and the response contains a Location header which includes a link to the to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="6947e-171">该链接可用于获取操作状态和详细信息。</span><span class="sxs-lookup"><span data-stu-id="6947e-171">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="6947e-172">有关详细信息，请参阅 [获取聊天操作](teamsasyncoperation-get.md#example-get-operation-on-chat)。</span><span class="sxs-lookup"><span data-stu-id="6947e-172">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="see-also"></a><span data-ttu-id="6947e-173">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6947e-173">See also</span></span>
- [<span data-ttu-id="6947e-174">获取 teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="6947e-174">Get teamsAsyncOperation</span></span>](teamsasyncoperation-get.md)
