---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Office 365 组。
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fefccee51195adafb1bb3881b6a39336059d7857
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125139"
---
# <a name="list-groups"></a><span data-ttu-id="9037d-103">列出组</span><span class="sxs-lookup"><span data-stu-id="9037d-103">List groups</span></span>

<span data-ttu-id="9037d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9037d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9037d-105">列出组织中的所有组，包括但不限于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="9037d-105">List all the groups in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="9037d-106">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="9037d-106">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="9037d-107">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="9037d-107">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="9037d-108">若要获取_非_默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="9037d-108">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="9037d-109">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="9037d-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="9037d-110">权限</span><span class="sxs-lookup"><span data-stu-id="9037d-110">Permissions</span></span>
<span data-ttu-id="9037d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9037d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9037d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="9037d-113">Permission type</span></span>      | <span data-ttu-id="9037d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9037d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9037d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9037d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9037d-116">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9037d-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9037d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9037d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9037d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9037d-118">Not supported.</span></span>    |
|<span data-ttu-id="9037d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="9037d-119">Application</span></span> | <span data-ttu-id="9037d-120">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9037d-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9037d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9037d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9037d-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9037d-122">Optional query parameters</span></span>
<span data-ttu-id="9037d-123">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="9037d-123">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="9037d-124">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="9037d-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="9037d-125">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9037d-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9037d-126">请求头</span><span class="sxs-lookup"><span data-stu-id="9037d-126">Request headers</span></span>
| <span data-ttu-id="9037d-127">名称</span><span class="sxs-lookup"><span data-stu-id="9037d-127">Name</span></span>       | <span data-ttu-id="9037d-128">类型</span><span class="sxs-lookup"><span data-stu-id="9037d-128">Type</span></span> | <span data-ttu-id="9037d-129">说明</span><span class="sxs-lookup"><span data-stu-id="9037d-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9037d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9037d-130">Authorization</span></span>  | <span data-ttu-id="9037d-131">string</span><span class="sxs-lookup"><span data-stu-id="9037d-131">string</span></span>  | <span data-ttu-id="9037d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9037d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9037d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="9037d-134">Request body</span></span>
<span data-ttu-id="9037d-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9037d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9037d-136">响应</span><span class="sxs-lookup"><span data-stu-id="9037d-136">Response</span></span>
<span data-ttu-id="9037d-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9037d-137">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="9037d-138">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="9037d-138">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="9037d-139">示例</span><span class="sxs-lookup"><span data-stu-id="9037d-139">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="9037d-140">示例 1：返回组对象列表</span><span class="sxs-lookup"><span data-stu-id="9037d-140">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="9037d-141">请求</span><span class="sxs-lookup"><span data-stu-id="9037d-141">Request</span></span>

<span data-ttu-id="9037d-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9037d-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9037d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9037d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```
# <a name="c"></a>[<span data-ttu-id="9037d-144">C#</span><span class="sxs-lookup"><span data-stu-id="9037d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9037d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9037d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9037d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9037d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9037d-147">Java</span><span class="sxs-lookup"><span data-stu-id="9037d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9037d-148">响应</span><span class="sxs-lookup"><span data-stu-id="9037d-148">Response</span></span>

<span data-ttu-id="9037d-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9037d-149">The following is an example of the response.</span></span>

><span data-ttu-id="9037d-150">**注意：** 为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9037d-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9037d-151">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="9037d-151">All the default properties are returned for each group in an actual call.</span></span>

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


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="9037d-152">示例 2：返回经过筛选的组对象列表</span><span class="sxs-lookup"><span data-stu-id="9037d-152">Example 2: Return a filtered list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="9037d-153">请求</span><span class="sxs-lookup"><span data-stu-id="9037d-153">Request</span></span>

<span data-ttu-id="9037d-154">此示例使用 `$filter` 查询选项获取成员在基于组的许可证分配中存在许可证错误的组。</span><span class="sxs-lookup"><span data-stu-id="9037d-154">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="9037d-155">还使用 `$select` 查询选项仅获取响应中每个组的 **id** 和 **displayName** 属性，而非其他默认或非默认属性。</span><span class="sxs-lookup"><span data-stu-id="9037d-155">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="9037d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="9037d-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="c"></a>[<span data-ttu-id="9037d-157">C#</span><span class="sxs-lookup"><span data-stu-id="9037d-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9037d-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9037d-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9037d-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9037d-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9037d-160">Java</span><span class="sxs-lookup"><span data-stu-id="9037d-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-withlicenseerrors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9037d-161">响应</span><span class="sxs-lookup"><span data-stu-id="9037d-161">Response</span></span>

<span data-ttu-id="9037d-162">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="9037d-162">The following is an example of the response which includes only the requested properties.</span></span>

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
