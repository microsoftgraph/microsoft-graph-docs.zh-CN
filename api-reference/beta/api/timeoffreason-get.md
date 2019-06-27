---
title: 获取 timeOffReason
description: 按 ID 获取 timeOffReason。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20ee24e4c3fb5c859c35a4e9196c1d8c6eb0b79f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270565"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="a479c-103">获取 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="a479c-103">Get timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a479c-104">按 ID 检索[timeOffReason](../resources/timeoffreason.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a479c-104">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a479c-105">权限</span><span class="sxs-lookup"><span data-stu-id="a479c-105">Permissions</span></span>

<span data-ttu-id="a479c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a479c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a479c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a479c-108">Permission type</span></span>      | <span data-ttu-id="a479c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a479c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a479c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a479c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a479c-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a479c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a479c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a479c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a479c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a479c-113">Not supported.</span></span>    |
|<span data-ttu-id="a479c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a479c-114">Application</span></span> | <span data-ttu-id="a479c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a479c-115">Not supported.</span></span> |

> <span data-ttu-id="a479c-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a479c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a479c-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="a479c-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a479c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a479c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="a479c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a479c-119">Request headers</span></span>

| <span data-ttu-id="a479c-120">标头</span><span class="sxs-lookup"><span data-stu-id="a479c-120">Header</span></span>       | <span data-ttu-id="a479c-121">值</span><span class="sxs-lookup"><span data-stu-id="a479c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a479c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a479c-122">Authorization</span></span>  | <span data-ttu-id="a479c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a479c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a479c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a479c-125">Content-Type</span></span>  | <span data-ttu-id="a479c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a479c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a479c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a479c-127">Request body</span></span>
<span data-ttu-id="a479c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a479c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a479c-129">响应</span><span class="sxs-lookup"><span data-stu-id="a479c-129">Response</span></span>

<span data-ttu-id="a479c-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[timeOffReason](../resources/timeoffreason.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a479c-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a479c-131">示例</span><span class="sxs-lookup"><span data-stu-id="a479c-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a479c-132">请求</span><span class="sxs-lookup"><span data-stu-id="a479c-132">Request</span></span>

<span data-ttu-id="a479c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a479c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="a479c-134">响应</span><span class="sxs-lookup"><span data-stu-id="a479c-134">Response</span></span>

<span data-ttu-id="a479c-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a479c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a479c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a479c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a479c-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a479c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a479c-139">C#</span><span class="sxs-lookup"><span data-stu-id="a479c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a479c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="a479c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a479c-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="a479c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
