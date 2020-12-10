---
title: 列出团队成员
description: 获取团队的 conversationMembers。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 842010263da003a1317fe2a90d1511d1d6465b62
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387765"
---
# <a name="list-members-of-team"></a><span data-ttu-id="0c693-103">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="0c693-103">List members of team</span></span>
<span data-ttu-id="0c693-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c693-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c693-105">获取 [team](../resources/team.md) 的 [conversationMember](../resources/conversationmember.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="0c693-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="0c693-106">必须将由服务器返回的成员资格 ID 视为不透明字符串。</span><span class="sxs-lookup"><span data-stu-id="0c693-106">The membership IDs returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="0c693-107">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="0c693-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
> 
> <span data-ttu-id="0c693-108">成员资格结果将来可能会映射到来自不同租户的用户，如响应中所示。</span><span class="sxs-lookup"><span data-stu-id="0c693-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="0c693-109">客户端不应假定所有成员都仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="0c693-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c693-110">权限</span><span class="sxs-lookup"><span data-stu-id="0c693-110">Permissions</span></span>
<span data-ttu-id="0c693-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c693-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c693-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c693-113">Permission type</span></span>|<span data-ttu-id="0c693-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0c693-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c693-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c693-115">Delegated (work or school account)</span></span>| <span data-ttu-id="0c693-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c693-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="0c693-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c693-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c693-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c693-118">Not supported.</span></span>    |
|<span data-ttu-id="0c693-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c693-119">Application</span></span>| <span data-ttu-id="0c693-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c693-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="0c693-121">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="0c693-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="0c693-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c693-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c693-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c693-123">Optional query parameters</span></span>
<span data-ttu-id="0c693-124">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c693-124">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0c693-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0c693-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c693-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c693-126">Request headers</span></span>
|<span data-ttu-id="0c693-127">名称</span><span class="sxs-lookup"><span data-stu-id="0c693-127">Name</span></span>|<span data-ttu-id="0c693-128">说明</span><span class="sxs-lookup"><span data-stu-id="0c693-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c693-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c693-129">Authorization</span></span>|<span data-ttu-id="0c693-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c693-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c693-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c693-132">Request body</span></span>
<span data-ttu-id="0c693-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c693-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c693-134">响应</span><span class="sxs-lookup"><span data-stu-id="0c693-134">Response</span></span>

<span data-ttu-id="0c693-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0c693-135">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c693-136">示例</span><span class="sxs-lookup"><span data-stu-id="0c693-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c693-137">请求</span><span class="sxs-lookup"><span data-stu-id="0c693-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0c693-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c693-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```
# <a name="c"></a>[<span data-ttu-id="0c693-139">C#</span><span class="sxs-lookup"><span data-stu-id="0c693-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c693-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c693-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c693-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c693-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c693-142">Java</span><span class="sxs-lookup"><span data-stu-id="0c693-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0c693-143">响应</span><span class="sxs-lookup"><span data-stu-id="0c693-143">Response</span></span>
<span data-ttu-id="0c693-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0c693-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_conversationmember",
  "@odata.type": "collection(microsoft.graph.aadUserConversationMember)"
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
        }
    ]
}
```
## <a name="see-also"></a><span data-ttu-id="0c693-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0c693-145">See also</span></span>

- [<span data-ttu-id="0c693-146">列出频道中的成员</span><span class="sxs-lookup"><span data-stu-id="0c693-146">List members in channel</span></span>](channel-list-members.md)
