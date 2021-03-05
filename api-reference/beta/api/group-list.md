---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Microsoft 365 组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b2f6170ce88c7f6c570f3bc0774898d0aa6bd256
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471031"
---
# <a name="list-groups"></a><span data-ttu-id="13d62-103">列出组</span><span class="sxs-lookup"><span data-stu-id="13d62-103">List groups</span></span>

<span data-ttu-id="13d62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13d62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13d62-105">列出组织中的所有组，包括但不限于 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="13d62-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="13d62-106">此操作在默认情况下仅返回每个组的一部分较常用属性。</span><span class="sxs-lookup"><span data-stu-id="13d62-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="13d62-107">这些 _默认_ 属性将记录在 [属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="13d62-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="13d62-108">若要获取 _非_ 默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="13d62-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="13d62-109">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="13d62-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="13d62-110">权限</span><span class="sxs-lookup"><span data-stu-id="13d62-110">Permissions</span></span>

<span data-ttu-id="13d62-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13d62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13d62-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="13d62-113">Permission type</span></span> | <span data-ttu-id="13d62-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13d62-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="13d62-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13d62-115">Delegated (work or school account)</span></span> | <span data-ttu-id="13d62-116">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="13d62-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="13d62-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13d62-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13d62-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="13d62-118">Not supported.</span></span> |
| <span data-ttu-id="13d62-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="13d62-119">Application</span></span> | <span data-ttu-id="13d62-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d62-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13d62-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13d62-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13d62-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13d62-122">Optional query parameters</span></span>

<span data-ttu-id="13d62-123">若要仅列出 Microsoft 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="13d62-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="13d62-124">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="13d62-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="13d62-125">你还可以使用 `$count` 和 `$search` 查询参数来限制响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="13d62-126">`$search` 查询参数仅支持对 **displayName** 和 **说明** 字段进行标记化。</span><span class="sxs-lookup"><span data-stu-id="13d62-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="13d62-127">其他字段默认为 `$filter` 行为。</span><span class="sxs-lookup"><span data-stu-id="13d62-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="13d62-128">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="13d62-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="13d62-129">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="13d62-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="13d62-130">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="13d62-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="13d62-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="13d62-131">Request headers</span></span>

| <span data-ttu-id="13d62-132">名称</span><span class="sxs-lookup"><span data-stu-id="13d62-132">Name</span></span> | <span data-ttu-id="13d62-133">说明</span><span class="sxs-lookup"><span data-stu-id="13d62-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="13d62-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="13d62-134">Authorization</span></span>  | <span data-ttu-id="13d62-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13d62-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13d62-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="13d62-137">ConsistencyLevel</span></span> | <span data-ttu-id="13d62-138">最终。</span><span class="sxs-lookup"><span data-stu-id="13d62-138">eventual.</span></span> <span data-ttu-id="13d62-139">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="13d62-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="13d62-140">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="13d62-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13d62-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="13d62-141">Request body</span></span>

<span data-ttu-id="13d62-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13d62-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13d62-143">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-143">Response</span></span>

<span data-ttu-id="13d62-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="13d62-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="13d62-145">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="13d62-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="13d62-146">示例</span><span class="sxs-lookup"><span data-stu-id="13d62-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="13d62-147">示例 1：获取组列表</span><span class="sxs-lookup"><span data-stu-id="13d62-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-148">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-148">Request</span></span>

<span data-ttu-id="13d62-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13d62-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13d62-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="13d62-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="13d62-151">C#</span><span class="sxs-lookup"><span data-stu-id="13d62-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13d62-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13d62-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13d62-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13d62-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13d62-154">Java</span><span class="sxs-lookup"><span data-stu-id="13d62-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="13d62-155">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-155">Response</span></span>

<span data-ttu-id="13d62-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-156">The following is an example of the response.</span></span>
><span data-ttu-id="13d62-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13d62-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13d62-158">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="13d62-158">All the default properties are returned for each group in an actual call.</span></span>

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

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="13d62-159">示例 2：获取组的筛选列表（包括返回的对象数）</span><span class="sxs-lookup"><span data-stu-id="13d62-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-160">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13d62-161">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-161">Response</span></span>

<span data-ttu-id="13d62-162">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="13d62-162">The following is an example of the response which includes only the requested properties.</span></span>

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

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="13d62-163">示例 3：仅获取组的计数</span><span class="sxs-lookup"><span data-stu-id="13d62-163">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-164">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-164">Request</span></span>

<span data-ttu-id="13d62-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13d62-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13d62-166">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-166">Response</span></span>

<span data-ttu-id="13d62-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="13d62-168">893</span><span class="sxs-lookup"><span data-stu-id="13d62-168">893</span></span>


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="13d62-169">示例 4：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="13d62-169">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-170">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-170">Request</span></span>

<span data-ttu-id="13d62-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13d62-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13d62-172">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-172">Response</span></span>

<span data-ttu-id="13d62-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-173">The following is an example of the response.</span></span>
><span data-ttu-id="13d62-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13d62-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="13d62-176">示例 5：使用 $search 获取显示名称中包含字母“Video”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="13d62-176">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-177">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-177">Request</span></span>

<span data-ttu-id="13d62-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13d62-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13d62-179">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-179">Response</span></span>

<span data-ttu-id="13d62-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-180">The following is an example of the response.</span></span>
><span data-ttu-id="13d62-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13d62-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="13d62-183">示例 6：使用 $search 获取显示名称中包含字母“Video”或其说明中包含字母“prod”（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="13d62-183">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-184">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-184">Request</span></span>

<span data-ttu-id="13d62-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13d62-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="13d62-186">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-186">Response</span></span>

<span data-ttu-id="13d62-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-187">The following is an example of the response.</span></span>
><span data-ttu-id="13d62-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13d62-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-7-list-dynamic-groups-filtered-by-enabled-membershipruleprocessingstate"></a><span data-ttu-id="13d62-190">示例 7：列出动态组，按已启用 membershipRuleProcessingState 筛选</span><span class="sxs-lookup"><span data-stu-id="13d62-190">Example 7: List dynamic groups, filtered by enabled membershipRuleProcessingState</span></span>

#### <a name="request"></a><span data-ttu-id="13d62-191">请求</span><span class="sxs-lookup"><span data-stu-id="13d62-191">Request</span></span>

<span data-ttu-id="13d62-192">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13d62-192">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="13d62-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="13d62-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_enabled_dynamic_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus&$filter=membershipRuleProcessingState eq 'On'
```
# <a name="c"></a>[<span data-ttu-id="13d62-194">C#</span><span class="sxs-lookup"><span data-stu-id="13d62-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13d62-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13d62-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13d62-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13d62-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13d62-197">Java</span><span class="sxs-lookup"><span data-stu-id="13d62-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="13d62-198">响应</span><span class="sxs-lookup"><span data-stu-id="13d62-198">Response</span></span>

<span data-ttu-id="13d62-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13d62-199">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus)",
  "value":[
    {
      "id": "1cdf9c18-a7dc-46b1-b47f-094d5656376d",
      "membershipRule": "user.accountEnabled -eq false",
      "membershipRuleProcessingState": "On",
      "membershipRuleProcessingStatus": {
          "status" : "Succeeded",
          "lastMembershipUpdated"  : "2020-09-14T00:00:00Z",
          "errorMessage" : null
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


