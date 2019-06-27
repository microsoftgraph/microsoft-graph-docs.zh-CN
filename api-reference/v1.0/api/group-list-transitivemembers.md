---
title: 列表组可传递成员
description: 获取组成员的列表。 组可以将用户、设备和其他组作为成员。 此操作是可传递的, 并且还将返回所有嵌套成员的简单列表。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 30e989817f1b0f7134a242687d49c2ae14024989
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277838"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="c1fa9-105">列表组可传递成员</span><span class="sxs-lookup"><span data-stu-id="c1fa9-105">List group transitive members</span></span>

<span data-ttu-id="c1fa9-106">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-106">Get a list of the group's members.</span></span> <span data-ttu-id="c1fa9-107">组可以将用户、设备和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-107">A group can have users, devices and other groups as members.</span></span> <span data-ttu-id="c1fa9-108">此操作是可传递的, 并且还将返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1fa9-109">权限</span><span class="sxs-lookup"><span data-stu-id="c1fa9-109">Permissions</span></span>

<span data-ttu-id="c1fa9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1fa9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1fa9-112">Permission type</span></span>      | <span data-ttu-id="c1fa9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1fa9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1fa9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1fa9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c1fa9-115">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="c1fa9-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="c1fa9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1fa9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1fa9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-117">Not supported.</span></span>    |
|<span data-ttu-id="c1fa9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1fa9-118">Application</span></span> | <span data-ttu-id="c1fa9-119">Read. All, User. All</span><span class="sxs-lookup"><span data-stu-id="c1fa9-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="c1fa9-120">**注意:** 若要列出隐藏的成员资格组的成员, 则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="c1fa9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1fa9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1fa9-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1fa9-122">Optional query parameters</span></span>

<span data-ttu-id="c1fa9-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1fa9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1fa9-124">Request headers</span></span>

| <span data-ttu-id="c1fa9-125">名称</span><span class="sxs-lookup"><span data-stu-id="c1fa9-125">Name</span></span>       | <span data-ttu-id="c1fa9-126">类型</span><span class="sxs-lookup"><span data-stu-id="c1fa9-126">Type</span></span> | <span data-ttu-id="c1fa9-127">说明</span><span class="sxs-lookup"><span data-stu-id="c1fa9-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1fa9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1fa9-128">Authorization</span></span>  | <span data-ttu-id="c1fa9-129">string</span><span class="sxs-lookup"><span data-stu-id="c1fa9-129">string</span></span>  | <span data-ttu-id="c1fa9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1fa9-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1fa9-132">Request body</span></span>

<span data-ttu-id="c1fa9-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1fa9-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa9-134">Response</span></span>

<span data-ttu-id="c1fa9-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1fa9-136">示例</span><span class="sxs-lookup"><span data-stu-id="c1fa9-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1fa9-137">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa9-137">Request</span></span>

<span data-ttu-id="c1fa9-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="c1fa9-139">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa9-139">Response</span></span>

<span data-ttu-id="c1fa9-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-140">The following is an example of the response.</span></span>
><span data-ttu-id="c1fa9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1fa9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c1fa9-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c1fa9-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c1fa9-144">C#</span><span class="sxs-lookup"><span data-stu-id="c1fa9-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1fa9-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1fa9-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c1fa9-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="c1fa9-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
