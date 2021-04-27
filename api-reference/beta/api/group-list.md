---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Microsoft 365 组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 753aad2f2b8de13986ffb713c4a28a5680216e89
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041321"
---
# <a name="list-groups"></a><span data-ttu-id="0b992-103">列出组</span><span class="sxs-lookup"><span data-stu-id="0b992-103">List groups</span></span>

<span data-ttu-id="0b992-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b992-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b992-105">列出组织中的所有组，包括但不限于 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="0b992-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="0b992-106">此操作在默认情况下仅返回每个组的一部分较常用属性。</span><span class="sxs-lookup"><span data-stu-id="0b992-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="0b992-107">这些 _默认_ 属性将记录在 [属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="0b992-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="0b992-108">若要获取 _非_ 默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="0b992-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="0b992-109">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="0b992-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b992-110">权限</span><span class="sxs-lookup"><span data-stu-id="0b992-110">Permissions</span></span>

<span data-ttu-id="0b992-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b992-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b992-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b992-113">Permission type</span></span> | <span data-ttu-id="0b992-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b992-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="0b992-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b992-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0b992-116">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b992-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="0b992-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b992-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b992-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b992-118">Not supported.</span></span> |
| <span data-ttu-id="0b992-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b992-119">Application</span></span> | <span data-ttu-id="0b992-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b992-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b992-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b992-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b992-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b992-122">Optional query parameters</span></span>

<span data-ttu-id="0b992-123">若要仅列出 Microsoft 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="0b992-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="0b992-124">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="0b992-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="0b992-125">你还可以使用 `$count` 和 `$search` 查询参数来限制响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="0b992-126">`$search` 查询参数仅支持对 **displayName** 和 **说明** 字段进行标记化。</span><span class="sxs-lookup"><span data-stu-id="0b992-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="0b992-127">其他字段默认为 `$filter` 行为。</span><span class="sxs-lookup"><span data-stu-id="0b992-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="0b992-128">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="0b992-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0b992-129">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="0b992-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="0b992-130">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b992-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b992-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b992-131">Request headers</span></span>

| <span data-ttu-id="0b992-132">名称</span><span class="sxs-lookup"><span data-stu-id="0b992-132">Name</span></span> | <span data-ttu-id="0b992-133">说明</span><span class="sxs-lookup"><span data-stu-id="0b992-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0b992-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b992-134">Authorization</span></span>  | <span data-ttu-id="0b992-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b992-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b992-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="0b992-137">ConsistencyLevel</span></span> | <span data-ttu-id="0b992-138">最终。</span><span class="sxs-lookup"><span data-stu-id="0b992-138">eventual.</span></span> <span data-ttu-id="0b992-139">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="0b992-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="0b992-140">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="0b992-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b992-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b992-141">Request body</span></span>

<span data-ttu-id="0b992-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b992-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b992-143">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-143">Response</span></span>

<span data-ttu-id="0b992-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0b992-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="0b992-145">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="0b992-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="0b992-146">示例</span><span class="sxs-lookup"><span data-stu-id="0b992-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="0b992-147">示例 1：获取组列表</span><span class="sxs-lookup"><span data-stu-id="0b992-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-148">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-148">Request</span></span>

<span data-ttu-id="0b992-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b992-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b992-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b992-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="0b992-151">C#</span><span class="sxs-lookup"><span data-stu-id="0b992-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b992-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b992-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b992-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b992-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b992-154">Java</span><span class="sxs-lookup"><span data-stu-id="0b992-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0b992-155">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-155">Response</span></span>

<span data-ttu-id="0b992-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-156">The following is an example of the response.</span></span>
><span data-ttu-id="0b992-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b992-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b992-158">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="0b992-158">All the default properties are returned for each group in an actual call.</span></span>

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

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="0b992-159">示例 2：获取组的筛选列表（包括返回的对象数）</span><span class="sxs-lookup"><span data-stu-id="0b992-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-160">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b992-161">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-161">Response</span></span>

<span data-ttu-id="0b992-162">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b992-162">The following is an example of the response which includes only the requested properties.</span></span>

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

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="0b992-163">示例 3：仅获取组的计数</span><span class="sxs-lookup"><span data-stu-id="0b992-163">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-164">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-164">Request</span></span>

<span data-ttu-id="0b992-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b992-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b992-166">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-166">Response</span></span>

<span data-ttu-id="0b992-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-167">The following is an example of the response.</span></span>

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


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0b992-168">示例 4：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="0b992-168">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-169">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-169">Request</span></span>

<span data-ttu-id="0b992-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b992-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b992-171">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-171">Response</span></span>

<span data-ttu-id="0b992-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-172">The following is an example of the response.</span></span>
><span data-ttu-id="0b992-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b992-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="0b992-174">示例 5：使用 $search 获取显示名称中包含字母“Video”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="0b992-174">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-175">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-175">Request</span></span>

<span data-ttu-id="0b992-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b992-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b992-177">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-177">Response</span></span>

<span data-ttu-id="0b992-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-178">The following is an example of the response.</span></span>
><span data-ttu-id="0b992-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b992-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="0b992-180">示例 6：使用 $search 获取显示名称中包含字母“Video”或其说明中包含字母“prod”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="0b992-180">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-181">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-181">Request</span></span>

<span data-ttu-id="0b992-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b992-182">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0b992-183">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-183">Response</span></span>

<span data-ttu-id="0b992-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-184">The following is an example of the response.</span></span>
><span data-ttu-id="0b992-185">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b992-185">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-7-list-dynamic-groups-filtered-by-enabled-membershipruleprocessingstate"></a><span data-ttu-id="0b992-186">示例 7：列出动态组，按已启用 membershipRuleProcessingState 筛选</span><span class="sxs-lookup"><span data-stu-id="0b992-186">Example 7: List dynamic groups, filtered by enabled membershipRuleProcessingState</span></span>

#### <a name="request"></a><span data-ttu-id="0b992-187">请求</span><span class="sxs-lookup"><span data-stu-id="0b992-187">Request</span></span>

<span data-ttu-id="0b992-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b992-188">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b992-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b992-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_enabled_dynamic_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus&$filter=membershipRuleProcessingState eq 'On'
```
# <a name="c"></a>[<span data-ttu-id="0b992-190">C#</span><span class="sxs-lookup"><span data-stu-id="0b992-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b992-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b992-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b992-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b992-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b992-193">Java</span><span class="sxs-lookup"><span data-stu-id="0b992-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b992-194">响应</span><span class="sxs-lookup"><span data-stu-id="0b992-194">Response</span></span>

<span data-ttu-id="0b992-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b992-195">The following is an example of the response.</span></span>

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


