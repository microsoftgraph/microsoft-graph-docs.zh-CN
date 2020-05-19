---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Office 365 组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c76c396219963a03a63ed229cd4d41e86153d36f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289600"
---
# <a name="list-groups"></a><span data-ttu-id="6858c-103">列出组</span><span class="sxs-lookup"><span data-stu-id="6858c-103">List groups</span></span>

<span data-ttu-id="6858c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6858c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6858c-105">列出组织中的所有组，包括但不限于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="6858c-105">List all the groups in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="6858c-106">此操作在默认情况下仅返回每个组的一部分较常用属性。</span><span class="sxs-lookup"><span data-stu-id="6858c-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="6858c-107">这些_默认_属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="6858c-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="6858c-108">若要获取_非_默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="6858c-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="6858c-109">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="6858c-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="6858c-110">权限</span><span class="sxs-lookup"><span data-stu-id="6858c-110">Permissions</span></span>

<span data-ttu-id="6858c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6858c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6858c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6858c-113">Permission type</span></span> | <span data-ttu-id="6858c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6858c-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="6858c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6858c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6858c-116">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6858c-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6858c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6858c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6858c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6858c-118">Not supported.</span></span> |
| <span data-ttu-id="6858c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6858c-119">Application</span></span> | <span data-ttu-id="6858c-120">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6858c-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6858c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6858c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6858c-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6858c-122">Optional query parameters</span></span>

<span data-ttu-id="6858c-123">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="6858c-123">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="6858c-124">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="6858c-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="6858c-125">您还可以使用 `$count` 和 `$search` 查询参数来限制响应。</span><span class="sxs-lookup"><span data-stu-id="6858c-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="6858c-126">`$search`查询参数仅支持在**displayName**和**description**字段上进行词汇切分。</span><span class="sxs-lookup"><span data-stu-id="6858c-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="6858c-127">其他字段默认为 `$filter` 行为。</span><span class="sxs-lookup"><span data-stu-id="6858c-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="6858c-128">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="6858c-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6858c-129">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="6858c-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="6858c-130">有关详细信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6858c-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6858c-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="6858c-131">Request headers</span></span>

| <span data-ttu-id="6858c-132">名称</span><span class="sxs-lookup"><span data-stu-id="6858c-132">Name</span></span> | <span data-ttu-id="6858c-133">说明</span><span class="sxs-lookup"><span data-stu-id="6858c-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="6858c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6858c-134">Authorization</span></span>  | <span data-ttu-id="6858c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6858c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6858c-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6858c-137">ConsistencyLevel</span></span> | <span data-ttu-id="6858c-138">仍然.</span><span class="sxs-lookup"><span data-stu-id="6858c-138">eventual.</span></span> <span data-ttu-id="6858c-139">此标头 `$count` 在使用时 `$search` 或在 `$filter` 与查询参数一起使用时是必需的 `$orderby` 。</span><span class="sxs-lookup"><span data-stu-id="6858c-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="6858c-140">它使用的索引可能不是最新的对象更改。</span><span class="sxs-lookup"><span data-stu-id="6858c-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6858c-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="6858c-141">Request body</span></span>

<span data-ttu-id="6858c-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6858c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6858c-143">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-143">Response</span></span>

<span data-ttu-id="6858c-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6858c-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="6858c-145">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="6858c-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="6858c-146">示例</span><span class="sxs-lookup"><span data-stu-id="6858c-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="6858c-147">示例1：获取组列表</span><span class="sxs-lookup"><span data-stu-id="6858c-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="6858c-148">请求</span><span class="sxs-lookup"><span data-stu-id="6858c-148">Request</span></span>

<span data-ttu-id="6858c-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6858c-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6858c-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6858c-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="6858c-151">C#</span><span class="sxs-lookup"><span data-stu-id="6858c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6858c-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6858c-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6858c-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6858c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6858c-154">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-154">Response</span></span>

<span data-ttu-id="6858c-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6858c-155">The following is an example of the response.</span></span>
><span data-ttu-id="6858c-156">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6858c-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6858c-157">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="6858c-157">All the default properties are returned for each group in an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="6858c-158">示例2：获取组的已筛选列表，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="6858c-158">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6858c-159">请求</span><span class="sxs-lookup"><span data-stu-id="6858c-159">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6858c-160">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-160">Response</span></span>

<span data-ttu-id="6858c-161">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="6858c-161">The following is an example of the response which includes only the requested properties.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
  "@odata.count":2,
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "displayName": "Contoso Group 1"
    },
    {
      "id": "22222222-3333-4444-5555-666666666666",
      "displayName": "Contoso Group 2"
    }
  ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="6858c-162">示例3：仅获取组的计数</span><span class="sxs-lookup"><span data-stu-id="6858c-162">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="6858c-163">请求</span><span class="sxs-lookup"><span data-stu-id="6858c-163">Request</span></span>

<span data-ttu-id="6858c-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6858c-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6858c-165">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-165">Response</span></span>

<span data-ttu-id="6858c-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6858c-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="6858c-167">893</span><span class="sxs-lookup"><span data-stu-id="6858c-167">893</span></span>


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6858c-168">示例4：使用 $filter 和 $top 获取一个显示名称以 ' a ' 开头的组，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="6858c-168">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6858c-169">请求</span><span class="sxs-lookup"><span data-stu-id="6858c-169">Request</span></span>

<span data-ttu-id="6858c-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6858c-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6858c-171">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-171">Response</span></span>

<span data-ttu-id="6858c-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6858c-172">The following is an example of the response.</span></span>
><span data-ttu-id="6858c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6858c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mailNickname":"a241"
    }
  ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="6858c-175">示例5：使用 $search 获取显示名称包含字母 "Video" 的组，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="6858c-175">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6858c-176">请求</span><span class="sxs-lookup"><span data-stu-id="6858c-176">Request</span></span>

<span data-ttu-id="6858c-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6858c-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6858c-178">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-178">Response</span></span>

<span data-ttu-id="6858c-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6858c-179">The following is an example of the response.</span></span>
><span data-ttu-id="6858c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6858c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="6858c-182">示例6：使用 $search 获取显示名称中包含字母 "Video" 的组或包含字母 "生产" 的说明，包括所返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="6858c-182">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6858c-183">请求</span><span class="sxs-lookup"><span data-stu-id="6858c-183">Request</span></span>

<span data-ttu-id="6858c-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6858c-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6858c-185">响应</span><span class="sxs-lookup"><span data-stu-id="6858c-185">Response</span></span>

<span data-ttu-id="6858c-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6858c-186">The following is an example of the response.</span></span>
><span data-ttu-id="6858c-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6858c-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    },
    {
      "description":"Video Production",
      "displayName":"Video Production",
      "mail":"videoprod@service.contoso.com",
      "mailNickname":"VideoProduction"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
