---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Microsoft 365 组。
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9b132ea523eee7b9ef51afcbf6199c38a8427b4c
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030892"
---
# <a name="list-groups"></a><span data-ttu-id="9fda7-103">列出组</span><span class="sxs-lookup"><span data-stu-id="9fda7-103">List groups</span></span>

<span data-ttu-id="9fda7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fda7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fda7-105">列出组织中的所有组，包括但不限于 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="9fda7-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="9fda7-106">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="9fda7-106">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="9fda7-107">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="9fda7-107">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="9fda7-108">若要获取 _非_ 默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="9fda7-108">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="9fda7-109">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="9fda7-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fda7-110">权限</span><span class="sxs-lookup"><span data-stu-id="9fda7-110">Permissions</span></span>
<span data-ttu-id="9fda7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fda7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fda7-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fda7-113">Permission type</span></span>      | <span data-ttu-id="9fda7-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fda7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fda7-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fda7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9fda7-116">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fda7-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9fda7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fda7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fda7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fda7-118">Not supported.</span></span>    |
|<span data-ttu-id="9fda7-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fda7-119">Application</span></span> | <span data-ttu-id="9fda7-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fda7-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fda7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fda7-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9fda7-122">Optional query parameters</span></span>
<span data-ttu-id="9fda7-123">若要仅列出 Microsoft 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="9fda7-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="9fda7-124">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="9fda7-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="9fda7-125">你还可以使用 `$count` 和 `$search` 查询参数来限制响应。</span><span class="sxs-lookup"><span data-stu-id="9fda7-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="9fda7-126">`$search` 查询参数仅支持对 **displayName** 和 **说明** 字段进行标记化。</span><span class="sxs-lookup"><span data-stu-id="9fda7-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="9fda7-127">其他字段默认为 `$filter` 行为。</span><span class="sxs-lookup"><span data-stu-id="9fda7-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="9fda7-128">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="9fda7-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9fda7-129">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="9fda7-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="9fda7-130">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9fda7-130">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fda7-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fda7-131">Request headers</span></span>

| <span data-ttu-id="9fda7-132">名称</span><span class="sxs-lookup"><span data-stu-id="9fda7-132">Name</span></span> | <span data-ttu-id="9fda7-133">说明</span><span class="sxs-lookup"><span data-stu-id="9fda7-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="9fda7-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fda7-134">Authorization</span></span>  | <span data-ttu-id="9fda7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fda7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fda7-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9fda7-137">ConsistencyLevel</span></span> | <span data-ttu-id="9fda7-138">最终。</span><span class="sxs-lookup"><span data-stu-id="9fda7-138">eventual.</span></span> <span data-ttu-id="9fda7-139">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="9fda7-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="9fda7-140">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="9fda7-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fda7-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fda7-141">Request body</span></span>
<span data-ttu-id="9fda7-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fda7-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fda7-143">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-143">Response</span></span>
<span data-ttu-id="9fda7-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9fda7-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="9fda7-145">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="9fda7-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="9fda7-146">示例</span><span class="sxs-lookup"><span data-stu-id="9fda7-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="9fda7-147">示例 1：获取组列表</span><span class="sxs-lookup"><span data-stu-id="9fda7-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="9fda7-148">请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-148">Request</span></span>

<span data-ttu-id="9fda7-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fda7-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9fda7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fda7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```
# <a name="c"></a>[<span data-ttu-id="9fda7-151">C#</span><span class="sxs-lookup"><span data-stu-id="9fda7-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fda7-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fda7-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fda7-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fda7-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fda7-154">Java</span><span class="sxs-lookup"><span data-stu-id="9fda7-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fda7-155">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-155">Response</span></span>

<span data-ttu-id="9fda7-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9fda7-156">The following is an example of the response.</span></span>

><span data-ttu-id="9fda7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="9fda7-p107">**Note:** The response object shown here might be shortened for readability. All the default properties are returned for each group in an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T02:21:05Z",
      "description": "Self help community for golf",
      "displayName": "Golf Assist",
      "expirationDateTime": null,
      "groupTypes": [
        "Unified"
      ],
      "isAssignableToRole": null,
      "mail": "golfassist@contoso.com",
      "mailEnabled": true,
      "mailNickname": "golfassist",
      "membershipRule": null,
      "membershipRuleProcessingState": null,
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "preferredLanguage": null,
      "proxyAddresses": [
        "smtp:golfassist@contoso.onmicrosoft.com",
        "SMTP:golfassist@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T02:21:05Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "theme": null,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
    },
    {
      "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-11-19T20:29:40Z",
      "description": "Talk about golf",
      "displayName": "Golf Discussion",
      "expirationDateTime": null,
      "groupTypes": [],
      "isAssignableToRole": null,
      "mail": "golftalk@contoso.com",
      "mailEnabled": true,
      "mailNickname": "golftalk",
      "membershipRule": null,
      "membershipRuleProcessingState": null,
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "preferredLanguage": null,
      "proxyAddresses": [
        "smtp:golftalk@contoso.onmicrosoft.com",
        "SMTP:golftalk@contoso.com"
      ],
      "renewedDateTime": "2018-11-19T20:29:40Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "theme": null,
      "visibility": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="9fda7-159">示例 2：获取组的筛选列表（包括返回的对象数）</span><span class="sxs-lookup"><span data-stu-id="9fda7-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

<span data-ttu-id="9fda7-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fda7-160">The following is an example of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="9fda7-161">请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-161">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9fda7-162">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-162">Response</span></span>

<span data-ttu-id="9fda7-163">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="9fda7-163">The following is an example of the response which includes only the requested properties.</span></span>

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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
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

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="9fda7-164">示例 3：仅获取组的计数</span><span class="sxs-lookup"><span data-stu-id="9fda7-164">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="9fda7-165">请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-165">Request</span></span>

<span data-ttu-id="9fda7-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fda7-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
  }-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9fda7-167">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-167">Response</span></span>

<span data-ttu-id="9fda7-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9fda7-168">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9fda7-169">示例 4：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="9fda7-169">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9fda7-170">请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-170">Request</span></span>

<span data-ttu-id="9fda7-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fda7-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9fda7-172">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-172">Response</span></span>

<span data-ttu-id="9fda7-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9fda7-173">The following is an example of the response.</span></span>

><span data-ttu-id="9fda7-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9fda7-174">**Note:** The response object shown here might be shortened for readability.</span></span>

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
   "@odata.count":1,
   "value":[
      {
         "displayName":"a",
         "mailNickname":"a241"
      }
   ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="9fda7-175">示例 5：使用 $search 获取显示名称中包含字母“Video”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="9fda7-175">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9fda7-176">请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-176">Request</span></span>

<span data-ttu-id="9fda7-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fda7-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9fda7-178">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-178">Response</span></span>

<span data-ttu-id="9fda7-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9fda7-179">The following is an example of the response.</span></span>

><span data-ttu-id="9fda7-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9fda7-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="9fda7-181">示例 6：使用 $search 获取显示名称中包含字母“Video”或其说明中包含字母“prod”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="9fda7-181">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9fda7-182">请求</span><span class="sxs-lookup"><span data-stu-id="9fda7-182">Request</span></span>

<span data-ttu-id="9fda7-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fda7-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9fda7-184">响应</span><span class="sxs-lookup"><span data-stu-id="9fda7-184">Response</span></span>

<span data-ttu-id="9fda7-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9fda7-185">The following is an example of the response.</span></span>

><span data-ttu-id="9fda7-186">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9fda7-186">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

