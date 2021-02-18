---
title: List group transitive members
description: 获取组的成员列表。 组可以将用户、设备、组织联系人和其他组作为成员。 此操作是可传递的，并返回简单列表嵌套成员中的一个。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0b428dd011937473d1c860e15b95d11e7171eb92
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272175"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="d19f0-105">List group transitive members</span><span class="sxs-lookup"><span data-stu-id="d19f0-105">List group transitive members</span></span>

<span data-ttu-id="d19f0-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d19f0-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d19f0-107">获取组的成员列表。</span><span class="sxs-lookup"><span data-stu-id="d19f0-107">Get a list of the group's members.</span></span> <span data-ttu-id="d19f0-108">组可以将用户、设备、组织联系人和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="d19f0-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="d19f0-109">此操作是可传递的，并返回简单列表嵌套成员中的一个。</span><span class="sxs-lookup"><span data-stu-id="d19f0-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="d19f0-110">权限</span><span class="sxs-lookup"><span data-stu-id="d19f0-110">Permissions</span></span>

<span data-ttu-id="d19f0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d19f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d19f0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d19f0-113">Permission type</span></span>      | <span data-ttu-id="d19f0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d19f0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d19f0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d19f0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d19f0-116">GroupMember.Read.All、Group.Read.All、GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d19f0-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="d19f0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d19f0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d19f0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d19f0-118">Not supported.</span></span>    |
|<span data-ttu-id="d19f0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d19f0-119">Application</span></span> | <span data-ttu-id="d19f0-120">GroupMember.Read.All、Group.Read.All、GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d19f0-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

><span data-ttu-id="d19f0-121">**注意：** 若要列出隐藏成员资格组的成员，需要 Member.Read.Hidden 权限。</span><span class="sxs-lookup"><span data-stu-id="d19f0-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d19f0-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d19f0-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d19f0-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d19f0-123">Optional query parameters</span></span>

<span data-ttu-id="d19f0-124">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="d19f0-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="d19f0-125">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="d19f0-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="d19f0-126">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="d19f0-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="d19f0-127">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="d19f0-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d19f0-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="d19f0-128">Request headers</span></span>

| <span data-ttu-id="d19f0-129">名称</span><span class="sxs-lookup"><span data-stu-id="d19f0-129">Name</span></span> | <span data-ttu-id="d19f0-130">说明</span><span class="sxs-lookup"><span data-stu-id="d19f0-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="d19f0-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d19f0-131">Authorization</span></span>  | <span data-ttu-id="d19f0-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d19f0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d19f0-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="d19f0-134">ConsistencyLevel</span></span> | <span data-ttu-id="d19f0-135">最终。</span><span class="sxs-lookup"><span data-stu-id="d19f0-135">eventual.</span></span> <span data-ttu-id="d19f0-136">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="d19f0-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="d19f0-137">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="d19f0-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d19f0-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="d19f0-138">Request body</span></span>

<span data-ttu-id="d19f0-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d19f0-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d19f0-140">响应</span><span class="sxs-lookup"><span data-stu-id="d19f0-140">Response</span></span>

<span data-ttu-id="d19f0-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d19f0-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d19f0-142">示例</span><span class="sxs-lookup"><span data-stu-id="d19f0-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="d19f0-143">示例 1：获取组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="d19f0-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="d19f0-144">请求</span><span class="sxs-lookup"><span data-stu-id="d19f0-144">Request</span></span>

<span data-ttu-id="d19f0-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d19f0-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d19f0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d19f0-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="d19f0-147">C#</span><span class="sxs-lookup"><span data-stu-id="d19f0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d19f0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d19f0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d19f0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d19f0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d19f0-150">Java</span><span class="sxs-lookup"><span data-stu-id="d19f0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d19f0-151">响应</span><span class="sxs-lookup"><span data-stu-id="d19f0-151">Response</span></span>

<span data-ttu-id="d19f0-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d19f0-152">The following is an example of the response.</span></span>

><span data-ttu-id="d19f0-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d19f0-153">**Note**: The response object shown here might be shortened for readability.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="d19f0-154">示例 2：仅获取可传递成员身份计数</span><span class="sxs-lookup"><span data-stu-id="d19f0-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="d19f0-155">请求</span><span class="sxs-lookup"><span data-stu-id="d19f0-155">Request</span></span>

<span data-ttu-id="d19f0-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d19f0-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d19f0-157">响应</span><span class="sxs-lookup"><span data-stu-id="d19f0-157">Response</span></span>

<span data-ttu-id="d19f0-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d19f0-158">The following is an example of the response.</span></span>

><span data-ttu-id="d19f0-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d19f0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="d19f0-161">示例 3：使用 OData 转换和$search获取显示名称包含字母"tier"（包括返回对象计数）的组的成员身份</span><span class="sxs-lookup"><span data-stu-id="d19f0-161">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d19f0-162">请求</span><span class="sxs-lookup"><span data-stu-id="d19f0-162">Request</span></span>

<span data-ttu-id="d19f0-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d19f0-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d19f0-164">响应</span><span class="sxs-lookup"><span data-stu-id="d19f0-164">Response</span></span>

<span data-ttu-id="d19f0-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d19f0-165">The following is an example of the response.</span></span>

><span data-ttu-id="d19f0-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d19f0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="d19f0-168">示例 4：使用 OData 转换和$filter获取组的用户成员资格，显示名称以"A"开头（包括返回的对象数）</span><span class="sxs-lookup"><span data-stu-id="d19f0-168">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d19f0-169">请求</span><span class="sxs-lookup"><span data-stu-id="d19f0-169">Request</span></span>

<span data-ttu-id="d19f0-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d19f0-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d19f0-171">响应</span><span class="sxs-lookup"><span data-stu-id="d19f0-171">Response</span></span>

<span data-ttu-id="d19f0-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d19f0-172">The following is an example of the response.</span></span>

><span data-ttu-id="d19f0-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d19f0-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
