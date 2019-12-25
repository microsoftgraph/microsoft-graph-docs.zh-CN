---
title: 添加 conversationMember
description: 将 conversationMember 添加到频道。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ac5cdef288ed45c1fb45c2d64d026241018528f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868737"
---
# <a name="add-conversationmember"></a><span data-ttu-id="825b8-103">添加 conversationMember</span><span class="sxs-lookup"><span data-stu-id="825b8-103">Add conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="825b8-104">将[conversationMember](../resources/conversationmember.md)添加到[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="825b8-104">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

> [!NOTE]
><span data-ttu-id="825b8-105">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的`private`通道上受支持。</span><span class="sxs-lookup"><span data-stu-id="825b8-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="825b8-106">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回400错误请求响应。</span><span class="sxs-lookup"><span data-stu-id="825b8-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a 400 Bad Request response.</span></span>

## <a name="permissions"></a><span data-ttu-id="825b8-107">权限</span><span class="sxs-lookup"><span data-stu-id="825b8-107">Permissions</span></span>

<span data-ttu-id="825b8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="825b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="825b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="825b8-110">Permission Type</span></span>|<span data-ttu-id="825b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="825b8-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="825b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="825b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="825b8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825b8-113">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="825b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="825b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="825b8-115">不支持</span><span class="sxs-lookup"><span data-stu-id="825b8-115">Not supported</span></span>|
|<span data-ttu-id="825b8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="825b8-116">Application</span></span>|<span data-ttu-id="825b8-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825b8-117">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="825b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="825b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="825b8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="825b8-119">Request headers</span></span>

| <span data-ttu-id="825b8-120">标头</span><span class="sxs-lookup"><span data-stu-id="825b8-120">Header</span></span>       | <span data-ttu-id="825b8-121">值</span><span class="sxs-lookup"><span data-stu-id="825b8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="825b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="825b8-122">Authorization</span></span>  | <span data-ttu-id="825b8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="825b8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="825b8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="825b8-125">Request body</span></span>

<span data-ttu-id="825b8-126">请求正文中包含以下属性。</span><span class="sxs-lookup"><span data-stu-id="825b8-126">Include the following properties in the request body.</span></span>

| <span data-ttu-id="825b8-127">属性</span><span class="sxs-lookup"><span data-stu-id="825b8-127">Property</span></span>   | <span data-ttu-id="825b8-128">类型</span><span class="sxs-lookup"><span data-stu-id="825b8-128">Type</span></span> |<span data-ttu-id="825b8-129">说明</span><span class="sxs-lookup"><span data-stu-id="825b8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="825b8-130">角色</span><span class="sxs-lookup"><span data-stu-id="825b8-130">roles</span></span>|<span data-ttu-id="825b8-131">string 集合</span><span class="sxs-lookup"><span data-stu-id="825b8-131">string collection</span></span>|<span data-ttu-id="825b8-132">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="825b8-132">The roles for that user.</span></span>|
|<span data-ttu-id="825b8-133">user</span><span class="sxs-lookup"><span data-stu-id="825b8-133">user</span></span>|[<span data-ttu-id="825b8-134">user</span><span class="sxs-lookup"><span data-stu-id="825b8-134">user</span></span>](../resources/user.md)|<span data-ttu-id="825b8-135">要添加到频道的用户。</span><span class="sxs-lookup"><span data-stu-id="825b8-135">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="825b8-136">响应</span><span class="sxs-lookup"><span data-stu-id="825b8-136">Response</span></span>

<span data-ttu-id="825b8-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="825b8-137">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="825b8-138">示例</span><span class="sxs-lookup"><span data-stu-id="825b8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="825b8-139">请求</span><span class="sxs-lookup"><span data-stu-id="825b8-139">Request</span></span>

<span data-ttu-id="825b8-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="825b8-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="825b8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="825b8-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="825b8-142">C#</span><span class="sxs-lookup"><span data-stu-id="825b8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="825b8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="825b8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="825b8-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="825b8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="825b8-145">响应</span><span class="sxs-lookup"><span data-stu-id="825b8-145">Response</span></span>

<span data-ttu-id="825b8-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="825b8-146">Here is an example of the response.</span></span>

><span data-ttu-id="825b8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="825b8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
