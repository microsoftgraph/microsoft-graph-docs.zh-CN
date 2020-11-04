---
title: 添加 conversationMember
description: 将 conversationMember 添加到频道。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 150c3003487ed4585951495b0f9e9ed9a6f38121
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848643"
---
# <a name="add-conversationmember"></a><span data-ttu-id="47d6d-103">添加 conversationMember</span><span class="sxs-lookup"><span data-stu-id="47d6d-103">Add conversationMember</span></span>

<span data-ttu-id="47d6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47d6d-105">将 [conversationMember](../resources/conversationmember.md) 添加到 [频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="47d6d-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="47d6d-106">权限</span><span class="sxs-lookup"><span data-stu-id="47d6d-106">Permissions</span></span>

<span data-ttu-id="47d6d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47d6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d6d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="47d6d-109">Permission Type</span></span>|<span data-ttu-id="47d6d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47d6d-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="47d6d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47d6d-111">Delegated (work or school account)</span></span>| <span data-ttu-id="47d6d-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d6d-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="47d6d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47d6d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d6d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="47d6d-114">Not supported.</span></span>|
|<span data-ttu-id="47d6d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="47d6d-115">Application</span></span>| <span data-ttu-id="47d6d-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d6d-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47d6d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47d6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="47d6d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="47d6d-118">Request headers</span></span>

| <span data-ttu-id="47d6d-119">标头</span><span class="sxs-lookup"><span data-stu-id="47d6d-119">Header</span></span>       | <span data-ttu-id="47d6d-120">值</span><span class="sxs-lookup"><span data-stu-id="47d6d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47d6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47d6d-121">Authorization</span></span>  | <span data-ttu-id="47d6d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47d6d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47d6d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="47d6d-124">Request body</span></span>

<span data-ttu-id="47d6d-125">请求正文中包含以下属性。</span><span class="sxs-lookup"><span data-stu-id="47d6d-125">Include the following properties in the request body.</span></span>

| <span data-ttu-id="47d6d-126">属性</span><span class="sxs-lookup"><span data-stu-id="47d6d-126">Property</span></span>   | <span data-ttu-id="47d6d-127">类型</span><span class="sxs-lookup"><span data-stu-id="47d6d-127">Type</span></span> |<span data-ttu-id="47d6d-128">说明</span><span class="sxs-lookup"><span data-stu-id="47d6d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47d6d-129">角色</span><span class="sxs-lookup"><span data-stu-id="47d6d-129">roles</span></span>|<span data-ttu-id="47d6d-130">string 集合</span><span class="sxs-lookup"><span data-stu-id="47d6d-130">string collection</span></span>|<span data-ttu-id="47d6d-131">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="47d6d-131">The roles for that user.</span></span>|
|<span data-ttu-id="47d6d-132">用户</span><span class="sxs-lookup"><span data-stu-id="47d6d-132">user</span></span>|[<span data-ttu-id="47d6d-133">用户</span><span class="sxs-lookup"><span data-stu-id="47d6d-133">user</span></span>](../resources/user.md)|<span data-ttu-id="47d6d-134">要添加到频道的用户。</span><span class="sxs-lookup"><span data-stu-id="47d6d-134">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="47d6d-135">响应</span><span class="sxs-lookup"><span data-stu-id="47d6d-135">Response</span></span>

<span data-ttu-id="47d6d-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47d6d-136">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d6d-137">示例</span><span class="sxs-lookup"><span data-stu-id="47d6d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d6d-138">请求</span><span class="sxs-lookup"><span data-stu-id="47d6d-138">Request</span></span>

<span data-ttu-id="47d6d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47d6d-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47d6d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="47d6d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="47d6d-141">C#</span><span class="sxs-lookup"><span data-stu-id="47d6d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47d6d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47d6d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47d6d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47d6d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47d6d-144">Java</span><span class="sxs-lookup"><span data-stu-id="47d6d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47d6d-145">响应</span><span class="sxs-lookup"><span data-stu-id="47d6d-145">Response</span></span>

<span data-ttu-id="47d6d-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="47d6d-146">Here is an example of the response.</span></span>

><span data-ttu-id="47d6d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="47d6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
