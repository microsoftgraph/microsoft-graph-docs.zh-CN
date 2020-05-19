---
title: 列出组 memberOf
description: 获取组是其直接成员的组和管理单元。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d5371bd0dffe343a844c6ea8a7ac5fec2a6fef1a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289628"
---
# <a name="list-group-memberof"></a><span data-ttu-id="f305c-103">列出组 memberOf</span><span class="sxs-lookup"><span data-stu-id="f305c-103">List group memberOf</span></span>

<span data-ttu-id="f305c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f305c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f305c-105">获取组是其直接成员的组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="f305c-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="f305c-p101">此操作不可传递。与获取用户的 Office 365 组不同，这将返回所有类型的组，而不只是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="f305c-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f305c-108">权限</span><span class="sxs-lookup"><span data-stu-id="f305c-108">Permissions</span></span>

<span data-ttu-id="f305c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f305c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f305c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f305c-111">Permission type</span></span> | <span data-ttu-id="f305c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f305c-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f305c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f305c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f305c-114">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f305c-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="f305c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f305c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f305c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f305c-116">Not supported.</span></span> |
| <span data-ttu-id="f305c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f305c-117">Application</span></span> | <span data-ttu-id="f305c-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f305c-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f305c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f305c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f305c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f305c-120">Optional query parameters</span></span>

<span data-ttu-id="f305c-121">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="f305c-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="f305c-122">此外，还启用了 OData 强制转换，例如，您可以强制转换以仅获取该组所属的组。</span><span class="sxs-lookup"><span data-stu-id="f305c-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="f305c-123">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="f305c-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="f305c-124">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="f305c-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="f305c-125">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="f305c-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f305c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f305c-126">Request headers</span></span>

| <span data-ttu-id="f305c-127">名称</span><span class="sxs-lookup"><span data-stu-id="f305c-127">Name</span></span> | <span data-ttu-id="f305c-128">说明</span><span class="sxs-lookup"><span data-stu-id="f305c-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f305c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f305c-129">Authorization</span></span>  | <span data-ttu-id="f305c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f305c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f305c-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f305c-132">ConsistencyLevel</span></span> | <span data-ttu-id="f305c-133">仍然.</span><span class="sxs-lookup"><span data-stu-id="f305c-133">eventual.</span></span> <span data-ttu-id="f305c-134">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="f305c-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="f305c-135">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="f305c-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f305c-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="f305c-136">Request body</span></span>

<span data-ttu-id="f305c-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f305c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f305c-138">响应</span><span class="sxs-lookup"><span data-stu-id="f305c-138">Response</span></span>

<span data-ttu-id="f305c-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f305c-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f305c-140">示例</span><span class="sxs-lookup"><span data-stu-id="f305c-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="f305c-141">示例1：获取组是组的直接成员的组和管理单元</span><span class="sxs-lookup"><span data-stu-id="f305c-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="f305c-142">请求</span><span class="sxs-lookup"><span data-stu-id="f305c-142">Request</span></span>

<span data-ttu-id="f305c-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f305c-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f305c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f305c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="f305c-145">C#</span><span class="sxs-lookup"><span data-stu-id="f305c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f305c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f305c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f305c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f305c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f305c-148">响应</span><span class="sxs-lookup"><span data-stu-id="f305c-148">Response</span></span>

<span data-ttu-id="f305c-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f305c-149">The following is an example of the response.</span></span>
><span data-ttu-id="f305c-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f305c-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f305c-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f305c-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="f305c-152">示例2：仅获取所有成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="f305c-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="f305c-153">请求</span><span class="sxs-lookup"><span data-stu-id="f305c-153">Request</span></span>

<span data-ttu-id="f305c-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f305c-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f305c-155">响应</span><span class="sxs-lookup"><span data-stu-id="f305c-155">Response</span></span>

<span data-ttu-id="f305c-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f305c-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="f305c-157">394</span><span class="sxs-lookup"><span data-stu-id="f305c-157">394</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="f305c-158">示例3：使用 OData 强制转换仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="f305c-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="f305c-159">请求</span><span class="sxs-lookup"><span data-stu-id="f305c-159">Request</span></span>

<span data-ttu-id="f305c-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f305c-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f305c-161">响应</span><span class="sxs-lookup"><span data-stu-id="f305c-161">Response</span></span>

<span data-ttu-id="f305c-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f305c-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="f305c-163">394</span><span class="sxs-lookup"><span data-stu-id="f305c-163">394</span></span>

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="f305c-164">示例4：使用 OData 强制转换和 $search 获取显示名称包含字母 "Video" 的成员资格，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="f305c-164">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f305c-165">请求</span><span class="sxs-lookup"><span data-stu-id="f305c-165">Request</span></span>

<span data-ttu-id="f305c-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f305c-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f305c-167">响应</span><span class="sxs-lookup"><span data-stu-id="f305c-167">Response</span></span>

<span data-ttu-id="f305c-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f305c-168">The following is an example of the response.</span></span>
><span data-ttu-id="f305c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f305c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f305c-171">示例5：使用 OData 强制转换和 $filter 获取显示名称以字母 "A" 开头的成员，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="f305c-171">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f305c-172">请求</span><span class="sxs-lookup"><span data-stu-id="f305c-172">Request</span></span>

<span data-ttu-id="f305c-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f305c-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f305c-174">响应</span><span class="sxs-lookup"><span data-stu-id="f305c-174">Response</span></span>

<span data-ttu-id="f305c-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f305c-175">The following is an example of the response.</span></span>
><span data-ttu-id="f305c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f305c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
