---
title: 列出团队成员
description: 获取团队的 conversationMembers。
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d55cb5847faee74b10892afd679573998f203f3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872210"
---
# <a name="list-members-of-team"></a><span data-ttu-id="eebc6-103">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="eebc6-103">List members of team</span></span>
<span data-ttu-id="eebc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eebc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eebc6-105">获取 [team](../resources/team.md) 的 [conversationMember](../resources/conversationmember.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="eebc6-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="eebc6-106">必须将由服务器返回的成员资格 ID 视为不透明字符串。</span><span class="sxs-lookup"><span data-stu-id="eebc6-106">The membership IDs returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="eebc6-107">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="eebc6-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
> 
> <span data-ttu-id="eebc6-108">成员资格结果将来可能会映射到来自不同租户的用户，如响应中所示。</span><span class="sxs-lookup"><span data-stu-id="eebc6-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="eebc6-109">客户端不应假定所有成员都仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="eebc6-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="eebc6-110">权限</span><span class="sxs-lookup"><span data-stu-id="eebc6-110">Permissions</span></span>
<span data-ttu-id="eebc6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eebc6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eebc6-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="eebc6-113">Permission type</span></span>|<span data-ttu-id="eebc6-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eebc6-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eebc6-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eebc6-115">Delegated (work or school account)</span></span>| <span data-ttu-id="eebc6-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eebc6-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="eebc6-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eebc6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eebc6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eebc6-118">Not supported.</span></span>    |
|<span data-ttu-id="eebc6-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="eebc6-119">Application</span></span>| <span data-ttu-id="eebc6-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eebc6-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="eebc6-121">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="eebc6-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="eebc6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eebc6-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eebc6-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eebc6-123">Optional query parameters</span></span>
<span data-ttu-id="eebc6-124">此方法支持`$filter` 和 `$select` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eebc6-124">This method supports the `$filter` and `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eebc6-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="eebc6-125">Request headers</span></span>
|<span data-ttu-id="eebc6-126">名称</span><span class="sxs-lookup"><span data-stu-id="eebc6-126">Name</span></span>|<span data-ttu-id="eebc6-127">说明</span><span class="sxs-lookup"><span data-stu-id="eebc6-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eebc6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="eebc6-128">Authorization</span></span>|<span data-ttu-id="eebc6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eebc6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eebc6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="eebc6-131">Request body</span></span>
<span data-ttu-id="eebc6-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eebc6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eebc6-133">响应</span><span class="sxs-lookup"><span data-stu-id="eebc6-133">Response</span></span>

<span data-ttu-id="eebc6-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="eebc6-134">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eebc6-135">示例</span><span class="sxs-lookup"><span data-stu-id="eebc6-135">Examples</span></span>

### <a name="example-1-get-list-of-members-in-team"></a><span data-ttu-id="eebc6-136">示例 1：获取团队中的成员列表</span><span class="sxs-lookup"><span data-stu-id="eebc6-136">Example 1: Get list of members in team</span></span>

#### <a name="request"></a><span data-ttu-id="eebc6-137">请求</span><span class="sxs-lookup"><span data-stu-id="eebc6-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eebc6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="eebc6-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```
# <a name="c"></a>[<span data-ttu-id="eebc6-139">C#</span><span class="sxs-lookup"><span data-stu-id="eebc6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eebc6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eebc6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eebc6-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eebc6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eebc6-142">Java</span><span class="sxs-lookup"><span data-stu-id="eebc6-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eebc6-143">响应</span><span class="sxs-lookup"><span data-stu-id="eebc6-143">Response</span></span>
><span data-ttu-id="eebc6-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eebc6-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 3,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyM3NTJmNTBiNy0yNTZmLTQ1MzktYjc3NS1jNGQxMmYyZTQ3MjI=",
            "roles": [],
            "displayName": "Harry Johnson",
            "userId": "752f50b7-256f-4539-b775-c4d12f2e4722",
            "email": "harry@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-2-find-members-of-a-team-by-their-azure-ad-user-object-id"></a><span data-ttu-id="eebc6-145">示例 2：按 Azure AD 用户对象 ID 查找团队成员</span><span class="sxs-lookup"><span data-stu-id="eebc6-145">Example 2: Find members of a team by their Azure AD user object ID</span></span>

<span data-ttu-id="eebc6-146">以下示例显示了根据与 [aadUserConversationMember](../resources/aaduserconversationmember.md) 相关联的 [Azure AD 用户](../resources/user.md)的 `id` 查找成员资格资源的请求。 </span><span class="sxs-lookup"><span data-stu-id="eebc6-146">The following example shows a request to find the membership resources based on `id` of the [Azure AD user](../resources/user.md) associated with the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="eebc6-147">请求</span><span class="sxs-lookup"><span data-stu-id="eebc6-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eebc6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="eebc6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_userid"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')

```
# <a name="c"></a>[<span data-ttu-id="eebc6-149">C#</span><span class="sxs-lookup"><span data-stu-id="eebc6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-userid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eebc6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eebc6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-userid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eebc6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eebc6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-userid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eebc6-152">Java</span><span class="sxs-lookup"><span data-stu-id="eebc6-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-userid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eebc6-153">响应</span><span class="sxs-lookup"><span data-stu-id="eebc6-153">Response</span></span>
><span data-ttu-id="eebc6-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eebc6-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_userid",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-3-find-members-of-a-team-by-their-names-or-email"></a><span data-ttu-id="eebc6-155">示例 3：按姓名或电子邮件查找团队成员</span><span class="sxs-lookup"><span data-stu-id="eebc6-155">Example 3: Find members of a team by their names or email</span></span>

<span data-ttu-id="eebc6-156">以下示例显示了根据 [aadUserConversationMember](../resources/aaduserconversationmember.md) 的 `displayName` 或 `email` 查找成员资格资源的请求。</span><span class="sxs-lookup"><span data-stu-id="eebc6-156">The following example shows a request to find the membership resources based on `displayName` or `email` of the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="eebc6-157">请求</span><span class="sxs-lookup"><span data-stu-id="eebc6-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eebc6-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="eebc6-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_username_or_email"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="eebc6-159">C#</span><span class="sxs-lookup"><span data-stu-id="eebc6-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-username-or-email-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eebc6-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eebc6-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-username-or-email-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eebc6-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eebc6-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-username-or-email-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eebc6-162">Java</span><span class="sxs-lookup"><span data-stu-id="eebc6-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-username-or-email-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eebc6-163">响应</span><span class="sxs-lookup"><span data-stu-id="eebc6-163">Response</span></span>
><span data-ttu-id="eebc6-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eebc6-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_username_or_email",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyM3NTJmNTBiNy0yNTZmLTQ1MzktYjc3NS1jNGQxMmYyZTQ3MjI=",
            "roles": [],
            "displayName": "Harry Johnson",
            "userId": "752f50b7-256f-4539-b775-c4d12f2e4722",
            "email": "harry@M365x987948.OnMicrosoft.com"
        }
    ]
}
```
## <a name="see-also"></a><span data-ttu-id="eebc6-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eebc6-165">See also</span></span>

- [<span data-ttu-id="eebc6-166">列出频道中的成员</span><span class="sxs-lookup"><span data-stu-id="eebc6-166">List members in channel</span></span>](channel-list-members.md)
