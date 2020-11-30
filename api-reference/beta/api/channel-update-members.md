---
title: 更新通道中的成员
description: 更新通道中成员的角色。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f38ffabd2f10f3226f1af03027e02f8e27b198ec
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387540"
---
# <a name="update-member-in-channel"></a><span data-ttu-id="59e91-103">更新通道中的成员</span><span class="sxs-lookup"><span data-stu-id="59e91-103">Update member in channel</span></span>

<span data-ttu-id="59e91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59e91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e91-105">在[频道](../resources/channel.md)中更新[conversationMember](../resources/conversationmember.md)的角色。</span><span class="sxs-lookup"><span data-stu-id="59e91-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="59e91-106">仅对 **membershipType** 值为的通道使用此操作 `private` 。</span><span class="sxs-lookup"><span data-stu-id="59e91-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="59e91-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="59e91-107">Permissions</span></span>

<span data-ttu-id="59e91-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59e91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59e91-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59e91-110">Permission Type</span></span>|<span data-ttu-id="59e91-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59e91-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="59e91-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59e91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59e91-113">ChannelMember。</span><span class="sxs-lookup"><span data-stu-id="59e91-113">ChannelMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="59e91-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59e91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59e91-115">不支持</span><span class="sxs-lookup"><span data-stu-id="59e91-115">Not supported</span></span>|
|<span data-ttu-id="59e91-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59e91-116">Application</span></span>|<span data-ttu-id="59e91-117">ChannelMember。</span><span class="sxs-lookup"><span data-stu-id="59e91-117">ChannelMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59e91-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59e91-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="59e91-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59e91-119">Request headers</span></span>

| <span data-ttu-id="59e91-120">标头</span><span class="sxs-lookup"><span data-stu-id="59e91-120">Header</span></span>       | <span data-ttu-id="59e91-121">值</span><span class="sxs-lookup"><span data-stu-id="59e91-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59e91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59e91-122">Authorization</span></span>  | <span data-ttu-id="59e91-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59e91-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59e91-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="59e91-125">Content-type</span></span> | <span data-ttu-id="59e91-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="59e91-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59e91-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="59e91-128">Request body</span></span>

<span data-ttu-id="59e91-129">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="59e91-129">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="59e91-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="59e91-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59e91-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="59e91-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59e91-132">属性</span><span class="sxs-lookup"><span data-stu-id="59e91-132">Property</span></span>   | <span data-ttu-id="59e91-133">类型</span><span class="sxs-lookup"><span data-stu-id="59e91-133">Type</span></span> |<span data-ttu-id="59e91-134">说明</span><span class="sxs-lookup"><span data-stu-id="59e91-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59e91-135">角色</span><span class="sxs-lookup"><span data-stu-id="59e91-135">roles</span></span>|<span data-ttu-id="59e91-136">string 集合</span><span class="sxs-lookup"><span data-stu-id="59e91-136">string collection</span></span>|<span data-ttu-id="59e91-137">用户的角色。</span><span class="sxs-lookup"><span data-stu-id="59e91-137">The role for the user.</span></span> <span data-ttu-id="59e91-138">必须为 `owner` 或为空。</span><span class="sxs-lookup"><span data-stu-id="59e91-138">Must be `owner` or empty.</span></span> <span data-ttu-id="59e91-139">来宾用户将自动标记为 `guest` 角色，并且此值不能更新。</span><span class="sxs-lookup"><span data-stu-id="59e91-139">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="59e91-140">响应</span><span class="sxs-lookup"><span data-stu-id="59e91-140">Response</span></span>

<span data-ttu-id="59e91-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59e91-141">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59e91-142">示例</span><span class="sxs-lookup"><span data-stu-id="59e91-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="59e91-143">请求</span><span class="sxs-lookup"><span data-stu-id="59e91-143">Request</span></span>

<span data-ttu-id="59e91-144">以下是将角色应用于 `owner` 频道现有成员的请求。</span><span class="sxs-lookup"><span data-stu-id="59e91-144">The following is a request to apply the `owner` role to an existing member of a channel.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="59e91-145">响应</span><span class="sxs-lookup"><span data-stu-id="59e91-145">Response</span></span>

><span data-ttu-id="59e91-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="59e91-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="59e91-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="59e91-147">See also</span></span>

- [<span data-ttu-id="59e91-148">更新团队中的成员角色</span><span class="sxs-lookup"><span data-stu-id="59e91-148">Update member's role in a team</span></span>](team-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of channel member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
