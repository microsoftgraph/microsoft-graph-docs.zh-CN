---
title: 从频道中删除成员
description: 从频道中删除成员。
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ae46702936fb82ac00c0744927c1d5b0b2ccc6dd
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060031"
---
# <a name="remove-member-from-channel"></a><span data-ttu-id="6047e-103">从频道中删除成员</span><span class="sxs-lookup"><span data-stu-id="6047e-103">Remove member from channel</span></span>

<span data-ttu-id="6047e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6047e-104">Namespace: microsoft.graph</span></span>
 
<span data-ttu-id="6047e-105">从频道[中删除 conversationMember。](../resources/conversationmember.md) [](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="6047e-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span> <span data-ttu-id="6047e-106">此操作仅允许 **membershipType** 值为 的通道 `private` 。</span><span class="sxs-lookup"><span data-stu-id="6047e-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>


## <a name="permissions"></a><span data-ttu-id="6047e-107">权限</span><span class="sxs-lookup"><span data-stu-id="6047e-107">Permissions</span></span>

<span data-ttu-id="6047e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6047e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6047e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6047e-110">Permission Type</span></span>|<span data-ttu-id="6047e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6047e-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="6047e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6047e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6047e-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6047e-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="6047e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6047e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6047e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6047e-115">Not supported.</span></span>|
|<span data-ttu-id="6047e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6047e-116">Application</span></span>| <span data-ttu-id="6047e-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6047e-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6047e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6047e-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="6047e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6047e-119">Request headers</span></span>

| <span data-ttu-id="6047e-120">标头</span><span class="sxs-lookup"><span data-stu-id="6047e-120">Header</span></span>       | <span data-ttu-id="6047e-121">值</span><span class="sxs-lookup"><span data-stu-id="6047e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6047e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6047e-122">Authorization</span></span>  | <span data-ttu-id="6047e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6047e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6047e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6047e-125">Request body</span></span>

<span data-ttu-id="6047e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6047e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6047e-127">响应</span><span class="sxs-lookup"><span data-stu-id="6047e-127">Response</span></span>

<span data-ttu-id="6047e-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6047e-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6047e-129">示例</span><span class="sxs-lookup"><span data-stu-id="6047e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6047e-130">请求</span><span class="sxs-lookup"><span data-stu-id="6047e-130">Request</span></span>

<span data-ttu-id="6047e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6047e-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6047e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6047e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel-member"
} -->
```http
DELETE https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="6047e-133">C#</span><span class="sxs-lookup"><span data-stu-id="6047e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6047e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6047e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6047e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6047e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6047e-136">Java</span><span class="sxs-lookup"><span data-stu-id="6047e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6047e-137">响应</span><span class="sxs-lookup"><span data-stu-id="6047e-137">Response</span></span>

<span data-ttu-id="6047e-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6047e-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="6047e-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6047e-139">See also</span></span>

- [<span data-ttu-id="6047e-140">从团队删除成员</span><span class="sxs-lookup"><span data-stu-id="6047e-140">Remove member from team</span></span>](team-delete-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
