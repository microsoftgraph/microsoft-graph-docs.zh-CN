---
title: 更新团队中的成员
description: 更新团队中成员的角色。
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0970bc564d23cfaadd7238f25c3afd0a487540f6
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060427"
---
# <a name="update-member-in-team"></a><span data-ttu-id="89b58-103">更新团队中的成员</span><span class="sxs-lookup"><span data-stu-id="89b58-103">Update member in team</span></span>

<span data-ttu-id="89b58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89b58-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89b58-105">更新团队 [中 conversationMember](../resources/conversationmember.md) [的角色](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="89b58-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89b58-106">权限</span><span class="sxs-lookup"><span data-stu-id="89b58-106">Permissions</span></span>

<span data-ttu-id="89b58-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89b58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89b58-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89b58-109">Permission Type</span></span>|<span data-ttu-id="89b58-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89b58-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="89b58-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89b58-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89b58-112">TeamMember.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="89b58-112">TeamMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="89b58-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89b58-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89b58-114">不支持</span><span class="sxs-lookup"><span data-stu-id="89b58-114">Not supported</span></span>|
|<span data-ttu-id="89b58-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="89b58-115">Application</span></span>|<span data-ttu-id="89b58-116">TeamMember.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="89b58-116">TeamMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89b58-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89b58-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="89b58-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="89b58-118">Request headers</span></span>

| <span data-ttu-id="89b58-119">标头</span><span class="sxs-lookup"><span data-stu-id="89b58-119">Header</span></span>       | <span data-ttu-id="89b58-120">值</span><span class="sxs-lookup"><span data-stu-id="89b58-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89b58-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89b58-121">Authorization</span></span>  | <span data-ttu-id="89b58-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89b58-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89b58-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="89b58-124">Content-type</span></span> | <span data-ttu-id="89b58-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="89b58-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89b58-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="89b58-127">Request body</span></span>

<span data-ttu-id="89b58-128">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="89b58-128">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="89b58-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="89b58-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="89b58-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="89b58-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="89b58-131">属性</span><span class="sxs-lookup"><span data-stu-id="89b58-131">Property</span></span>   | <span data-ttu-id="89b58-132">类型</span><span class="sxs-lookup"><span data-stu-id="89b58-132">Type</span></span> |<span data-ttu-id="89b58-133">说明</span><span class="sxs-lookup"><span data-stu-id="89b58-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89b58-134">角色</span><span class="sxs-lookup"><span data-stu-id="89b58-134">roles</span></span>|<span data-ttu-id="89b58-135">string 集合</span><span class="sxs-lookup"><span data-stu-id="89b58-135">string collection</span></span>|<span data-ttu-id="89b58-136">用户的角色。</span><span class="sxs-lookup"><span data-stu-id="89b58-136">The role for the user.</span></span> <span data-ttu-id="89b58-137">必须为空 `owner` 。</span><span class="sxs-lookup"><span data-stu-id="89b58-137">Must be `owner` or empty.</span></span> <span data-ttu-id="89b58-138">来宾用户将自动标记 `guest` 角色，并且此值无法更新。</span><span class="sxs-lookup"><span data-stu-id="89b58-138">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="89b58-139">响应</span><span class="sxs-lookup"><span data-stu-id="89b58-139">Response</span></span>

<span data-ttu-id="89b58-140">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89b58-140">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b58-141">示例</span><span class="sxs-lookup"><span data-stu-id="89b58-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="89b58-142">请求</span><span class="sxs-lookup"><span data-stu-id="89b58-142">Request</span></span>

<span data-ttu-id="89b58-143">下面是一个请求，要求将角色 `owner` 应用于团队的现有成员。</span><span class="sxs-lookup"><span data-stu-id="89b58-143">The following is a request to apply the `owner` role to an existing member of a team.</span></span>


# <a name="http"></a>[<span data-ttu-id="89b58-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="89b58-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member_2"
} -->
```http
PATCH https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="89b58-145">C#</span><span class="sxs-lookup"><span data-stu-id="89b58-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89b58-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89b58-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89b58-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89b58-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89b58-148">Java</span><span class="sxs-lookup"><span data-stu-id="89b58-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89b58-149">响应</span><span class="sxs-lookup"><span data-stu-id="89b58-149">Response</span></span>

><span data-ttu-id="89b58-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89b58-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="89b58-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89b58-151">See also</span></span>

- [<span data-ttu-id="89b58-152">更新频道中的成员</span><span class="sxs-lookup"><span data-stu-id="89b58-152">Update member in channel</span></span>](channel-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of team member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
