---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Office 365 组。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5081c5013c1bf7c1a1bfbcff58afe5a83aa67bc9
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726573"
---
# <a name="list-groups"></a><span data-ttu-id="41bbc-103">列出组</span><span class="sxs-lookup"><span data-stu-id="41bbc-103">List groups</span></span>
<span data-ttu-id="41bbc-104">列出组织中所有可用的组，包括但不限于 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="41bbc-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="41bbc-105">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="41bbc-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="41bbc-106">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="41bbc-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="41bbc-107">若要获取_非_默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="41bbc-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="41bbc-108">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="41bbc-108">See an [example](group-get.md#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="41bbc-109">权限</span><span class="sxs-lookup"><span data-stu-id="41bbc-109">Permissions</span></span>
<span data-ttu-id="41bbc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41bbc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41bbc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="41bbc-112">Permission type</span></span>      | <span data-ttu-id="41bbc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41bbc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41bbc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41bbc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="41bbc-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bbc-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="41bbc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41bbc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41bbc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41bbc-117">Not supported.</span></span>    |
|<span data-ttu-id="41bbc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="41bbc-118">Application</span></span> | <span data-ttu-id="41bbc-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bbc-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41bbc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41bbc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41bbc-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41bbc-121">Optional query parameters</span></span>
<span data-ttu-id="41bbc-122">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="41bbc-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="41bbc-123">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="41bbc-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="41bbc-124">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="41bbc-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41bbc-125">请求头</span><span class="sxs-lookup"><span data-stu-id="41bbc-125">Request headers</span></span>
| <span data-ttu-id="41bbc-126">名称</span><span class="sxs-lookup"><span data-stu-id="41bbc-126">Name</span></span>       | <span data-ttu-id="41bbc-127">类型</span><span class="sxs-lookup"><span data-stu-id="41bbc-127">Type</span></span> | <span data-ttu-id="41bbc-128">说明</span><span class="sxs-lookup"><span data-stu-id="41bbc-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41bbc-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="41bbc-129">Authorization</span></span>  | <span data-ttu-id="41bbc-130">string</span><span class="sxs-lookup"><span data-stu-id="41bbc-130">string</span></span>  | <span data-ttu-id="41bbc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41bbc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41bbc-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="41bbc-133">Request body</span></span>
<span data-ttu-id="41bbc-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41bbc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41bbc-135">响应</span><span class="sxs-lookup"><span data-stu-id="41bbc-135">Response</span></span>
<span data-ttu-id="41bbc-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="41bbc-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="41bbc-137">该响应仅包括每个组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="41bbc-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="41bbc-138">示例</span><span class="sxs-lookup"><span data-stu-id="41bbc-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="41bbc-139">请求</span><span class="sxs-lookup"><span data-stu-id="41bbc-139">Request</span></span>
<span data-ttu-id="41bbc-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="41bbc-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="41bbc-141">响应</span><span class="sxs-lookup"><span data-stu-id="41bbc-141">Response</span></span>
<span data-ttu-id="41bbc-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41bbc-142">The following is an example of the response.</span></span>

><span data-ttu-id="41bbc-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="41bbc-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41bbc-144">在实际调用中会返回每个组的所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="41bbc-144">All the default properties are returned for each group in an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
