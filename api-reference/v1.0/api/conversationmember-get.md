---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d010f19945b08a7bd127c19a0938473b73ff0fae
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377094"
---
# <a name="get-conversationmember"></a><span data-ttu-id="8542e-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="8542e-103">Get conversationMember</span></span>

<span data-ttu-id="8542e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8542e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8542e-105">检索[聊天](../resources/chatmessage.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="8542e-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8542e-106">权限</span><span class="sxs-lookup"><span data-stu-id="8542e-106">Permissions</span></span>

<span data-ttu-id="8542e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8542e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8542e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8542e-109">Permission Type</span></span>|<span data-ttu-id="8542e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8542e-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8542e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8542e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8542e-112">对于 **用户** 或 **聊天** 资源：Chat.ReadBasic、Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8542e-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="8542e-113">对于 **频道** 资源：ChannelMember.Read.All、ChannelMember.ReadWrite、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8542e-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="8542e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8542e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8542e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8542e-115">Not supported.</span></span>|
|<span data-ttu-id="8542e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8542e-116">Application</span></span>| <span data-ttu-id="8542e-117">对于 **用户** 或 **聊天** 资源：不支持。</span><span class="sxs-lookup"><span data-stu-id="8542e-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="8542e-118">对于 **频道** 资源：TeamMember.Read.Group\*、ChannelMember.Read.All、ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8542e-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="8542e-119">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="8542e-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="8542e-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="8542e-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="8542e-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="8542e-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="8542e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8542e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8542e-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8542e-123">Optional query parameters</span></span>

<span data-ttu-id="8542e-124">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8542e-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8542e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="8542e-125">Request headers</span></span>

| <span data-ttu-id="8542e-126">标头</span><span class="sxs-lookup"><span data-stu-id="8542e-126">Header</span></span>       | <span data-ttu-id="8542e-127">值</span><span class="sxs-lookup"><span data-stu-id="8542e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8542e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8542e-128">Authorization</span></span>  | <span data-ttu-id="8542e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8542e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8542e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="8542e-131">Request body</span></span>

<span data-ttu-id="8542e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8542e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8542e-133">响应</span><span class="sxs-lookup"><span data-stu-id="8542e-133">Response</span></span>

<span data-ttu-id="8542e-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8542e-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8542e-135">示例</span><span class="sxs-lookup"><span data-stu-id="8542e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="8542e-136">请求</span><span class="sxs-lookup"><span data-stu-id="8542e-136">Request</span></span>

<span data-ttu-id="8542e-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8542e-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```

### <a name="response"></a><span data-ttu-id="8542e-138">响应</span><span class="sxs-lookup"><span data-stu-id="8542e-138">Response</span></span>

<span data-ttu-id="8542e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8542e-139">Here is an example of the response.</span></span>

><span data-ttu-id="8542e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8542e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!--
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
