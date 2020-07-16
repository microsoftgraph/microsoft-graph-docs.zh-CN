---
title: 向团队添加成员
description: 向团队添加新成员。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a6a397e0b9f1b74d657e55354c03f062c8364dd
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142435"
---
# <a name="create-members"></a><span data-ttu-id="04b72-103">创建成员</span><span class="sxs-lookup"><span data-stu-id="04b72-103">Create members</span></span>
<span data-ttu-id="04b72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04b72-105">向 [team](../resources/team.md) 添加新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="04b72-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="04b72-106">权限</span><span class="sxs-lookup"><span data-stu-id="04b72-106">Permissions</span></span>
<span data-ttu-id="04b72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b72-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04b72-109">Permission type</span></span>|<span data-ttu-id="04b72-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04b72-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b72-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04b72-111">Delegated (work or school account)</span></span>| <span data-ttu-id="04b72-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b72-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="04b72-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04b72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b72-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04b72-114">Not supported.</span></span>    |
|<span data-ttu-id="04b72-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04b72-115">Application</span></span>| <span data-ttu-id="04b72-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b72-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b72-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04b72-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="04b72-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04b72-118">Request headers</span></span>
|<span data-ttu-id="04b72-119">名称</span><span class="sxs-lookup"><span data-stu-id="04b72-119">Name</span></span>|<span data-ttu-id="04b72-120">说明</span><span class="sxs-lookup"><span data-stu-id="04b72-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04b72-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b72-121">Authorization</span></span>|<span data-ttu-id="04b72-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04b72-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04b72-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04b72-124">Content-Type</span></span>|<span data-ttu-id="04b72-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="04b72-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b72-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04b72-127">Request body</span></span>
<span data-ttu-id="04b72-128">在请求正文中，提供 JSON 表示形式的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04b72-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04b72-129">响应</span><span class="sxs-lookup"><span data-stu-id="04b72-129">Response</span></span>

<span data-ttu-id="04b72-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04b72-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04b72-131">示例</span><span class="sxs-lookup"><span data-stu-id="04b72-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04b72-132">请求</span><span class="sxs-lookup"><span data-stu-id="04b72-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="04b72-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="04b72-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{id}/members
Content-type: application/json
Content-length: 26

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="04b72-134">C#</span><span class="sxs-lookup"><span data-stu-id="04b72-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04b72-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04b72-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04b72-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04b72-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="04b72-137">响应</span><span class="sxs-lookup"><span data-stu-id="04b72-137">Response</span></span>
<span data-ttu-id="04b72-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="04b72-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
