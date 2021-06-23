---
title: 列出频道的成员
description: 列出频道成员。
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dd59e40abbd24a80af11fa4bcde48ecbbe3def98
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060018"
---
# <a name="list-members-of-a-channel"></a><span data-ttu-id="4775b-103">列出频道的成员</span><span class="sxs-lookup"><span data-stu-id="4775b-103">List members of a channel</span></span>

<span data-ttu-id="4775b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4775b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4775b-105">从[频道](../resources/channel.md)中检索[conversationMembers](../resources/conversationmember.md)列表。</span><span class="sxs-lookup"><span data-stu-id="4775b-105">Retrieve a list of [conversationMembers](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="4775b-106">必须将由服务器返回的成员资格 ID 视为不透明字符串。</span><span class="sxs-lookup"><span data-stu-id="4775b-106">The membership IDs returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="4775b-107">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="4775b-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="4775b-p102">未来，成员资格结果可以映射到来自不同租户的用户，如响应中所示。客户端不应假定所有成员仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="4775b-p102">The membership results could map to users from different tenants, as indicated in the response, in the future. The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="4775b-110">权限</span><span class="sxs-lookup"><span data-stu-id="4775b-110">Permissions</span></span>

<span data-ttu-id="4775b-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4775b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4775b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4775b-113">Permission Type</span></span>|<span data-ttu-id="4775b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4775b-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4775b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4775b-115">Delegated (work or school account)</span></span>|<span data-ttu-id="4775b-116">ChannelMember.Read.All、 ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4775b-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="4775b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4775b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4775b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4775b-118">Not supported.</span></span>|
|<span data-ttu-id="4775b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4775b-119">Application</span></span>|<span data-ttu-id="4775b-120">ChannelMember.Read.All、 ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4775b-120">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="4775b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4775b-121">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
GET /teams/{team-id}/channels/{channel-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4775b-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4775b-122">Optional query parameters</span></span>

<span data-ttu-id="4775b-123">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4775b-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4775b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4775b-124">Request headers</span></span>

| <span data-ttu-id="4775b-125">标头</span><span class="sxs-lookup"><span data-stu-id="4775b-125">Header</span></span>       | <span data-ttu-id="4775b-126">值</span><span class="sxs-lookup"><span data-stu-id="4775b-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4775b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4775b-127">Authorization</span></span>  | <span data-ttu-id="4775b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4775b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4775b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4775b-130">Request body</span></span>

<span data-ttu-id="4775b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4775b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4775b-132">响应</span><span class="sxs-lookup"><span data-stu-id="4775b-132">Response</span></span>

<span data-ttu-id="4775b-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4775b-133">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4775b-134">示例</span><span class="sxs-lookup"><span data-stu-id="4775b-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="4775b-135">请求</span><span class="sxs-lookup"><span data-stu-id="4775b-135">Request</span></span>

<span data-ttu-id="4775b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4775b-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4775b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4775b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel-list_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/2ab9c796-2902-45f8-b712-7c5a63cf41c4/channels/19%3A20bc1df46b1148e9b22539b83bc66809%40thread.skype/members
```
# <a name="c"></a>[<span data-ttu-id="4775b-138">C#</span><span class="sxs-lookup"><span data-stu-id="4775b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-list-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4775b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4775b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-list-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4775b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4775b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-list-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4775b-141">Java</span><span class="sxs-lookup"><span data-stu-id="4775b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-list-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4775b-142">响应</span><span class="sxs-lookup"><span data-stu-id="4775b-142">Response</span></span>

<span data-ttu-id="4775b-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4775b-143">Here is an example of the response.</span></span>

><span data-ttu-id="4775b-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4775b-144">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
"@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('2ab9c796-2902-45f8-b712-7c5a63cf41c4')/channels('19%3A20bc1df46b1148e9b22539b83bc66809%40thread.skype')/members",
"@odata.count": 2,
"value": [
    {
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ=",
        "roles": [],
        "displayName": "Jane Doe",
        "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
        "email": "jdoe@teamsip.onmicrosoft.com"
    },
    {
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNiMzI0NmY0NC1jMDkxLTQ2MjctOTZjNi0yNWIxOGZhMmM5MTA=",
        "roles": [
            "owner"
        ],
        "displayName": "Ace John",
        "userId": "b3246f44-c091-4627-96c6-25b18fa2c910",
        "email": "ajohn@teamsip.onmicrosoft.com"
    }
]
}

```

## <a name="see-also"></a><span data-ttu-id="4775b-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4775b-145">See also</span></span>

- [<span data-ttu-id="4775b-146">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="4775b-146">List members of team</span></span>](team-list-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
