---
title: 列出成员
description: 获取团队的 conversationMembers。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ff0912caecb5947e18d05ae5c7f3b36b571a158
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848624"
---
# <a name="list-members"></a><span data-ttu-id="2d9c9-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="2d9c9-103">List members</span></span>
<span data-ttu-id="2d9c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d9c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d9c9-105">获取 [team](../resources/team.md) 的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="2d9c9-106">注意：此 API 当前不支持分页，因此当成员过多导致一个请求无法容纳时，将无法获取所有成员。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d9c9-107">权限</span><span class="sxs-lookup"><span data-stu-id="2d9c9-107">Permissions</span></span>
<span data-ttu-id="2d9c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9c9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d9c9-110">Permission type</span></span>|<span data-ttu-id="2d9c9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d9c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d9c9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d9c9-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2d9c9-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9c9-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="2d9c9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d9c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d9c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-115">Not supported.</span></span>    |
|<span data-ttu-id="2d9c9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d9c9-116">Application</span></span>| <span data-ttu-id="2d9c9-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9c9-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="2d9c9-118">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-118">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="2d9c9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d9c9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d9c9-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2d9c9-120">Optional query parameters</span></span>
<span data-ttu-id="2d9c9-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2d9c9-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d9c9-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d9c9-123">Request headers</span></span>
|<span data-ttu-id="2d9c9-124">名称</span><span class="sxs-lookup"><span data-stu-id="2d9c9-124">Name</span></span>|<span data-ttu-id="2d9c9-125">说明</span><span class="sxs-lookup"><span data-stu-id="2d9c9-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d9c9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d9c9-126">Authorization</span></span>|<span data-ttu-id="2d9c9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9c9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d9c9-129">Request body</span></span>
<span data-ttu-id="2d9c9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d9c9-131">响应</span><span class="sxs-lookup"><span data-stu-id="2d9c9-131">Response</span></span>

<span data-ttu-id="2d9c9-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-132">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d9c9-133">示例</span><span class="sxs-lookup"><span data-stu-id="2d9c9-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d9c9-134">请求</span><span class="sxs-lookup"><span data-stu-id="2d9c9-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2d9c9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d9c9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="2d9c9-136">C#</span><span class="sxs-lookup"><span data-stu-id="2d9c9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d9c9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d9c9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d9c9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d9c9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d9c9-139">Java</span><span class="sxs-lookup"><span data-stu-id="2d9c9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2d9c9-140">响应</span><span class="sxs-lookup"><span data-stu-id="2d9c9-140">Response</span></span>
<span data-ttu-id="2d9c9-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2d9c9-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
