---
title: 列出频道
description: 检索此团队中的频道列表。
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 67079a369f666ab3b689a7a80f51ee58f437bedc
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275684"
---
# <a name="list-channels"></a><span data-ttu-id="b44ae-103">列出频道</span><span class="sxs-lookup"><span data-stu-id="b44ae-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b44ae-104">检索此[团队](../resources/team.md)中的[频道](../resources/channel.md)列表。</span><span class="sxs-lookup"><span data-stu-id="b44ae-104">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b44ae-105">权限</span><span class="sxs-lookup"><span data-stu-id="b44ae-105">Permissions</span></span>

<span data-ttu-id="b44ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b44ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b44ae-108">Permission type</span></span>      | <span data-ttu-id="b44ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b44ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b44ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b44ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b44ae-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44ae-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b44ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b44ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b44ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b44ae-113">Not supported.</span></span>    |
|<span data-ttu-id="b44ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b44ae-114">Application</span></span> | <span data-ttu-id="b44ae-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44ae-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="b44ae-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b44ae-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b44ae-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="b44ae-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b44ae-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b44ae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b44ae-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b44ae-119">Optional query parameters</span></span>
<span data-ttu-id="b44ae-120">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b44ae-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b44ae-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b44ae-121">Request headers</span></span>

| <span data-ttu-id="b44ae-122">标头</span><span class="sxs-lookup"><span data-stu-id="b44ae-122">Header</span></span>       | <span data-ttu-id="b44ae-123">值</span><span class="sxs-lookup"><span data-stu-id="b44ae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b44ae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b44ae-124">Authorization</span></span>  | <span data-ttu-id="b44ae-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b44ae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b44ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b44ae-127">Request body</span></span>

<span data-ttu-id="b44ae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b44ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b44ae-129">响应</span><span class="sxs-lookup"><span data-stu-id="b44ae-129">Response</span></span>

<span data-ttu-id="b44ae-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Channel](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b44ae-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b44ae-131">示例</span><span class="sxs-lookup"><span data-stu-id="b44ae-131">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="b44ae-132">示例 1：列出所有频道</span><span class="sxs-lookup"><span data-stu-id="b44ae-132">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="b44ae-133">请求</span><span class="sxs-lookup"><span data-stu-id="b44ae-133">Request</span></span>

<span data-ttu-id="b44ae-134">以下示例显示列出所有频道的请求。</span><span class="sxs-lookup"><span data-stu-id="b44ae-134">The following example shows a request to list all channels.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b44ae-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b44ae-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b44ae-136">C#</span><span class="sxs-lookup"><span data-stu-id="b44ae-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b44ae-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b44ae-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b44ae-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b44ae-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b44ae-139">响应</span><span class="sxs-lookup"><span data-stu-id="b44ae-139">Response</span></span>

<span data-ttu-id="b44ae-140">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="b44ae-140">The following is the response.</span></span>

> <span data-ttu-id="b44ae-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b44ae-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b44ae-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b44ae-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="b44ae-143">示例 2：列出所有私人频道</span><span class="sxs-lookup"><span data-stu-id="b44ae-143">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="b44ae-144">请求</span><span class="sxs-lookup"><span data-stu-id="b44ae-144">Request</span></span>

<span data-ttu-id="b44ae-145">以下示例显示列出所有私人频道的请求。</span><span class="sxs-lookup"><span data-stu-id="b44ae-145">The following example shows a request to list all private channels.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```

#### <a name="response"></a><span data-ttu-id="b44ae-146">响应</span><span class="sxs-lookup"><span data-stu-id="b44ae-146">Response</span></span>

<span data-ttu-id="b44ae-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b44ae-147">The following is an example of the response.</span></span>

> <span data-ttu-id="b44ae-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b44ae-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
