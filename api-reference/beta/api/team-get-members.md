---
title: 获取团队成员
description: 获取团队成员。
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a12455b9fb2d51c13dc725ec509542136affa1e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060320"
---
# <a name="get-member-of-team"></a><span data-ttu-id="451a5-103">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="451a5-103">Get member of team</span></span>

<span data-ttu-id="451a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="451a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="451a5-105">从 [团队](../resources/team.md) 中获取新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="451a5-105">Get a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="451a5-106">权限</span><span class="sxs-lookup"><span data-stu-id="451a5-106">Permissions</span></span>

<span data-ttu-id="451a5-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="451a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="451a5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="451a5-109">Permission Type</span></span>|<span data-ttu-id="451a5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="451a5-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="451a5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="451a5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="451a5-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="451a5-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="451a5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="451a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="451a5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="451a5-114">Not supported.</span></span>    |
|<span data-ttu-id="451a5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="451a5-115">Application</span></span>| <span data-ttu-id="451a5-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="451a5-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="451a5-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="451a5-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="451a5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="451a5-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="451a5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="451a5-119">Optional query parameters</span></span>

<span data-ttu-id="451a5-120">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="451a5-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="451a5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="451a5-121">Request headers</span></span>

| <span data-ttu-id="451a5-122">标头</span><span class="sxs-lookup"><span data-stu-id="451a5-122">Header</span></span>       | <span data-ttu-id="451a5-123">值</span><span class="sxs-lookup"><span data-stu-id="451a5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="451a5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="451a5-124">Authorization</span></span>  | <span data-ttu-id="451a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="451a5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="451a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="451a5-127">Request body</span></span>

<span data-ttu-id="451a5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="451a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="451a5-129">响应</span><span class="sxs-lookup"><span data-stu-id="451a5-129">Response</span></span>

<span data-ttu-id="451a5-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="451a5-130">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="451a5-131">示例</span><span class="sxs-lookup"><span data-stu-id="451a5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="451a5-132">请求</span><span class="sxs-lookup"><span data-stu-id="451a5-132">Request</span></span>

<span data-ttu-id="451a5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="451a5-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="451a5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="451a5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members//ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="451a5-135">C#</span><span class="sxs-lookup"><span data-stu-id="451a5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="451a5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="451a5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="451a5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="451a5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="451a5-138">Java</span><span class="sxs-lookup"><span data-stu-id="451a5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="451a5-139">响应</span><span class="sxs-lookup"><span data-stu-id="451a5-139">Response</span></span>

<span data-ttu-id="451a5-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="451a5-140">Here is an example of the response.</span></span>

><span data-ttu-id="451a5-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="451a5-141">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
   "@odata.type":"#microsoft.graph.aadUserConversationMember",
   "id":"/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
   "roles":[
      "owner"
   ],
   "displayName":"John Doe",
   "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
   "email":null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "get_team_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="451a5-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="451a5-142">See also</span></span>

- [<span data-ttu-id="451a5-143">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="451a5-143">Get member of channel</span></span>](channel-get-members.md)

