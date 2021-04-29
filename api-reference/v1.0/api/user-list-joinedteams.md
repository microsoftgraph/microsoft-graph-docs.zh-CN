---
title: 列出 joinedTeams
description: 获取用户不是其直接成员的 Microsoft Teams 团队。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ac69603a83a1b02d9fdd8f06aa0be0a7f7abdb20
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051205"
---
# <a name="list-joinedteams"></a><span data-ttu-id="f81c0-103">列出 joinedTeams</span><span class="sxs-lookup"><span data-stu-id="f81c0-103">List joinedTeams</span></span>

<span data-ttu-id="f81c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f81c0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f81c0-105">获取用户不是其直接成员的 Microsoft Teams [团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="f81c0-105">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="f81c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="f81c0-106">Permissions</span></span>
<span data-ttu-id="f81c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f81c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f81c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f81c0-109">Permission type</span></span>      | <span data-ttu-id="f81c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f81c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f81c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f81c0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f81c0-112">Team.ReadBasic.All、 TeamSettings.Read.All、 TeamSettings.ReadWrite.All、 User.Read.All、 User.ReadWrite.All、 Directory.Read.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81c0-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f81c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f81c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f81c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f81c0-114">Not supported.</span></span>    |
|<span data-ttu-id="f81c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f81c0-115">Application</span></span> | <span data-ttu-id="f81c0-116">Team.ReadBasic.All、 TeamSettings.Read.All、 TeamSettings.ReadWrite.All、 User.Read.All、 User.ReadWrite.All、 Directory.Read.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81c0-116">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f81c0-117">使用用户委派的权限时，此操作仅适用于“me”用户。</span><span class="sxs-lookup"><span data-stu-id="f81c0-117">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="f81c0-118">使用应用程序权限时，此操作通过指定特定用户 ID 而适用于所有用户。（使用应用程序权限时，不支持“me”别名）</span><span class="sxs-lookup"><span data-stu-id="f81c0-118">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="f81c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f81c0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f81c0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f81c0-120">Optional query parameters</span></span>
<span data-ttu-id="f81c0-121">目前不支持 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f81c0-121">The [OData Query Parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f81c0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f81c0-122">Request headers</span></span>
| <span data-ttu-id="f81c0-123">标头</span><span class="sxs-lookup"><span data-stu-id="f81c0-123">Header</span></span>       | <span data-ttu-id="f81c0-124">值</span><span class="sxs-lookup"><span data-stu-id="f81c0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f81c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f81c0-125">Authorization</span></span>  | <span data-ttu-id="f81c0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f81c0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f81c0-128">接受</span><span class="sxs-lookup"><span data-stu-id="f81c0-128">Accept</span></span>  | <span data-ttu-id="f81c0-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f81c0-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f81c0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f81c0-130">Request body</span></span>
<span data-ttu-id="f81c0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f81c0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f81c0-132">响应</span><span class="sxs-lookup"><span data-stu-id="f81c0-132">Response</span></span>

<span data-ttu-id="f81c0-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f81c0-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f81c0-134">示例</span><span class="sxs-lookup"><span data-stu-id="f81c0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f81c0-135">请求</span><span class="sxs-lookup"><span data-stu-id="f81c0-135">Request</span></span>
<span data-ttu-id="f81c0-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f81c0-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f81c0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f81c0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
# <a name="c"></a>[<span data-ttu-id="f81c0-138">C#</span><span class="sxs-lookup"><span data-stu-id="f81c0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f81c0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f81c0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f81c0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f81c0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f81c0-141">Java</span><span class="sxs-lookup"><span data-stu-id="f81c0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-joinedteams-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f81c0-142">响应</span><span class="sxs-lookup"><span data-stu-id="f81c0-142">Response</span></span>
<span data-ttu-id="f81c0-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f81c0-143">Here is an example of the response.</span></span> <span data-ttu-id="f81c0-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f81c0-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "31aa74dd-dd65-43ac-8c4e-0ec1ae5a8ee1"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="f81c0-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f81c0-145">See also</span></span>
[<span data-ttu-id="f81c0-146">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="f81c0-146">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
