---
title: 添加 conversationMember
description: 将 conversationMember 添加到频道。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 40ed8afa7700bc2fa1639986c336d15130b03a57
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050753"
---
# <a name="add-conversationmember"></a><span data-ttu-id="0f3db-103">添加 conversationMember</span><span class="sxs-lookup"><span data-stu-id="0f3db-103">Add conversationMember</span></span>

<span data-ttu-id="0f3db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f3db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f3db-105">将[conversationMember](../resources/conversationmember.md)添加到[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="0f3db-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

> [!NOTE]
><span data-ttu-id="0f3db-106">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的通道上受支持 `private` 。</span><span class="sxs-lookup"><span data-stu-id="0f3db-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="0f3db-107">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回400错误请求响应。</span><span class="sxs-lookup"><span data-stu-id="0f3db-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a 400 Bad Request response.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f3db-108">权限</span><span class="sxs-lookup"><span data-stu-id="0f3db-108">Permissions</span></span>

<span data-ttu-id="0f3db-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0f3db-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0f3db-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f3db-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f3db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f3db-111">Permission Type</span></span>|<span data-ttu-id="0f3db-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f3db-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0f3db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f3db-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0f3db-114">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="0f3db-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0f3db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f3db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f3db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f3db-116">Not supported.</span></span>|
|<span data-ttu-id="0f3db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f3db-117">Application</span></span>| <span data-ttu-id="0f3db-118">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="0f3db-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f3db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f3db-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="0f3db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f3db-120">Request headers</span></span>

| <span data-ttu-id="0f3db-121">标头</span><span class="sxs-lookup"><span data-stu-id="0f3db-121">Header</span></span>       | <span data-ttu-id="0f3db-122">值</span><span class="sxs-lookup"><span data-stu-id="0f3db-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f3db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f3db-123">Authorization</span></span>  | <span data-ttu-id="0f3db-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0f3db-124">Bearer {token}.</span></span> <span data-ttu-id="0f3db-125">Required.</span><span class="sxs-lookup"><span data-stu-id="0f3db-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f3db-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f3db-126">Request body</span></span>

<span data-ttu-id="0f3db-127">请求正文中包含以下属性。</span><span class="sxs-lookup"><span data-stu-id="0f3db-127">Include the following properties in the request body.</span></span>

| <span data-ttu-id="0f3db-128">属性</span><span class="sxs-lookup"><span data-stu-id="0f3db-128">Property</span></span>   | <span data-ttu-id="0f3db-129">类型</span><span class="sxs-lookup"><span data-stu-id="0f3db-129">Type</span></span> |<span data-ttu-id="0f3db-130">说明</span><span class="sxs-lookup"><span data-stu-id="0f3db-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f3db-131">角色</span><span class="sxs-lookup"><span data-stu-id="0f3db-131">roles</span></span>|<span data-ttu-id="0f3db-132">string 集合</span><span class="sxs-lookup"><span data-stu-id="0f3db-132">string collection</span></span>|<span data-ttu-id="0f3db-133">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="0f3db-133">The roles for that user.</span></span>|
|<span data-ttu-id="0f3db-134">用户</span><span class="sxs-lookup"><span data-stu-id="0f3db-134">user</span></span>|[<span data-ttu-id="0f3db-135">用户</span><span class="sxs-lookup"><span data-stu-id="0f3db-135">user</span></span>](../resources/user.md)|<span data-ttu-id="0f3db-136">要添加到频道的用户。</span><span class="sxs-lookup"><span data-stu-id="0f3db-136">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="0f3db-137">响应</span><span class="sxs-lookup"><span data-stu-id="0f3db-137">Response</span></span>

<span data-ttu-id="0f3db-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f3db-138">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f3db-139">示例</span><span class="sxs-lookup"><span data-stu-id="0f3db-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f3db-140">请求</span><span class="sxs-lookup"><span data-stu-id="0f3db-140">Request</span></span>

<span data-ttu-id="0f3db-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f3db-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f3db-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f3db-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="0f3db-143">C#</span><span class="sxs-lookup"><span data-stu-id="0f3db-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f3db-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f3db-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f3db-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f3db-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f3db-146">响应</span><span class="sxs-lookup"><span data-stu-id="0f3db-146">Response</span></span>

<span data-ttu-id="0f3db-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f3db-147">Here is an example of the response.</span></span>

><span data-ttu-id="0f3db-148">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0f3db-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f3db-149">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0f3db-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
