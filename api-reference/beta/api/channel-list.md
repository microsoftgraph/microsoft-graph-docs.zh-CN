---
title: 列出频道
description: 检索此团队中的频道列表。
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b96365b6e29e5742ac59d9b202be8c8d2e094db8
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633396"
---
# <a name="list-channels"></a><span data-ttu-id="bd96c-103">列出频道</span><span class="sxs-lookup"><span data-stu-id="bd96c-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd96c-104">检索此[团队](../resources/team.md)中的[频道](../resources/channel.md)列表。</span><span class="sxs-lookup"><span data-stu-id="bd96c-104">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd96c-105">权限</span><span class="sxs-lookup"><span data-stu-id="bd96c-105">Permissions</span></span>

<span data-ttu-id="bd96c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd96c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd96c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd96c-108">Permission type</span></span>      | <span data-ttu-id="bd96c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd96c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd96c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd96c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd96c-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd96c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd96c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd96c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd96c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd96c-113">Not supported.</span></span>    |
|<span data-ttu-id="bd96c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd96c-114">Application</span></span> | <span data-ttu-id="bd96c-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd96c-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="bd96c-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="bd96c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bd96c-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="bd96c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd96c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd96c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd96c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bd96c-119">Optional query parameters</span></span>
<span data-ttu-id="bd96c-120">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd96c-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd96c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd96c-121">Request headers</span></span>

| <span data-ttu-id="bd96c-122">标头</span><span class="sxs-lookup"><span data-stu-id="bd96c-122">Header</span></span>       | <span data-ttu-id="bd96c-123">值</span><span class="sxs-lookup"><span data-stu-id="bd96c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd96c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd96c-124">Authorization</span></span>  | <span data-ttu-id="bd96c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd96c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd96c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd96c-127">Request body</span></span>

<span data-ttu-id="bd96c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd96c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd96c-129">响应</span><span class="sxs-lookup"><span data-stu-id="bd96c-129">Response</span></span>

<span data-ttu-id="bd96c-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Channel](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd96c-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd96c-131">示例</span><span class="sxs-lookup"><span data-stu-id="bd96c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd96c-132">请求</span><span class="sxs-lookup"><span data-stu-id="bd96c-132">Request</span></span>

<span data-ttu-id="bd96c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd96c-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd96c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd96c-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd96c-135">C#</span><span class="sxs-lookup"><span data-stu-id="bd96c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd96c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd96c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd96c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd96c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bd96c-138">响应</span><span class="sxs-lookup"><span data-stu-id="bd96c-138">Response</span></span>

<span data-ttu-id="bd96c-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bd96c-139">Here is an example of the response.</span></span>

> <span data-ttu-id="bd96c-140">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bd96c-140">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bd96c-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd96c-141">All of the properties will be returned from an actual call.</span></span>

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
      "membershipType": "membership-type-value"
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
