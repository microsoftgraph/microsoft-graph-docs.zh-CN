---
title: 列出 joinedTeams
description: 获取用户已是直接成员的 Microsoft 团队中的团队。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 95dfa387a55dd5270035816d144ac3a6ac2b6703
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016700"
---
# <a name="list-joinedteams"></a><span data-ttu-id="569d9-103">列出 joinedTeams</span><span class="sxs-lookup"><span data-stu-id="569d9-103">List joinedTeams</span></span>



<span data-ttu-id="569d9-104">获取用户已是直接成员的 Microsoft 团队中的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="569d9-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="569d9-105">权限</span><span class="sxs-lookup"><span data-stu-id="569d9-105">Permissions</span></span>
<span data-ttu-id="569d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="569d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="569d9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="569d9-108">Permission type</span></span>      | <span data-ttu-id="569d9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="569d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="569d9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="569d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="569d9-111">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569d9-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="569d9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="569d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="569d9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="569d9-113">Not supported.</span></span>    |
|<span data-ttu-id="569d9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="569d9-114">Application</span></span> | <span data-ttu-id="569d9-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569d9-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="569d9-116">用户委派权限与此操作仅适用于 me 用户。</span><span class="sxs-lookup"><span data-stu-id="569d9-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="569d9-117">应用程序权限，它适用于所有用户通过指定的特定用户 id。（me 别名不支持应用程序权限）</span><span class="sxs-lookup"><span data-stu-id="569d9-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="569d9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="569d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="569d9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="569d9-119">Optional query parameters</span></span>
<span data-ttu-id="569d9-120">目前不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="569d9-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="569d9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="569d9-121">Request headers</span></span>
| <span data-ttu-id="569d9-122">标头</span><span class="sxs-lookup"><span data-stu-id="569d9-122">Header</span></span>       | <span data-ttu-id="569d9-123">值</span><span class="sxs-lookup"><span data-stu-id="569d9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="569d9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="569d9-124">Authorization</span></span>  | <span data-ttu-id="569d9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="569d9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="569d9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="569d9-127">Accept</span></span>  | <span data-ttu-id="569d9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="569d9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="569d9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="569d9-129">Request body</span></span>
<span data-ttu-id="569d9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="569d9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="569d9-131">响应</span><span class="sxs-lookup"><span data-stu-id="569d9-131">Response</span></span>

<span data-ttu-id="569d9-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="569d9-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="569d9-133">示例</span><span class="sxs-lookup"><span data-stu-id="569d9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="569d9-134">请求</span><span class="sxs-lookup"><span data-stu-id="569d9-134">Request</span></span>
<span data-ttu-id="569d9-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="569d9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="569d9-136">响应</span><span class="sxs-lookup"><span data-stu-id="569d9-136">Response</span></span>
<span data-ttu-id="569d9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="569d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="569d9-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="569d9-140">See also</span></span>
[<span data-ttu-id="569d9-141">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="569d9-141">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
