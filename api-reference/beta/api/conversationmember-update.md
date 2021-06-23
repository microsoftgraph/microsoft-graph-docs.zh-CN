---
title: 更新 conversationMember
description: 更新团队或频道中 conversationMember 的角色。
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 01f477c74e46876eae38c8d8d622a1a179671a5d
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059901"
---
# <a name="update-conversationmember"></a><span data-ttu-id="f5b7c-103">更新 conversationMember</span><span class="sxs-lookup"><span data-stu-id="f5b7c-103">Update conversationMember</span></span>

<span data-ttu-id="f5b7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5b7c-105">更新团队 [中 conversationMember](../resources/conversationmember.md) [的角色](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>
<span data-ttu-id="f5b7c-106">或 [频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-106">or [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f5b7c-107">在频道上，此操作仅在 [channelMembershipType](../resources/enums.md#channelmembershiptype-values) 为 的频道上受支持 `private` 。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-107">On channels, this operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="f5b7c-108">具有任何其他 [channelMembershipType](../resources/enums.md#channelmembershiptype-values) 的调用将返回 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-108">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5b7c-109">权限</span><span class="sxs-lookup"><span data-stu-id="f5b7c-109">Permissions</span></span>

<span data-ttu-id="f5b7c-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b7c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5b7c-112">Permission Type</span></span>|<span data-ttu-id="f5b7c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5b7c-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="f5b7c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5b7c-114">Delegated (work or school account)</span></span>| <span data-ttu-id="f5b7c-115">在团队中：TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b7c-115">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="f5b7c-116">在频道中：ChannelMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b7c-116">In channels: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f5b7c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5b7c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5b7c-118">不支持</span><span class="sxs-lookup"><span data-stu-id="f5b7c-118">Not supported</span></span>|
|<span data-ttu-id="f5b7c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5b7c-119">Application</span></span>| <span data-ttu-id="f5b7c-120">在团队中：TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b7c-120">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="f5b7c-121">在频道中：ChannelMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b7c-121">In channels:  ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5b7c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5b7c-122">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/members/{id}
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5b7c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5b7c-123">Request headers</span></span>

| <span data-ttu-id="f5b7c-124">标头</span><span class="sxs-lookup"><span data-stu-id="f5b7c-124">Header</span></span>       | <span data-ttu-id="f5b7c-125">值</span><span class="sxs-lookup"><span data-stu-id="f5b7c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5b7c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5b7c-126">Authorization</span></span>  | <span data-ttu-id="f5b7c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5b7c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5b7c-129">Request body</span></span>

<span data-ttu-id="f5b7c-130">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-130">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="f5b7c-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f5b7c-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5b7c-133">属性</span><span class="sxs-lookup"><span data-stu-id="f5b7c-133">Property</span></span>   | <span data-ttu-id="f5b7c-134">类型</span><span class="sxs-lookup"><span data-stu-id="f5b7c-134">Type</span></span> |<span data-ttu-id="f5b7c-135">说明</span><span class="sxs-lookup"><span data-stu-id="f5b7c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5b7c-136">角色</span><span class="sxs-lookup"><span data-stu-id="f5b7c-136">roles</span></span>|<span data-ttu-id="f5b7c-137">string 集合</span><span class="sxs-lookup"><span data-stu-id="f5b7c-137">string collection</span></span>|<span data-ttu-id="f5b7c-138">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-138">The roles for that user.</span></span> <span data-ttu-id="f5b7c-139">必须是"owner"或为空。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-139">Must be "owner" or empty.</span></span> <span data-ttu-id="f5b7c-140">来宾用户必须始终具有角色"来宾"且无法更改。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-140">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="f5b7c-141">响应</span><span class="sxs-lookup"><span data-stu-id="f5b7c-141">Response</span></span>

<span data-ttu-id="f5b7c-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-142">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5b7c-143">示例</span><span class="sxs-lookup"><span data-stu-id="f5b7c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5b7c-144">请求</span><span class="sxs-lookup"><span data-stu-id="f5b7c-144">Request</span></span>

<span data-ttu-id="f5b7c-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5b7c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b7c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="f5b7c-147">C#</span><span class="sxs-lookup"><span data-stu-id="f5b7c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5b7c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5b7c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5b7c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5b7c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5b7c-150">Java</span><span class="sxs-lookup"><span data-stu-id="f5b7c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5b7c-151">响应</span><span class="sxs-lookup"><span data-stu-id="f5b7c-151">Response</span></span>

<span data-ttu-id="f5b7c-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-152">Here is an example of the response.</span></span>

><span data-ttu-id="f5b7c-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f5b7c-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```


