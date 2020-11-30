---
title: 将成员添加到频道
description: 将成员添加到频道。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 797b970987106cf1720cebcec39739fde488dd22
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387857"
---
# <a name="add-member-to-channel"></a><span data-ttu-id="301db-103">将成员添加到频道</span><span class="sxs-lookup"><span data-stu-id="301db-103">Add member to channel</span></span>

<span data-ttu-id="301db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="301db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="301db-105">将 [conversationMember](../resources/conversationmember.md) 添加到 [频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="301db-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span> <span data-ttu-id="301db-106">仅对 **membershipType** 值为的通道使用此操作 `private` 。</span><span class="sxs-lookup"><span data-stu-id="301db-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="301db-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="301db-107">Permissions</span></span>

<span data-ttu-id="301db-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="301db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="301db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="301db-110">Permission Type</span></span>|<span data-ttu-id="301db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="301db-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="301db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="301db-112">Delegated (work or school account)</span></span>| <span data-ttu-id="301db-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="301db-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="301db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="301db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="301db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="301db-115">Not supported.</span></span>|
|<span data-ttu-id="301db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="301db-116">Application</span></span>| <span data-ttu-id="301db-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="301db-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="301db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="301db-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{team-id}/channels/{channel-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="301db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="301db-119">Request headers</span></span>

| <span data-ttu-id="301db-120">标头</span><span class="sxs-lookup"><span data-stu-id="301db-120">Header</span></span>       | <span data-ttu-id="301db-121">值</span><span class="sxs-lookup"><span data-stu-id="301db-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="301db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="301db-122">Authorization</span></span>  | <span data-ttu-id="301db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="301db-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="301db-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="301db-125">Content-type</span></span> | <span data-ttu-id="301db-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="301db-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="301db-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="301db-128">Request body</span></span>

<span data-ttu-id="301db-129">请求正文中包含以下属性。</span><span class="sxs-lookup"><span data-stu-id="301db-129">Include the following properties in the request body.</span></span>

| <span data-ttu-id="301db-130">属性</span><span class="sxs-lookup"><span data-stu-id="301db-130">Property</span></span>   | <span data-ttu-id="301db-131">类型</span><span class="sxs-lookup"><span data-stu-id="301db-131">Type</span></span> |<span data-ttu-id="301db-132">说明</span><span class="sxs-lookup"><span data-stu-id="301db-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="301db-133">角色</span><span class="sxs-lookup"><span data-stu-id="301db-133">roles</span></span>|<span data-ttu-id="301db-134">string 集合</span><span class="sxs-lookup"><span data-stu-id="301db-134">string collection</span></span>|<span data-ttu-id="301db-135">用户的角色。</span><span class="sxs-lookup"><span data-stu-id="301db-135">The role for the user.</span></span> <span data-ttu-id="301db-136">必须为 `owner` 或为空。</span><span class="sxs-lookup"><span data-stu-id="301db-136">Must be `owner` or empty.</span></span>|
|<span data-ttu-id="301db-137">user</span><span class="sxs-lookup"><span data-stu-id="301db-137">user</span></span>|[<span data-ttu-id="301db-138">用户</span><span class="sxs-lookup"><span data-stu-id="301db-138">user</span></span>](../resources/user.md)|<span data-ttu-id="301db-139">要添加到频道的用户。</span><span class="sxs-lookup"><span data-stu-id="301db-139">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="301db-140">响应</span><span class="sxs-lookup"><span data-stu-id="301db-140">Response</span></span>

<span data-ttu-id="301db-141">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="301db-141">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="301db-142">示例</span><span class="sxs-lookup"><span data-stu-id="301db-142">Examples</span></span>

### <a name="example-1-add-a-member-to-a-channel"></a><span data-ttu-id="301db-143">示例1：向通道中添加成员</span><span class="sxs-lookup"><span data-stu-id="301db-143">Example 1: Add a member to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="301db-144">请求</span><span class="sxs-lookup"><span data-stu-id="301db-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
Content-type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
}
```

#### <a name="response"></a><span data-ttu-id="301db-145">响应</span><span class="sxs-lookup"><span data-stu-id="301db-145">Response</span></span>

><span data-ttu-id="301db-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="301db-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="example-2-add-a-member-with-the-owner-role-to-a-channel"></a><span data-ttu-id="301db-147">示例2：将具有 owner 角色的成员添加到通道</span><span class="sxs-lookup"><span data-stu-id="301db-147">Example 2: Add a member with the owner role to a channel</span></span>

#### <a name="request"></a><span data-ttu-id="301db-148">请求</span><span class="sxs-lookup"><span data-stu-id="301db-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "channel_add_member"
} -->

```http
POST https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members
```

#### <a name="response"></a><span data-ttu-id="301db-149">响应</span><span class="sxs-lookup"><span data-stu-id="301db-149">Response</span></span>

<span data-ttu-id="301db-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="301db-150">Here is an example of the response.</span></span>

><span data-ttu-id="301db-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="301db-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="301db-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="301db-152">See also</span></span>

- [<span data-ttu-id="301db-153">向团队添加成员</span><span class="sxs-lookup"><span data-stu-id="301db-153">Add member to team</span></span>](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add member to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
