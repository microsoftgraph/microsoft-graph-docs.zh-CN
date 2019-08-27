---
title: 更新 conversationMember
description: 在频道中更新 conversationMember 的角色。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d1fad235333e968317d3e4681f56b501016d6352
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633901"
---
# <a name="update-conversationmember"></a><span data-ttu-id="88cae-103">更新 conversationMember</span><span class="sxs-lookup"><span data-stu-id="88cae-103">Update conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88cae-104">在[频道](../resources/channel.md)中更新[conversationMember](../resources/conversationmember.md)的角色。</span><span class="sxs-lookup"><span data-stu-id="88cae-104">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="88cae-105">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的`private`通道上受支持。</span><span class="sxs-lookup"><span data-stu-id="88cae-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="88cae-106">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回`400 Bad Request`响应。</span><span class="sxs-lookup"><span data-stu-id="88cae-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="88cae-107">权限</span><span class="sxs-lookup"><span data-stu-id="88cae-107">Permissions</span></span>

<span data-ttu-id="88cae-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88cae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88cae-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="88cae-110">Permission Type</span></span>|<span data-ttu-id="88cae-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88cae-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="88cae-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88cae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88cae-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88cae-113">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="88cae-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88cae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88cae-115">不支持</span><span class="sxs-lookup"><span data-stu-id="88cae-115">Not supported</span></span>|
|<span data-ttu-id="88cae-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="88cae-116">Application</span></span>|<span data-ttu-id="88cae-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88cae-117">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88cae-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88cae-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="88cae-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="88cae-119">Request headers</span></span>

| <span data-ttu-id="88cae-120">标头</span><span class="sxs-lookup"><span data-stu-id="88cae-120">Header</span></span>       | <span data-ttu-id="88cae-121">值</span><span class="sxs-lookup"><span data-stu-id="88cae-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88cae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="88cae-122">Authorization</span></span>  | <span data-ttu-id="88cae-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88cae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88cae-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="88cae-125">Request body</span></span>

<span data-ttu-id="88cae-126">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="88cae-126">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="88cae-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="88cae-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="88cae-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="88cae-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="88cae-129">属性</span><span class="sxs-lookup"><span data-stu-id="88cae-129">Property</span></span>   | <span data-ttu-id="88cae-130">类型</span><span class="sxs-lookup"><span data-stu-id="88cae-130">Type</span></span> |<span data-ttu-id="88cae-131">说明</span><span class="sxs-lookup"><span data-stu-id="88cae-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88cae-132">roles</span><span class="sxs-lookup"><span data-stu-id="88cae-132">roles</span></span>|<span data-ttu-id="88cae-133">字符串集合</span><span class="sxs-lookup"><span data-stu-id="88cae-133">string collection</span></span>|<span data-ttu-id="88cae-134">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="88cae-134">The roles for that user.</span></span> <span data-ttu-id="88cae-135">必须为 "owner" 或空。</span><span class="sxs-lookup"><span data-stu-id="88cae-135">Must be "owner" or empty.</span></span> <span data-ttu-id="88cae-136">来宾用户必须始终拥有角色 "来宾", 并且无法更改。</span><span class="sxs-lookup"><span data-stu-id="88cae-136">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="88cae-137">响应</span><span class="sxs-lookup"><span data-stu-id="88cae-137">Response</span></span>

<span data-ttu-id="88cae-138">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[conversationMember](../resources/conversationmember.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88cae-138">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88cae-139">示例</span><span class="sxs-lookup"><span data-stu-id="88cae-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="88cae-140">请求</span><span class="sxs-lookup"><span data-stu-id="88cae-140">Request</span></span>

<span data-ttu-id="88cae-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88cae-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="88cae-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="88cae-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="88cae-143">C#</span><span class="sxs-lookup"><span data-stu-id="88cae-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88cae-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88cae-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88cae-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="88cae-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88cae-146">响应</span><span class="sxs-lookup"><span data-stu-id="88cae-146">Response</span></span>

<span data-ttu-id="88cae-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88cae-147">Here is an example of the response.</span></span>

><span data-ttu-id="88cae-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88cae-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
