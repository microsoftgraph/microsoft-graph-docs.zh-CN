---
title: 更新 conversationMember
description: 在频道中更新 conversationMember 的角色。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8046572b62374407bc077fffa40e6ab692fefb75
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491299"
---
# <a name="update-conversationmember"></a><span data-ttu-id="1a30a-103">更新 conversationMember</span><span class="sxs-lookup"><span data-stu-id="1a30a-103">Update conversationMember</span></span>

<span data-ttu-id="1a30a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a30a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a30a-105">在[频道](../resources/channel.md)中更新[conversationMember](../resources/conversationmember.md)的角色。</span><span class="sxs-lookup"><span data-stu-id="1a30a-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="1a30a-106">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的通道上受支持 `private` 。</span><span class="sxs-lookup"><span data-stu-id="1a30a-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="1a30a-107">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="1a30a-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a30a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="1a30a-108">Permissions</span></span>

<span data-ttu-id="1a30a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a30a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a30a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a30a-111">Permission Type</span></span>|<span data-ttu-id="1a30a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a30a-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1a30a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a30a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1a30a-114">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="1a30a-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1a30a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a30a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a30a-116">不支持</span><span class="sxs-lookup"><span data-stu-id="1a30a-116">Not supported</span></span>|
|<span data-ttu-id="1a30a-117">Application</span><span class="sxs-lookup"><span data-stu-id="1a30a-117">Application</span></span>| <span data-ttu-id="1a30a-118">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="1a30a-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a30a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a30a-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a30a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a30a-120">Request headers</span></span>

| <span data-ttu-id="1a30a-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a30a-121">Header</span></span>       | <span data-ttu-id="1a30a-122">值</span><span class="sxs-lookup"><span data-stu-id="1a30a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a30a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a30a-123">Authorization</span></span>  | <span data-ttu-id="1a30a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a30a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a30a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a30a-126">Request body</span></span>

<span data-ttu-id="1a30a-127">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="1a30a-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="1a30a-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="1a30a-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1a30a-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1a30a-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1a30a-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a30a-130">Property</span></span>   | <span data-ttu-id="1a30a-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a30a-131">Type</span></span> |<span data-ttu-id="1a30a-132">Description</span><span class="sxs-lookup"><span data-stu-id="1a30a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a30a-133">角色</span><span class="sxs-lookup"><span data-stu-id="1a30a-133">roles</span></span>|<span data-ttu-id="1a30a-134">string 集合</span><span class="sxs-lookup"><span data-stu-id="1a30a-134">string collection</span></span>|<span data-ttu-id="1a30a-135">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="1a30a-135">The roles for that user.</span></span> <span data-ttu-id="1a30a-136">必须为 "owner" 或空。</span><span class="sxs-lookup"><span data-stu-id="1a30a-136">Must be "owner" or empty.</span></span> <span data-ttu-id="1a30a-137">来宾用户必须始终拥有角色 "来宾"，并且无法更改。</span><span class="sxs-lookup"><span data-stu-id="1a30a-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="1a30a-138">响应</span><span class="sxs-lookup"><span data-stu-id="1a30a-138">Response</span></span>

<span data-ttu-id="1a30a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a30a-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a30a-140">示例</span><span class="sxs-lookup"><span data-stu-id="1a30a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a30a-141">请求</span><span class="sxs-lookup"><span data-stu-id="1a30a-141">Request</span></span>

<span data-ttu-id="1a30a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a30a-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a30a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a30a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="1a30a-144">C#</span><span class="sxs-lookup"><span data-stu-id="1a30a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a30a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a30a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a30a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a30a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a30a-147">响应</span><span class="sxs-lookup"><span data-stu-id="1a30a-147">Response</span></span>

<span data-ttu-id="1a30a-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a30a-148">Here is an example of the response.</span></span>

><span data-ttu-id="1a30a-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1a30a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
