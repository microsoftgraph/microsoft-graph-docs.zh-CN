---
title: 列出组成员
description: 获取组的直接成员列表。 组可以将用户、联系人、设备、服务主体和其他组作为成员。 此操作不可传递。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8ffb262c4f841687b7ccf0184db34f39b332a65a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263054"
---
# <a name="list-group-members"></a><span data-ttu-id="f4052-105">列出组成员</span><span class="sxs-lookup"><span data-stu-id="f4052-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4052-106">获取组的直接成员列表。</span><span class="sxs-lookup"><span data-stu-id="f4052-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="f4052-107">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="f4052-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="f4052-108">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="f4052-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4052-109">权限</span><span class="sxs-lookup"><span data-stu-id="f4052-109">Permissions</span></span>

<span data-ttu-id="f4052-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4052-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4052-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4052-112">Permission type</span></span>      | <span data-ttu-id="f4052-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4052-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4052-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4052-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4052-115">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="f4052-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="f4052-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4052-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4052-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4052-117">Not supported.</span></span>    |
|<span data-ttu-id="f4052-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4052-118">Application</span></span> | <span data-ttu-id="f4052-119">Read. All, User. All</span><span class="sxs-lookup"><span data-stu-id="f4052-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="f4052-120">注意: 若要列出隐藏的成员资格组的成员, 则需要使用 Read。隐藏权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="f4052-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="f4052-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4052-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4052-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4052-122">Optional query parameters</span></span>
<span data-ttu-id="f4052-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4052-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4052-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4052-124">Request headers</span></span>
| <span data-ttu-id="f4052-125">名称</span><span class="sxs-lookup"><span data-stu-id="f4052-125">Name</span></span>       | <span data-ttu-id="f4052-126">类型</span><span class="sxs-lookup"><span data-stu-id="f4052-126">Type</span></span> | <span data-ttu-id="f4052-127">说明</span><span class="sxs-lookup"><span data-stu-id="f4052-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f4052-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4052-128">Authorization</span></span>  | <span data-ttu-id="f4052-129">string</span><span class="sxs-lookup"><span data-stu-id="f4052-129">string</span></span>  | <span data-ttu-id="f4052-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4052-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4052-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4052-132">Request body</span></span>
<span data-ttu-id="f4052-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4052-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4052-134">响应</span><span class="sxs-lookup"><span data-stu-id="f4052-134">Response</span></span>
<span data-ttu-id="f4052-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4052-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4052-136">示例</span><span class="sxs-lookup"><span data-stu-id="f4052-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f4052-137">请求</span><span class="sxs-lookup"><span data-stu-id="f4052-137">Request</span></span>
<span data-ttu-id="f4052-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4052-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="f4052-139">响应</span><span class="sxs-lookup"><span data-stu-id="f4052-139">Response</span></span>
<span data-ttu-id="f4052-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4052-140">The following is an example of the response.</span></span>
><span data-ttu-id="f4052-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4052-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f4052-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f4052-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f4052-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f4052-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f4052-144">C#</span><span class="sxs-lookup"><span data-stu-id="f4052-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4052-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4052-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f4052-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="f4052-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
