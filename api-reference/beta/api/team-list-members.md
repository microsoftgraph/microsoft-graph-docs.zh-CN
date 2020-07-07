---
title: 列出成员
description: 获取团队的 conversationMembers。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9adfa391634164af0818bd81b2cc33d9969a79df
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051002"
---
# <a name="list-members"></a><span data-ttu-id="b3854-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="b3854-103">List members</span></span>
<span data-ttu-id="b3854-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3854-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3854-105">获取[团队](../resources/team.md)的[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="b3854-105">Get the [conversationMember](../resources/conversationmember.md) of a [team](../resources/team.md).</span></span>

><span data-ttu-id="b3854-106">注意：此 API 当前不支持分页，因此如果有过多的成员适合一个请求，则不会获取所有成员。</span><span class="sxs-lookup"><span data-stu-id="b3854-106">Note: This API currently does not support pagination, so if there's too many members to fit into one request, you won't get all the members.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3854-107">权限</span><span class="sxs-lookup"><span data-stu-id="b3854-107">Permissions</span></span>
<span data-ttu-id="b3854-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b3854-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b3854-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3854-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3854-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3854-110">Permission type</span></span>|<span data-ttu-id="b3854-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3854-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3854-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3854-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3854-113">TeamMember、TeamMember 和所有</span><span class="sxs-lookup"><span data-stu-id="b3854-113">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="b3854-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3854-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3854-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3854-115">Not supported.</span></span>    |
|<span data-ttu-id="b3854-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3854-116">Application</span></span>|<span data-ttu-id="b3854-117">TeamMember、TeamMember 和所有</span><span class="sxs-lookup"><span data-stu-id="b3854-117">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3854-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3854-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3854-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3854-119">Optional query parameters</span></span>
<span data-ttu-id="b3854-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b3854-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b3854-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b3854-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3854-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3854-122">Request headers</span></span>
|<span data-ttu-id="b3854-123">名称</span><span class="sxs-lookup"><span data-stu-id="b3854-123">Name</span></span>|<span data-ttu-id="b3854-124">说明</span><span class="sxs-lookup"><span data-stu-id="b3854-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3854-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3854-125">Authorization</span></span>|<span data-ttu-id="b3854-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b3854-126">Bearer {token}.</span></span> <span data-ttu-id="b3854-127">Required.</span><span class="sxs-lookup"><span data-stu-id="b3854-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3854-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3854-128">Request body</span></span>
<span data-ttu-id="b3854-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3854-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3854-130">响应</span><span class="sxs-lookup"><span data-stu-id="b3854-130">Response</span></span>

<span data-ttu-id="b3854-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[conversationMember](../resources/conversationmember.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b3854-131">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3854-132">示例</span><span class="sxs-lookup"><span data-stu-id="b3854-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3854-133">请求</span><span class="sxs-lookup"><span data-stu-id="b3854-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### <a name="response"></a><span data-ttu-id="b3854-134">响应</span><span class="sxs-lookup"><span data-stu-id="b3854-134">Response</span></span>
<span data-ttu-id="b3854-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b3854-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
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
