---
title: List group transitive members
description: 获取组成员的列表。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b713b3fcddbe4d3a7e0b1931847f94c0f1f60692
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082046"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="c7b8f-103">List group transitive members</span><span class="sxs-lookup"><span data-stu-id="c7b8f-103">List group transitive members</span></span>

<span data-ttu-id="c7b8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7b8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7b8f-105">获取组成员的列表。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-105">Get a list of the group's members.</span></span> <span data-ttu-id="c7b8f-106">组可以将用户、联系人、设备、服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="c7b8f-107">此操作是可传递的，并且还将返回所有嵌套成员的简单列表。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7b8f-108">权限</span><span class="sxs-lookup"><span data-stu-id="c7b8f-108">Permissions</span></span>

<span data-ttu-id="c7b8f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7b8f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7b8f-111">Permission type</span></span> | <span data-ttu-id="c7b8f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7b8f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="c7b8f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b8f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c7b8f-114">Directory.accessasuser.all、User.readbasic.all、用户、全部、用户、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="c7b8f-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
| <span data-ttu-id="c7b8f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b8f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7b8f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-116">Not supported.</span></span> |
| <span data-ttu-id="c7b8f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7b8f-117">Application</span></span> | <span data-ttu-id="c7b8f-118">Read. All，User. All</span><span class="sxs-lookup"><span data-stu-id="c7b8f-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="c7b8f-119">**注意：** 若要列出隐藏的成员资格组的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c7b8f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7b8f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7b8f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7b8f-121">Optional query parameters</span></span>

<span data-ttu-id="c7b8f-p103">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p103">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7b8f-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7b8f-126">Request headers</span></span>

| <span data-ttu-id="c7b8f-127">名称</span><span class="sxs-lookup"><span data-stu-id="c7b8f-127">Name</span></span> | <span data-ttu-id="c7b8f-128">说明</span><span class="sxs-lookup"><span data-stu-id="c7b8f-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="c7b8f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7b8f-129">Authorization</span></span>  | <span data-ttu-id="c7b8f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7b8f-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c7b8f-132">ConsistencyLevel</span></span> | <span data-ttu-id="c7b8f-133">最终。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-133">eventual.</span></span> <span data-ttu-id="c7b8f-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c7b8f-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7b8f-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7b8f-136">Request body</span></span>

<span data-ttu-id="c7b8f-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7b8f-138">响应</span><span class="sxs-lookup"><span data-stu-id="c7b8f-138">Response</span></span>

<span data-ttu-id="c7b8f-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7b8f-140">示例</span><span class="sxs-lookup"><span data-stu-id="c7b8f-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="c7b8f-141">示例1：获取组的可传递成员身份</span><span class="sxs-lookup"><span data-stu-id="c7b8f-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="c7b8f-142">请求</span><span class="sxs-lookup"><span data-stu-id="c7b8f-142">Request</span></span>

<span data-ttu-id="c7b8f-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7b8f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7b8f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="c7b8f-145">C#</span><span class="sxs-lookup"><span data-stu-id="c7b8f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7b8f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7b8f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7b8f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7b8f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7b8f-148">Java</span><span class="sxs-lookup"><span data-stu-id="c7b8f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c7b8f-149">响应</span><span class="sxs-lookup"><span data-stu-id="c7b8f-149">Response</span></span>

<span data-ttu-id="c7b8f-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-150">The following is an example of the response.</span></span>

><span data-ttu-id="c7b8f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="c7b8f-153">示例2：仅获取可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="c7b8f-153">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="c7b8f-154">请求</span><span class="sxs-lookup"><span data-stu-id="c7b8f-154">Request</span></span>

<span data-ttu-id="c7b8f-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c7b8f-156">响应</span><span class="sxs-lookup"><span data-stu-id="c7b8f-156">Response</span></span>

<span data-ttu-id="c7b8f-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-157">The following is an example of the response.</span></span>
><span data-ttu-id="c7b8f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="c7b8f-160">893</span><span class="sxs-lookup"><span data-stu-id="c7b8f-160">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="c7b8f-161">示例3：使用 OData 强制转换和 $search 获取包含包含字母 "层" 的组的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="c7b8f-161">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c7b8f-162">请求</span><span class="sxs-lookup"><span data-stu-id="c7b8f-162">Request</span></span>

<span data-ttu-id="c7b8f-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c7b8f-164">响应</span><span class="sxs-lookup"><span data-stu-id="c7b8f-164">Response</span></span>

<span data-ttu-id="c7b8f-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-165">The following is an example of the response.</span></span>
><span data-ttu-id="c7b8f-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c7b8f-168">示例4：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的组中的用户成员，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="c7b8f-168">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c7b8f-169">请求</span><span class="sxs-lookup"><span data-stu-id="c7b8f-169">Request</span></span>

<span data-ttu-id="c7b8f-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c7b8f-171">响应</span><span class="sxs-lookup"><span data-stu-id="c7b8f-171">Response</span></span>

<span data-ttu-id="c7b8f-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-172">The following is an example of the response.</span></span>
><span data-ttu-id="c7b8f-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7b8f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


