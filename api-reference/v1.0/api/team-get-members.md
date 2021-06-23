---
title: 获取团队成员
description: 获取团队成员。
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5ee28e588be74979259f1cf7dfa63cc5635d441f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060510"
---
# <a name="get-member-of-team"></a><span data-ttu-id="c42a0-103">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="c42a0-103">Get member of team</span></span>

<span data-ttu-id="c42a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c42a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c42a0-105">从 [团队](../resources/team.md) 中获取新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="c42a0-105">Get a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c42a0-106">权限</span><span class="sxs-lookup"><span data-stu-id="c42a0-106">Permissions</span></span>

<span data-ttu-id="c42a0-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c42a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c42a0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c42a0-109">Permission Type</span></span>|<span data-ttu-id="c42a0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c42a0-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c42a0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c42a0-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c42a0-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c42a0-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="c42a0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c42a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c42a0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c42a0-114">Not supported.</span></span>    |
|<span data-ttu-id="c42a0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c42a0-115">Application</span></span>| <span data-ttu-id="c42a0-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c42a0-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="c42a0-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="c42a0-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="c42a0-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="c42a0-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c42a0-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="c42a0-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c42a0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c42a0-120">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c42a0-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c42a0-121">Optional query parameters</span></span>

<span data-ttu-id="c42a0-122">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c42a0-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c42a0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c42a0-123">Request headers</span></span>

| <span data-ttu-id="c42a0-124">标头</span><span class="sxs-lookup"><span data-stu-id="c42a0-124">Header</span></span>       | <span data-ttu-id="c42a0-125">值</span><span class="sxs-lookup"><span data-stu-id="c42a0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c42a0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c42a0-126">Authorization</span></span>  | <span data-ttu-id="c42a0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c42a0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c42a0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c42a0-129">Request body</span></span>

<span data-ttu-id="c42a0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c42a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c42a0-131">响应</span><span class="sxs-lookup"><span data-stu-id="c42a0-131">Response</span></span>

<span data-ttu-id="c42a0-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c42a0-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c42a0-133">示例</span><span class="sxs-lookup"><span data-stu-id="c42a0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c42a0-134">请求</span><span class="sxs-lookup"><span data-stu-id="c42a0-134">Request</span></span>

<span data-ttu-id="c42a0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c42a0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c42a0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c42a0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="c42a0-137">C#</span><span class="sxs-lookup"><span data-stu-id="c42a0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c42a0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c42a0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c42a0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c42a0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c42a0-140">Java</span><span class="sxs-lookup"><span data-stu-id="c42a0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c42a0-141">响应</span><span class="sxs-lookup"><span data-stu-id="c42a0-141">Response</span></span>

<span data-ttu-id="c42a0-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c42a0-142">Here is an example of the response.</span></span>

><span data-ttu-id="c42a0-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c42a0-143">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
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

## <a name="see-also"></a><span data-ttu-id="c42a0-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c42a0-144">See also</span></span>

- [<span data-ttu-id="c42a0-145">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="c42a0-145">Get member of channel</span></span>](channel-get-members.md)

