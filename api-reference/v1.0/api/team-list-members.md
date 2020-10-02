---
title: 列出成员
description: 获取团队的 conversationMembers。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 801062feac6e6f7a7e7de03a145a6b83c6c12d57
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330002"
---
# <a name="list-members"></a><span data-ttu-id="32568-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="32568-103">List members</span></span>
<span data-ttu-id="32568-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32568-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32568-105">获取 [team](../resources/team.md) 的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="32568-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="32568-106">注意：此 API 当前不支持分页，因此当成员过多导致一个请求无法容纳时，将无法获取所有成员。</span><span class="sxs-lookup"><span data-stu-id="32568-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="32568-107">权限</span><span class="sxs-lookup"><span data-stu-id="32568-107">Permissions</span></span>
<span data-ttu-id="32568-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32568-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32568-110">Permission type</span></span>|<span data-ttu-id="32568-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32568-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32568-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32568-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32568-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32568-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="32568-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32568-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32568-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32568-115">Not supported.</span></span>    |
|<span data-ttu-id="32568-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32568-116">Application</span></span>|<span data-ttu-id="32568-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32568-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32568-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32568-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
GET /teams/{teamsId}/channels/{channelId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32568-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="32568-119">Optional query parameters</span></span>
<span data-ttu-id="32568-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="32568-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="32568-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="32568-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="32568-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="32568-122">Request headers</span></span>
|<span data-ttu-id="32568-123">名称</span><span class="sxs-lookup"><span data-stu-id="32568-123">Name</span></span>|<span data-ttu-id="32568-124">说明</span><span class="sxs-lookup"><span data-stu-id="32568-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32568-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="32568-125">Authorization</span></span>|<span data-ttu-id="32568-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32568-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32568-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="32568-128">Request body</span></span>
<span data-ttu-id="32568-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32568-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32568-130">响应</span><span class="sxs-lookup"><span data-stu-id="32568-130">Response</span></span>

<span data-ttu-id="32568-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="32568-131">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32568-132">示例</span><span class="sxs-lookup"><span data-stu-id="32568-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32568-133">请求</span><span class="sxs-lookup"><span data-stu-id="32568-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="32568-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="32568-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="32568-135">C#</span><span class="sxs-lookup"><span data-stu-id="32568-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32568-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32568-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32568-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32568-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32568-138">Java</span><span class="sxs-lookup"><span data-stu-id="32568-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="32568-139">响应</span><span class="sxs-lookup"><span data-stu-id="32568-139">Response</span></span>
<span data-ttu-id="32568-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="32568-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
