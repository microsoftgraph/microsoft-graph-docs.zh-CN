---
title: 列出 joinedTeams
description: 获取用户已是直接成员的 Microsoft 团队中的团队。
author: dkershaw10
ms.openlocfilehash: 1fdc3ac9f2f09e31af71cdb4707dd84adf2c74a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343839"
---
# <a name="list-joinedteams"></a><span data-ttu-id="0a736-103">列出 joinedTeams</span><span class="sxs-lookup"><span data-stu-id="0a736-103">List joinedTeams</span></span>

> <span data-ttu-id="0a736-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a736-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a736-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a736-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a736-106">获取用户已是直接成员的 Microsoft 团队中的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="0a736-106">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="0a736-107">权限</span><span class="sxs-lookup"><span data-stu-id="0a736-107">Permissions</span></span>
<span data-ttu-id="0a736-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a736-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a736-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a736-110">Permission type</span></span>      | <span data-ttu-id="0a736-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a736-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a736-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a736-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0a736-113">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a736-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a736-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a736-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a736-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a736-115">Not supported.</span></span>    |
|<span data-ttu-id="0a736-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a736-116">Application</span></span> | <span data-ttu-id="0a736-117">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a736-117">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="0a736-118">目前，使用委派的用户权限此操作仅适用于 me 用户。</span><span class="sxs-lookup"><span data-stu-id="0a736-118">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="0a736-119">应用程序权限，它适用于所有用户通过指定的特定用户 id。（me 别名不支持应用程序权限）有关详细信息，请参阅[已知问题](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview)。</span><span class="sxs-lookup"><span data-stu-id="0a736-119">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="0a736-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a736-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a736-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0a736-121">Optional query parameters</span></span>
<span data-ttu-id="0a736-122">目前不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="0a736-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a736-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a736-123">Request headers</span></span>
| <span data-ttu-id="0a736-124">标头</span><span class="sxs-lookup"><span data-stu-id="0a736-124">Header</span></span>       | <span data-ttu-id="0a736-125">值</span><span class="sxs-lookup"><span data-stu-id="0a736-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a736-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a736-126">Authorization</span></span>  | <span data-ttu-id="0a736-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a736-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a736-129">Accept</span><span class="sxs-lookup"><span data-stu-id="0a736-129">Accept</span></span>  | <span data-ttu-id="0a736-130">application/json</span><span class="sxs-lookup"><span data-stu-id="0a736-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a736-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a736-131">Request body</span></span>
<span data-ttu-id="0a736-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a736-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a736-133">响应</span><span class="sxs-lookup"><span data-stu-id="0a736-133">Response</span></span>

<span data-ttu-id="0a736-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0a736-134">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a736-135">示例</span><span class="sxs-lookup"><span data-stu-id="0a736-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a736-136">请求</span><span class="sxs-lookup"><span data-stu-id="0a736-136">Request</span></span>
<span data-ttu-id="0a736-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a736-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="0a736-138">响应</span><span class="sxs-lookup"><span data-stu-id="0a736-138">Response</span></span>
<span data-ttu-id="0a736-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a736-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0a736-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0a736-142">See also</span></span>
[<span data-ttu-id="0a736-143">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="0a736-143">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
