---
title: 列出 memberOf
description: '获取直接成员组构成的组集合。 '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e26119bdd6430a7e8ad0af35593248b7bcf6289
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082244"
---
# <a name="list-memberof"></a><span data-ttu-id="ed8f1-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="ed8f1-103">List memberOf</span></span>

<span data-ttu-id="ed8f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed8f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed8f1-105">获取直接成员组构成的组集合。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="ed8f1-p101">此操作不可传递。与获取用户的 Microsoft 365 组不同，该操作将返回所有类型的组，而不仅是 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed8f1-108">权限</span><span class="sxs-lookup"><span data-stu-id="ed8f1-108">Permissions</span></span>
<span data-ttu-id="ed8f1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed8f1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed8f1-111">Permission type</span></span>      | <span data-ttu-id="ed8f1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed8f1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed8f1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed8f1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ed8f1-114">GroupMember.Read.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8f1-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="ed8f1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed8f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed8f1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-116">Not supported.</span></span>    |
|<span data-ttu-id="ed8f1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed8f1-117">Application</span></span> | <span data-ttu-id="ed8f1-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8f1-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ed8f1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed8f1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed8f1-120">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="ed8f1-120">Optional query parameters</span></span>

<span data-ttu-id="ed8f1-p103">此方法支持使用 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。此外还将启用 OData 强制转换，例如，你可以强制转换以获取组所属的组。你可以在 **displayName** 和 **description** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p103">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`. OData cast is also enabled, for example, you can cast to get just the groups the group is a member of. You can use `$search` on the **displayName** and **description** properties. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed8f1-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed8f1-126">Request headers</span></span>

| <span data-ttu-id="ed8f1-127">名称</span><span class="sxs-lookup"><span data-stu-id="ed8f1-127">Name</span></span> | <span data-ttu-id="ed8f1-128">说明</span><span class="sxs-lookup"><span data-stu-id="ed8f1-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ed8f1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed8f1-129">Authorization</span></span>  | <span data-ttu-id="ed8f1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed8f1-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="ed8f1-132">ConsistencyLevel</span></span> | <span data-ttu-id="ed8f1-p105">最终。使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p105">eventual. This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters. It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed8f1-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed8f1-136">Request body</span></span>
<span data-ttu-id="ed8f1-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed8f1-138">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f1-138">Response</span></span>
<span data-ttu-id="ed8f1-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed8f1-140">示例</span><span class="sxs-lookup"><span data-stu-id="ed8f1-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="ed8f1-141">示例 1：获取组是其直接成员的组和管理单元</span><span class="sxs-lookup"><span data-stu-id="ed8f1-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="ed8f1-142">请求</span><span class="sxs-lookup"><span data-stu-id="ed8f1-142">Request</span></span>

<span data-ttu-id="ed8f1-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed8f1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed8f1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="ed8f1-145">C#</span><span class="sxs-lookup"><span data-stu-id="ed8f1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed8f1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed8f1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed8f1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed8f1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed8f1-148">Java</span><span class="sxs-lookup"><span data-stu-id="ed8f1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ed8f1-149">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f1-149">Response</span></span>

<span data-ttu-id="ed8f1-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-150">The following is an example of the response.</span></span>

><span data-ttu-id="ed8f1-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="ed8f1-153">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="ed8f1-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="ed8f1-154">请求</span><span class="sxs-lookup"><span data-stu-id="ed8f1-154">Request</span></span>

<span data-ttu-id="ed8f1-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ed8f1-156">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f1-156">Response</span></span>

<span data-ttu-id="ed8f1-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="ed8f1-158">示例 3：使用 OData 强制转换以仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="ed8f1-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="ed8f1-159">请求</span><span class="sxs-lookup"><span data-stu-id="ed8f1-159">Request</span></span>

<span data-ttu-id="ed8f1-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ed8f1-161">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f1-161">Response</span></span>

<span data-ttu-id="ed8f1-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="ed8f1-163">示例 4：使用 OData 强制转换和 $search 来获取显示名称中包含字母“Video”（包括返回的对象数）的成员资格</span><span class="sxs-lookup"><span data-stu-id="ed8f1-163">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ed8f1-164">请求</span><span class="sxs-lookup"><span data-stu-id="ed8f1-164">Request</span></span>

<span data-ttu-id="ed8f1-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ed8f1-166">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f1-166">Response</span></span>

<span data-ttu-id="ed8f1-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-167">The following is an example of the response.</span></span>

><span data-ttu-id="ed8f1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="ed8f1-170">示例 5：使用 $filter 和 OData 强制转换来获取显示名称以“A”开头（包括返回的对象数）的成员资格</span><span class="sxs-lookup"><span data-stu-id="ed8f1-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="ed8f1-171">请求</span><span class="sxs-lookup"><span data-stu-id="ed8f1-171">Request</span></span>

<span data-ttu-id="ed8f1-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="ed8f1-173">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f1-173">Response</span></span>

<span data-ttu-id="ed8f1-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-174">The following is an example of the response.</span></span>

><span data-ttu-id="ed8f1-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
