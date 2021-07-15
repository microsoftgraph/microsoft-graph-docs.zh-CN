---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Microsoft 365 组。
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 89eee306f2153186d7aaf52f9fc796f2bba24c45
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430075"
---
# <a name="list-groups"></a><span data-ttu-id="84cc7-103">列出组</span><span class="sxs-lookup"><span data-stu-id="84cc7-103">List groups</span></span>

<span data-ttu-id="84cc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84cc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84cc7-105">列出组织中的所有组，包括但不限于 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="84cc7-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="84cc7-106">此操作在默认情况下仅返回每个组的一部分较常用属性。</span><span class="sxs-lookup"><span data-stu-id="84cc7-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="84cc7-107">这些 _默认_ 属性将记录在 [属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="84cc7-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="84cc7-108">若要获取 _非_ 默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="84cc7-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="84cc7-109">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="84cc7-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="84cc7-110">权限</span><span class="sxs-lookup"><span data-stu-id="84cc7-110">Permissions</span></span>

<span data-ttu-id="84cc7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84cc7-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="84cc7-113">Permission type</span></span> | <span data-ttu-id="84cc7-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84cc7-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="84cc7-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84cc7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="84cc7-116">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84cc7-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="84cc7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84cc7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84cc7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="84cc7-118">Not supported.</span></span> |
| <span data-ttu-id="84cc7-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="84cc7-119">Application</span></span> | <span data-ttu-id="84cc7-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84cc7-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84cc7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84cc7-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="84cc7-122">Optional query parameters</span></span>

<span data-ttu-id="84cc7-123">此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-123">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="84cc7-124">只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。</span><span class="sxs-lookup"><span data-stu-id="84cc7-124">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="84cc7-125">有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-125">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<span data-ttu-id="84cc7-126">若要仅列出 Microsoft 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="84cc7-126">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="84cc7-127">`$search`查询参数仅支持对 **displayName** 和 **说明** 字段进行标记化，并且需要 **ConsistencyLevel** 标头。</span><span class="sxs-lookup"><span data-stu-id="84cc7-127">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields and requires the **ConsistencyLevel** header.</span></span> <span data-ttu-id="84cc7-128">**displayName** 和 **说明以外的字段** 默认为`$filter``startswith`行为。</span><span class="sxs-lookup"><span data-stu-id="84cc7-128">Fields other than **displayName** and **description** default to `$filter` `startswith` behavior.</span></span>

<span data-ttu-id="84cc7-129">有关 OData 查询选项的详细信息，请参阅 [ OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-129">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="84cc7-130">有关使用 **ConsistencyLevel** 和`$count`的详细信息，请参阅 [ Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-130">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="84cc7-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="84cc7-131">Request headers</span></span>

| <span data-ttu-id="84cc7-132">名称</span><span class="sxs-lookup"><span data-stu-id="84cc7-132">Name</span></span> | <span data-ttu-id="84cc7-133">说明</span><span class="sxs-lookup"><span data-stu-id="84cc7-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="84cc7-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="84cc7-134">Authorization</span></span>  | <span data-ttu-id="84cc7-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84cc7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84cc7-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="84cc7-137">ConsistencyLevel</span></span> | <span data-ttu-id="84cc7-138">最终。</span><span class="sxs-lookup"><span data-stu-id="84cc7-138">eventual.</span></span> <span data-ttu-id="84cc7-139">当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。</span><span class="sxs-lookup"><span data-stu-id="84cc7-139">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="84cc7-140">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-140">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="84cc7-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="84cc7-141">Request body</span></span>

<span data-ttu-id="84cc7-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84cc7-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84cc7-143">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-143">Response</span></span>

<span data-ttu-id="84cc7-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="84cc7-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="84cc7-145">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="84cc7-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="84cc7-146">示例</span><span class="sxs-lookup"><span data-stu-id="84cc7-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="84cc7-147">示例 1：获取组列表</span><span class="sxs-lookup"><span data-stu-id="84cc7-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-148">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-148">Request</span></span>

<span data-ttu-id="84cc7-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84cc7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="84cc7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="84cc7-151">C#</span><span class="sxs-lookup"><span data-stu-id="84cc7-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84cc7-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84cc7-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84cc7-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84cc7-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84cc7-154">Java</span><span class="sxs-lookup"><span data-stu-id="84cc7-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="84cc7-155">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-155">Response</span></span>

<span data-ttu-id="84cc7-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-156">The following is an example of the response.</span></span>
><span data-ttu-id="84cc7-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="84cc7-p109">**Note:** The response object shown here might be shortened for readability. All the default properties are returned for each group in an actual call.</span></span>

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
   "value":[
      {
         "id":"45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
         "deletedDateTime":null,
         "classification":null,
         "createdDateTime":"2018-12-22T02:21:05Z",
         "description":"Self help community for golf",
         "displayName":"Golf Assist",
         "expirationDateTime":null,
         "groupTypes":[
            "Unified"
         ],
         "isAssignableToRole":null,
         "mail":"golfassist@contoso.com",
         "mailEnabled":true,
         "mailNickname":"golfassist",
         "membershipRule":null,
         "membershipRuleProcessingState":null,
         "onPremisesLastSyncDateTime":null,
         "onPremisesSecurityIdentifier":null,
         "onPremisesSyncEnabled":null,
         "preferredDataLocation":"CAN",
         "preferredLanguage":null,
         "proxyAddresses":[
            "smtp:golfassist@contoso.onmicrosoft.com",
            "SMTP:golfassist@contoso.com"
         ],
         "renewedDateTime":"2018-12-22T02:21:05Z",
         "resourceBehaviorOptions":[
         ],
         "resourceProvisioningOptions":[
         ],
         "securityEnabled":false,
         "theme":null,
         "visibility":"Public",
         "onPremisesProvisioningErrors":[
         ]
      },
      {
         "id":"d7797254-3084-44d0-99c9-a3b5ab149538",
         "deletedDateTime":null,
         "classification":null,
         "createdDateTime":"2018-11-19T20:29:40Z",
         "description":"Talk about golf",
         "displayName":"Golf Discussion",
         "expirationDateTime":null,
         "groupTypes":[
         ],
         "isAssignableToRole":null,
         "mail":"golftalk@contoso.com",
         "mailEnabled":true,
         "mailNickname":"golftalk",
         "membershipRule":null,
         "membershipRuleProcessingState":null,
         "onPremisesLastSyncDateTime":null,
         "onPremisesSecurityIdentifier":null,
         "onPremisesSyncEnabled":null,
         "preferredDataLocation":"CAN",
         "preferredLanguage":null,
         "proxyAddresses":[
            "smtp:golftalk@contoso.onmicrosoft.com",
            "SMTP:golftalk@contoso.com"
         ],
         "renewedDateTime":"2018-11-19T20:29:40Z",
         "resourceBehaviorOptions":[
         ],
         "resourceProvisioningOptions":[ 
         ],
         "securityEnabled":false,
         "theme":null,
         "visibility":null,
         "onPremisesProvisioningErrors":[
         ]
      }
   ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="84cc7-159">示例 2：获取组的筛选列表（包括返回的对象数）</span><span class="sxs-lookup"><span data-stu-id="84cc7-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-160">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-160">Request</span></span>

<span data-ttu-id="84cc7-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-161">The following is an example of the request.</span></span> <span data-ttu-id="84cc7-162">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="84cc7-162">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="84cc7-163">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-163">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="84cc7-164">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-164">Response</span></span>

<span data-ttu-id="84cc7-165">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="84cc7-165">The following is an example of the response which includes only the requested properties.</span></span>

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
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
   "@odata.count":2,
   "value":[
      {
         "id":"11111111-2222-3333-4444-555555555555",
         "displayName":"Contoso Group 1"
      },
      {
         "id":"22222222-3333-4444-5555-666666666666",
         "displayName":"Contoso Group 2"
      }
   ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="84cc7-166">示例 3：仅获取组的计数</span><span class="sxs-lookup"><span data-stu-id="84cc7-166">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-167">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-167">Request</span></span>

<span data-ttu-id="84cc7-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-168">The following is an example of the request.</span></span> <span data-ttu-id="84cc7-169">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="84cc7-169">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="84cc7-170">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-170">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="84cc7-171">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-171">Response</span></span>

<span data-ttu-id="84cc7-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="84cc7-173">示例 4：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="84cc7-173">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-174">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-174">Request</span></span>

<span data-ttu-id="84cc7-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-175">The following is an example of the request.</span></span> <span data-ttu-id="84cc7-176">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="84cc7-176">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="84cc7-177">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-177">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="84cc7-178">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-178">Response</span></span>

<span data-ttu-id="84cc7-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-179">The following is an example of the response.</span></span>
><span data-ttu-id="84cc7-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84cc7-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="84cc7-181">示例 5：使用 $search 获取显示名称中包含字母“Video”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="84cc7-181">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-182">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-182">Request</span></span>

<span data-ttu-id="84cc7-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-183">The following is an example of the request.</span></span> <span data-ttu-id="84cc7-184">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。</span><span class="sxs-lookup"><span data-stu-id="84cc7-184">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="84cc7-185">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-185">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="84cc7-186">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-186">Response</span></span>

<span data-ttu-id="84cc7-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-187">The following is an example of the response.</span></span>
><span data-ttu-id="84cc7-188">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84cc7-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="84cc7-189">示例 6：使用 $search 获取显示名称中包含字母“Video”或其说明中包含字母“prod”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="84cc7-189">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-190">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-190">Request</span></span>

<span data-ttu-id="84cc7-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-191">The following is an example of the request.</span></span> <span data-ttu-id="84cc7-192">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。</span><span class="sxs-lookup"><span data-stu-id="84cc7-192">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="84cc7-193">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="84cc7-193">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="84cc7-194">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-194">Response</span></span>

<span data-ttu-id="84cc7-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-195">The following is an example of the response.</span></span>
><span data-ttu-id="84cc7-196">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84cc7-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-7-list-dynamic-groups-filtered-by-enabled-membershipruleprocessingstate"></a><span data-ttu-id="84cc7-197">示例 7：列出动态组，按已启用 membershipRuleProcessingState 筛选</span><span class="sxs-lookup"><span data-stu-id="84cc7-197">Example 7: List dynamic groups, filtered by enabled membershipRuleProcessingState</span></span>

#### <a name="request"></a><span data-ttu-id="84cc7-198">请求</span><span class="sxs-lookup"><span data-stu-id="84cc7-198">Request</span></span>

<span data-ttu-id="84cc7-199">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84cc7-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="84cc7-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="84cc7-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_enabled_dynamic_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus&$filter=membershipRuleProcessingState eq 'On'
```
# <a name="c"></a>[<span data-ttu-id="84cc7-201">C#</span><span class="sxs-lookup"><span data-stu-id="84cc7-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84cc7-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84cc7-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84cc7-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84cc7-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84cc7-204">Java</span><span class="sxs-lookup"><span data-stu-id="84cc7-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84cc7-205">响应</span><span class="sxs-lookup"><span data-stu-id="84cc7-205">Response</span></span>

<span data-ttu-id="84cc7-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84cc7-206">The following is an example of the response.</span></span>

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
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus)",
   "value":[
      {
         "id":"1cdf9c18-a7dc-46b1-b47f-094d5656376d",
         "membershipRule":"user.accountEnabled -eq false",
         "membershipRuleProcessingState":"On",
         "membershipRuleProcessingStatus":{
            "status":"Succeeded",
            "lastMembershipUpdated":"2020-09-14T00:00:00Z",
            "errorMessage":null
         }
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


