---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Office 365 组。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 393381bfe5f21c4d4196251a4055fc65e0771e5c
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726601"
---
# <a name="list-groups"></a><span data-ttu-id="a18ee-103">列出组</span><span class="sxs-lookup"><span data-stu-id="a18ee-103">List groups</span></span>

> <span data-ttu-id="a18ee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a18ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a18ee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a18ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a18ee-106">列出组织中所有可用的组，包括但不限于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="a18ee-106">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="a18ee-107">此操作在默认情况下仅返回每个组的一部分较常用属性。</span><span class="sxs-lookup"><span data-stu-id="a18ee-107">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="a18ee-108">这些_默认_属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="a18ee-108">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="a18ee-109">若要获取_非_默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="a18ee-109">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="a18ee-110">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="a18ee-110">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="a18ee-111">**hasMembersWithLicenseErrors** 属性是例外。</span><span class="sxs-lookup"><span data-stu-id="a18ee-111">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="a18ee-112">请参阅关于如何使用此属性的[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="a18ee-112">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a18ee-113">权限</span><span class="sxs-lookup"><span data-stu-id="a18ee-113">Permissions</span></span>
<span data-ttu-id="a18ee-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a18ee-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18ee-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="a18ee-116">Permission type</span></span>      | <span data-ttu-id="a18ee-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a18ee-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18ee-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a18ee-118">Delegated (work or school account)</span></span> | <span data-ttu-id="a18ee-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18ee-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a18ee-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a18ee-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18ee-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a18ee-121">Not supported.</span></span>    |
|<span data-ttu-id="a18ee-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="a18ee-122">Application</span></span> | <span data-ttu-id="a18ee-123">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18ee-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a18ee-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a18ee-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a18ee-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a18ee-125">Optional query parameters</span></span>

<span data-ttu-id="a18ee-126">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a18ee-126">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="a18ee-127">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a18ee-127">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="a18ee-128">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a18ee-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a18ee-129">请求头</span><span class="sxs-lookup"><span data-stu-id="a18ee-129">Request headers</span></span>
| <span data-ttu-id="a18ee-130">名称</span><span class="sxs-lookup"><span data-stu-id="a18ee-130">Name</span></span>       | <span data-ttu-id="a18ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="a18ee-131">Type</span></span> | <span data-ttu-id="a18ee-132">说明</span><span class="sxs-lookup"><span data-stu-id="a18ee-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a18ee-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="a18ee-133">Authorization</span></span>  | <span data-ttu-id="a18ee-134">string</span><span class="sxs-lookup"><span data-stu-id="a18ee-134">string</span></span>  | <span data-ttu-id="a18ee-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a18ee-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a18ee-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="a18ee-137">Request body</span></span>
<span data-ttu-id="a18ee-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a18ee-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a18ee-139">响应</span><span class="sxs-lookup"><span data-stu-id="a18ee-139">Response</span></span>
<span data-ttu-id="a18ee-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a18ee-140">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="a18ee-141">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="a18ee-141">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="a18ee-142">示例</span><span class="sxs-lookup"><span data-stu-id="a18ee-142">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="a18ee-143">请求 1</span><span class="sxs-lookup"><span data-stu-id="a18ee-143">Request 1</span></span>
<span data-ttu-id="a18ee-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a18ee-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response-1"></a><span data-ttu-id="a18ee-145">响应 1</span><span class="sxs-lookup"><span data-stu-id="a18ee-145">Response 1</span></span>
<span data-ttu-id="a18ee-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a18ee-146">The following is an example of the response.</span></span>
><span data-ttu-id="a18ee-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a18ee-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a18ee-148">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="a18ee-148">All the default properties are returned for each group in an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="a18ee-149">请求 2</span><span class="sxs-lookup"><span data-stu-id="a18ee-149">Request 2</span></span>
<span data-ttu-id="a18ee-150">此示例使用 `$filter` 查询选项获取成员在基于组的许可证分配中存在许可证错误的组。</span><span class="sxs-lookup"><span data-stu-id="a18ee-150">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="a18ee-151">还使用 `$select` 查询选项仅获取响应中每个组的 **id** 和 **displayName** 属性，而非其他默认或非默认属性。</span><span class="sxs-lookup"><span data-stu-id="a18ee-151">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="a18ee-152">响应 2</span><span class="sxs-lookup"><span data-stu-id="a18ee-152">Response 2</span></span>
<span data-ttu-id="a18ee-153">下面是一个仅包括所请求的属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="a18ee-153">The following is an example of the response which includes only the requested properties.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
