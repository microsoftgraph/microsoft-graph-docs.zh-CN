---
title: 列出成员
description: 获取组的直接成员列表。 组可将用户、联系人和其他组作为成员。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6c79b4bd4ee3059e693e63817420e1c5d0b8d612
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279322"
---
# <a name="list-members"></a><span data-ttu-id="3d3db-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="3d3db-104">List members</span></span>
<span data-ttu-id="3d3db-p102">获取组的直接成员列表。组可将用户、联系人和其他组作为成员。此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="3d3db-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d3db-108">权限</span><span class="sxs-lookup"><span data-stu-id="3d3db-108">Permissions</span></span>
<span data-ttu-id="3d3db-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d3db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d3db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d3db-111">Permission type</span></span>      | <span data-ttu-id="3d3db-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d3db-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d3db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d3db-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3d3db-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d3db-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="3d3db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d3db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d3db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d3db-116">Not supported.</span></span>    |
|<span data-ttu-id="3d3db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d3db-117">Application</span></span> | <span data-ttu-id="3d3db-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d3db-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d3db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d3db-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d3db-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3d3db-120">Optional query parameters</span></span>
<span data-ttu-id="3d3db-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3d3db-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d3db-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d3db-122">Request headers</span></span>
| <span data-ttu-id="3d3db-123">名称</span><span class="sxs-lookup"><span data-stu-id="3d3db-123">Name</span></span>       | <span data-ttu-id="3d3db-124">类型</span><span class="sxs-lookup"><span data-stu-id="3d3db-124">Type</span></span> | <span data-ttu-id="3d3db-125">说明</span><span class="sxs-lookup"><span data-stu-id="3d3db-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d3db-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d3db-126">Authorization</span></span>  | <span data-ttu-id="3d3db-127">string</span><span class="sxs-lookup"><span data-stu-id="3d3db-127">string</span></span>  | <span data-ttu-id="3d3db-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d3db-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d3db-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d3db-130">Request body</span></span>
<span data-ttu-id="3d3db-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d3db-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d3db-132">响应</span><span class="sxs-lookup"><span data-stu-id="3d3db-132">Response</span></span>
<span data-ttu-id="3d3db-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3d3db-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d3db-134">示例</span><span class="sxs-lookup"><span data-stu-id="3d3db-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3d3db-135">请求</span><span class="sxs-lookup"><span data-stu-id="3d3db-135">Request</span></span>
<span data-ttu-id="3d3db-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3d3db-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="3d3db-137">响应</span><span class="sxs-lookup"><span data-stu-id="3d3db-137">Response</span></span>
<span data-ttu-id="3d3db-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3d3db-138">The following is an example of the response.</span></span>
><span data-ttu-id="3d3db-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3d3db-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3d3db-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3d3db-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d3db-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3d3db-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d3db-142">C#</span><span class="sxs-lookup"><span data-stu-id="3d3db-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d3db-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d3db-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d3db-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d3db-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
