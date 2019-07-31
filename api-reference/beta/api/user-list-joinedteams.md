---
title: 列出 joinedTeams
description: 获取用户不是其直接成员的 Microsoft Teams 团队。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3124f72b30a9ca82efe7f2583a6afc766bed1718
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931468"
---
# <a name="list-joinedteams"></a><span data-ttu-id="280fc-103">列出 joinedTeams</span><span class="sxs-lookup"><span data-stu-id="280fc-103">List joinedTeams</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="280fc-104">获取用户不是其直接成员的 Microsoft Teams [团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="280fc-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="280fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="280fc-105">Permissions</span></span>
<span data-ttu-id="280fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="280fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="280fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="280fc-108">Permission type</span></span>      | <span data-ttu-id="280fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="280fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="280fc-110">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="280fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="280fc-111">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="280fc-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="280fc-112">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="280fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="280fc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="280fc-113">Not supported.</span></span>    |
|<span data-ttu-id="280fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="280fc-114">Application</span></span> | <span data-ttu-id="280fc-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="280fc-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="280fc-116">目前，使用用户委派的权限时，此操作仅适用于“me”用户。</span><span class="sxs-lookup"><span data-stu-id="280fc-116">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="280fc-117">使用应用程序权限时，此操作通过指定特定用户 ID 而适用于所有用户。（使用应用程序权限时，不支持“me”别名。）有关详细信息，请参阅[已知问题](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview)。</span><span class="sxs-lookup"><span data-stu-id="280fc-117">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="280fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="280fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="280fc-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="280fc-119">Optional query parameters</span></span>
<span data-ttu-id="280fc-120">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="280fc-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="280fc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="280fc-121">Request headers</span></span>
| <span data-ttu-id="280fc-122">标头</span><span class="sxs-lookup"><span data-stu-id="280fc-122">Header</span></span>       | <span data-ttu-id="280fc-123">值</span><span class="sxs-lookup"><span data-stu-id="280fc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="280fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="280fc-124">Authorization</span></span>  | <span data-ttu-id="280fc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="280fc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="280fc-127">接受</span><span class="sxs-lookup"><span data-stu-id="280fc-127">Accept</span></span>  | <span data-ttu-id="280fc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="280fc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="280fc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="280fc-129">Request body</span></span>
<span data-ttu-id="280fc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="280fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="280fc-131">响应</span><span class="sxs-lookup"><span data-stu-id="280fc-131">Response</span></span>

<span data-ttu-id="280fc-132">如果成功，此方法在响应正文中返回`200 OK`响应代码和[team](../resources/team.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="280fc-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/team.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="280fc-133">示例</span><span class="sxs-lookup"><span data-stu-id="280fc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="280fc-134">请求</span><span class="sxs-lookup"><span data-stu-id="280fc-134">Request</span></span>
<span data-ttu-id="280fc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="280fc-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="280fc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="280fc-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="280fc-137">C#</span><span class="sxs-lookup"><span data-stu-id="280fc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="280fc-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="280fc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="280fc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="280fc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="280fc-140">Java</span><span class="sxs-lookup"><span data-stu-id="280fc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-joinedteams-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="280fc-141">响应</span><span class="sxs-lookup"><span data-stu-id="280fc-141">Response</span></span>
<span data-ttu-id="280fc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="280fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="280fc-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="280fc-145">See also</span></span>
[<span data-ttu-id="280fc-146">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="280fc-146">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
