---
title: 列出组
description: 列出组织中可用的所有组，包括但不限于 Office 365 组。
localization_priority: Priority
ms.openlocfilehash: dd243d1f07b98564bb5aa4751664337c0f0654cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813270"
---
# <a name="list-groups"></a><span data-ttu-id="0e25c-103">列出组</span><span class="sxs-lookup"><span data-stu-id="0e25c-103">List groups</span></span>

> <span data-ttu-id="0e25c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e25c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e25c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e25c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e25c-p102">列出组织中所有可用的组，包括但不限于 Office 365 组。返回每个组的[默认属性](../api/group-get.md#default-properties)。</span><span class="sxs-lookup"><span data-stu-id="0e25c-p102">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="0e25c-108">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="0e25c-108">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="0e25c-109">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="0e25c-109">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="0e25c-110">若要返回包含与许可错误的成员的组，请使用 **$filter**查询参数：</span><span class="sxs-lookup"><span data-stu-id="0e25c-110">To return groups containing members with license errors, use the **$filter** query parameter:</span></span> 

```http 
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true 
```
## <a name="permissions"></a><span data-ttu-id="0e25c-111">权限</span><span class="sxs-lookup"><span data-stu-id="0e25c-111">Permissions</span></span>
<span data-ttu-id="0e25c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e25c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e25c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e25c-114">Permission type</span></span>      | <span data-ttu-id="0e25c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e25c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e25c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e25c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0e25c-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e25c-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e25c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e25c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e25c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e25c-119">Not supported.</span></span>    |
|<span data-ttu-id="0e25c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e25c-120">Application</span></span> | <span data-ttu-id="0e25c-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e25c-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e25c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e25c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e25c-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e25c-123">Optional query parameters</span></span>
<span data-ttu-id="0e25c-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e25c-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e25c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e25c-125">Request headers</span></span>
| <span data-ttu-id="0e25c-126">名称</span><span class="sxs-lookup"><span data-stu-id="0e25c-126">Name</span></span>       | <span data-ttu-id="0e25c-127">类型</span><span class="sxs-lookup"><span data-stu-id="0e25c-127">Type</span></span> | <span data-ttu-id="0e25c-128">说明</span><span class="sxs-lookup"><span data-stu-id="0e25c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e25c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e25c-129">Authorization</span></span>  | <span data-ttu-id="0e25c-130">string</span><span class="sxs-lookup"><span data-stu-id="0e25c-130">string</span></span>  | <span data-ttu-id="0e25c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e25c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e25c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e25c-133">Request body</span></span>
<span data-ttu-id="0e25c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e25c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e25c-135">响应</span><span class="sxs-lookup"><span data-stu-id="0e25c-135">Response</span></span>
<span data-ttu-id="0e25c-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0e25c-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e25c-137">示例</span><span class="sxs-lookup"><span data-stu-id="0e25c-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0e25c-138">请求</span><span class="sxs-lookup"><span data-stu-id="0e25c-138">Request</span></span>
<span data-ttu-id="0e25c-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e25c-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response"></a><span data-ttu-id="0e25c-140">响应</span><span class="sxs-lookup"><span data-stu-id="0e25c-140">Response</span></span>
<span data-ttu-id="0e25c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e25c-141">The following is an example of the response.</span></span>
><span data-ttu-id="0e25c-142">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e25c-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0e25c-143">[默认属性](../api/group-get.md#default-properties)将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0e25c-143">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
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
