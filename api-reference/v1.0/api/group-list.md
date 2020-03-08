---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Office 365 组。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c6b9fc09f21dca5b12c4e46101183eb28233d168
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517017"
---
# <a name="list-groups"></a><span data-ttu-id="d262b-103">列出组</span><span class="sxs-lookup"><span data-stu-id="d262b-103">List groups</span></span>

<span data-ttu-id="d262b-104">命名空间：microsoft.graph 列出组织中的所有组，包括但不限于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d262b-104">Namespace: microsoft.graph List all the groups in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="d262b-105">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="d262b-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="d262b-106">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="d262b-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="d262b-107">若要获取_非_默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="d262b-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="d262b-108">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="d262b-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="d262b-109">权限</span><span class="sxs-lookup"><span data-stu-id="d262b-109">Permissions</span></span>
<span data-ttu-id="d262b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d262b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d262b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d262b-112">Permission type</span></span>      | <span data-ttu-id="d262b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d262b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d262b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d262b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d262b-115">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d262b-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d262b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d262b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d262b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d262b-117">Not supported.</span></span>    |
|<span data-ttu-id="d262b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d262b-118">Application</span></span> | <span data-ttu-id="d262b-119">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d262b-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d262b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d262b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d262b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d262b-121">Optional query parameters</span></span>
<span data-ttu-id="d262b-122">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="d262b-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="d262b-123">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="d262b-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="d262b-124">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d262b-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d262b-125">请求头</span><span class="sxs-lookup"><span data-stu-id="d262b-125">Request headers</span></span>
| <span data-ttu-id="d262b-126">名称</span><span class="sxs-lookup"><span data-stu-id="d262b-126">Name</span></span>       | <span data-ttu-id="d262b-127">类型</span><span class="sxs-lookup"><span data-stu-id="d262b-127">Type</span></span> | <span data-ttu-id="d262b-128">说明</span><span class="sxs-lookup"><span data-stu-id="d262b-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d262b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d262b-129">Authorization</span></span>  | <span data-ttu-id="d262b-130">string</span><span class="sxs-lookup"><span data-stu-id="d262b-130">string</span></span>  | <span data-ttu-id="d262b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d262b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d262b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d262b-133">Request body</span></span>
<span data-ttu-id="d262b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d262b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d262b-135">响应</span><span class="sxs-lookup"><span data-stu-id="d262b-135">Response</span></span>
<span data-ttu-id="d262b-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d262b-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="d262b-137">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="d262b-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="d262b-138">示例</span><span class="sxs-lookup"><span data-stu-id="d262b-138">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="d262b-139">示例 1：返回组对象列表</span><span class="sxs-lookup"><span data-stu-id="d262b-139">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="d262b-140">请求</span><span class="sxs-lookup"><span data-stu-id="d262b-140">Request</span></span>

<span data-ttu-id="d262b-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d262b-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d262b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d262b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```
# <a name="c"></a>[<span data-ttu-id="d262b-143">C#</span><span class="sxs-lookup"><span data-stu-id="d262b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d262b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d262b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d262b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d262b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d262b-146">Java</span><span class="sxs-lookup"><span data-stu-id="d262b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d262b-147">响应</span><span class="sxs-lookup"><span data-stu-id="d262b-147">Response</span></span>

<span data-ttu-id="d262b-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d262b-148">The following is an example of the response.</span></span>

><span data-ttu-id="d262b-149">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d262b-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d262b-150">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="d262b-150">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
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
            "creationOptions": [],
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "creationOptions": [],
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="d262b-151">示例 2：返回经过筛选的组对象列表</span><span class="sxs-lookup"><span data-stu-id="d262b-151">Example 2: Return a filtered list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="d262b-152">请求</span><span class="sxs-lookup"><span data-stu-id="d262b-152">Request</span></span>

<span data-ttu-id="d262b-153">此示例使用 `$filter` 查询选项获取成员在基于组的许可证分配中存在许可证错误的组。</span><span class="sxs-lookup"><span data-stu-id="d262b-153">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="d262b-154">还使用 `$select` 查询选项仅获取响应中每个组的 **id** 和 **displayName** 属性，而非其他默认或非默认属性。</span><span class="sxs-lookup"><span data-stu-id="d262b-154">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="d262b-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="d262b-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="c"></a>[<span data-ttu-id="d262b-156">C#</span><span class="sxs-lookup"><span data-stu-id="d262b-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d262b-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d262b-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d262b-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d262b-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d262b-159">Java</span><span class="sxs-lookup"><span data-stu-id="d262b-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-withlicenseerrors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d262b-160">响应</span><span class="sxs-lookup"><span data-stu-id="d262b-160">Response</span></span>

<span data-ttu-id="d262b-161">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="d262b-161">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups_withlicenseerrors"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
    "value": [
        {
            "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
            "displayName": "Library Assist"
        },
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "displayName": "Golf Assist"
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
