---
title: 向团队添加成员
description: 向团队添加新成员。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 932c5e59d38c2dec7364299202f293f01e6e1513
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314442"
---
# <a name="create-members"></a><span data-ttu-id="dd5e5-103">创建成员</span><span class="sxs-lookup"><span data-stu-id="dd5e5-103">Create members</span></span>
<span data-ttu-id="dd5e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd5e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd5e5-105">向 [team](../resources/team.md) 添加新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd5e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd5e5-106">Permissions</span></span>
<span data-ttu-id="dd5e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd5e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd5e5-109">Permission type</span></span>|<span data-ttu-id="dd5e5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd5e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd5e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd5e5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="dd5e5-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd5e5-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="dd5e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd5e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd5e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-114">Not supported.</span></span>    |
|<span data-ttu-id="dd5e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd5e5-115">Application</span></span>| <span data-ttu-id="dd5e5-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd5e5-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd5e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd5e5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="dd5e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd5e5-118">Request headers</span></span>
|<span data-ttu-id="dd5e5-119">名称</span><span class="sxs-lookup"><span data-stu-id="dd5e5-119">Name</span></span>|<span data-ttu-id="dd5e5-120">说明</span><span class="sxs-lookup"><span data-stu-id="dd5e5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dd5e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd5e5-121">Authorization</span></span>|<span data-ttu-id="dd5e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dd5e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd5e5-124">Content-Type</span></span>|<span data-ttu-id="dd5e5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="dd5e5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd5e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd5e5-127">Request body</span></span>
<span data-ttu-id="dd5e5-128">在请求正文中，提供 JSON 表示形式的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd5e5-129">响应</span><span class="sxs-lookup"><span data-stu-id="dd5e5-129">Response</span></span>

<span data-ttu-id="dd5e5-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd5e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="dd5e5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd5e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="dd5e5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dd5e5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd5e5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{id}/members
Content-type: application/json
Content-length: 26

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="dd5e5-134">C#</span><span class="sxs-lookup"><span data-stu-id="dd5e5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd5e5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd5e5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd5e5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd5e5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd5e5-137">Java</span><span class="sxs-lookup"><span data-stu-id="dd5e5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dd5e5-138">响应</span><span class="sxs-lookup"><span data-stu-id="dd5e5-138">Response</span></span>
<span data-ttu-id="dd5e5-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dd5e5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "3c02af05-9312-4966-bc84-c1a0818791c4",
    "roles": [
        "owner"
    ],
    "userId": "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    "displayName": "Cameron White",
    "email": "CameronW@M365x987948.OnMicrosoft.com"
}
```
