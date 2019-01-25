---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Office 365 组。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4967fd5b84f1329836b6a3e3e5dc7ba7b08ee19a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520618"
---
# <a name="list-groups"></a><span data-ttu-id="b8045-103">列出组</span><span class="sxs-lookup"><span data-stu-id="b8045-103">List groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8045-104">列出组织中所有可用的组，包括但不限于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="b8045-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="b8045-105">此操作在默认情况下仅返回每个组的一部分较常用属性。</span><span class="sxs-lookup"><span data-stu-id="b8045-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="b8045-106">这些_默认_属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="b8045-106">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="b8045-107">若要获取_非_默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="b8045-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="b8045-108">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="b8045-108">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="b8045-109">**hasMembersWithLicenseErrors** 属性是例外。</span><span class="sxs-lookup"><span data-stu-id="b8045-109">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="b8045-110">请参阅关于如何使用此属性的[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="b8045-110">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8045-111">权限</span><span class="sxs-lookup"><span data-stu-id="b8045-111">Permissions</span></span>
<span data-ttu-id="b8045-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8045-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8045-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8045-114">Permission type</span></span>      | <span data-ttu-id="b8045-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8045-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8045-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8045-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b8045-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8045-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8045-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8045-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8045-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8045-119">Not supported.</span></span>    |
|<span data-ttu-id="b8045-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8045-120">Application</span></span> | <span data-ttu-id="b8045-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8045-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8045-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8045-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8045-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b8045-123">Optional query parameters</span></span>

<span data-ttu-id="b8045-124">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="b8045-124">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**: <!-- { "blockType": "ignored" } --></span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="b8045-125">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="b8045-125">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example: <!-- { "blockType": "ignored" } --></span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="b8045-126">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b8045-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8045-127">请求头</span><span class="sxs-lookup"><span data-stu-id="b8045-127">Request headers</span></span>
| <span data-ttu-id="b8045-128">名称</span><span class="sxs-lookup"><span data-stu-id="b8045-128">Name</span></span>       | <span data-ttu-id="b8045-129">类型</span><span class="sxs-lookup"><span data-stu-id="b8045-129">Type</span></span> | <span data-ttu-id="b8045-130">说明</span><span class="sxs-lookup"><span data-stu-id="b8045-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8045-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8045-131">Authorization</span></span>  | <span data-ttu-id="b8045-132">string</span><span class="sxs-lookup"><span data-stu-id="b8045-132">string</span></span>  | <span data-ttu-id="b8045-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8045-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8045-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8045-135">Request body</span></span>
<span data-ttu-id="b8045-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8045-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8045-137">响应</span><span class="sxs-lookup"><span data-stu-id="b8045-137">Response</span></span>
<span data-ttu-id="b8045-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b8045-138">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="b8045-139">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="b8045-139">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="b8045-140">示例</span><span class="sxs-lookup"><span data-stu-id="b8045-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="b8045-141">请求 1</span><span class="sxs-lookup"><span data-stu-id="b8045-141">Request 1</span></span>
<span data-ttu-id="b8045-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8045-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response-1"></a><span data-ttu-id="b8045-143">响应 1</span><span class="sxs-lookup"><span data-stu-id="b8045-143">Response 1</span></span>
<span data-ttu-id="b8045-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b8045-144">The following is an example of the response.</span></span>
><span data-ttu-id="b8045-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8045-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8045-146">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="b8045-146">All the default properties are returned for each group in an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="b8045-147">请求 2</span><span class="sxs-lookup"><span data-stu-id="b8045-147">Request 2</span></span>
<span data-ttu-id="b8045-148">此示例使用 `$filter` 查询选项获取成员在基于组的许可证分配中存在许可证错误的组。</span><span class="sxs-lookup"><span data-stu-id="b8045-148">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="b8045-149">还使用 `$select` 查询选项仅获取响应中每个组的 **id** 和 **displayName** 属性，而非其他默认或非默认属性。</span><span class="sxs-lookup"><span data-stu-id="b8045-149">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="b8045-150">响应 2</span><span class="sxs-lookup"><span data-stu-id="b8045-150">Response 2</span></span>
<span data-ttu-id="b8045-151">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="b8045-151">The following is an example of the response which includes only the requested properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
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
<!--
{
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
