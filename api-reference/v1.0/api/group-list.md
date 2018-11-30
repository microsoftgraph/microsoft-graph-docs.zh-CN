---
title: 列出组
description: 列出组织中可用的所有组，包括但不限于 Office 365 组。
ms.openlocfilehash: 15d39db7c3b5c322b90a7d7bbfc29ac4d2e81794
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009779"
---
# <a name="list-groups"></a><span data-ttu-id="3917d-103">列出组</span><span class="sxs-lookup"><span data-stu-id="3917d-103">List groups</span></span>
<span data-ttu-id="3917d-p101">列出组织中所有可用的组，包括但不限于 Office 365 组。返回每个组的[默认属性](../api/group-get.md#default-properties)。</span><span class="sxs-lookup"><span data-stu-id="3917d-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="3917d-106">若要仅列出 Office 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：</span><span class="sxs-lookup"><span data-stu-id="3917d-106">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="3917d-107">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="3917d-107">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

## <a name="permissions"></a><span data-ttu-id="3917d-108">权限</span><span class="sxs-lookup"><span data-stu-id="3917d-108">Permissions</span></span>
<span data-ttu-id="3917d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3917d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3917d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3917d-111">Permission type</span></span>      | <span data-ttu-id="3917d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3917d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3917d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3917d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3917d-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3917d-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3917d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3917d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3917d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3917d-116">Not supported.</span></span>    |
|<span data-ttu-id="3917d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3917d-117">Application</span></span> | <span data-ttu-id="3917d-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3917d-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3917d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3917d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3917d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3917d-120">Optional query parameters</span></span>
<span data-ttu-id="3917d-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3917d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3917d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3917d-122">Request headers</span></span>
| <span data-ttu-id="3917d-123">名称</span><span class="sxs-lookup"><span data-stu-id="3917d-123">Name</span></span>       | <span data-ttu-id="3917d-124">类型</span><span class="sxs-lookup"><span data-stu-id="3917d-124">Type</span></span> | <span data-ttu-id="3917d-125">说明</span><span class="sxs-lookup"><span data-stu-id="3917d-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3917d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3917d-126">Authorization</span></span>  | <span data-ttu-id="3917d-127">string</span><span class="sxs-lookup"><span data-stu-id="3917d-127">string</span></span>  | <span data-ttu-id="3917d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3917d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3917d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3917d-130">Request body</span></span>
<span data-ttu-id="3917d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3917d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3917d-132">响应</span><span class="sxs-lookup"><span data-stu-id="3917d-132">Response</span></span>
<span data-ttu-id="3917d-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3917d-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3917d-134">示例</span><span class="sxs-lookup"><span data-stu-id="3917d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3917d-135">请求</span><span class="sxs-lookup"><span data-stu-id="3917d-135">Request</span></span>
<span data-ttu-id="3917d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3917d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="3917d-137">响应</span><span class="sxs-lookup"><span data-stu-id="3917d-137">Response</span></span>
<span data-ttu-id="3917d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3917d-138">The following is an example of the response.</span></span>

><span data-ttu-id="3917d-139">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3917d-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3917d-140">[默认属性](../api/group-get.md#default-properties)将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3917d-140">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

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
