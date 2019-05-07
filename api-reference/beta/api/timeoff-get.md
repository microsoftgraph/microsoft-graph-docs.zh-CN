---
title: 获取 timeOff
description: 按 ID 获取 timeOff。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f1fdd14a155c7113425916081ed38f5745267e2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637532"
---
# <a name="get-timeoff"></a><span data-ttu-id="0d0d4-103">获取 timeOff</span><span class="sxs-lookup"><span data-stu-id="0d0d4-103">Get timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d0d4-104">按 ID 检索[timeOff](../resources/timeoff.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-104">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d0d4-105">权限</span><span class="sxs-lookup"><span data-stu-id="0d0d4-105">Permissions</span></span>

<span data-ttu-id="0d0d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d0d4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d0d4-108">Permission type</span></span>      | <span data-ttu-id="0d0d4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d0d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d0d4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d0d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d0d4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d0d4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d0d4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d0d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d0d4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-113">Not supported.</span></span>    |
|<span data-ttu-id="0d0d4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d0d4-114">Application</span></span> | <span data-ttu-id="0d0d4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-115">Not supported.</span></span> |

> <span data-ttu-id="0d0d4-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0d0d4-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0d0d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d0d4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="0d0d4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d0d4-119">Request headers</span></span>

| <span data-ttu-id="0d0d4-120">标头</span><span class="sxs-lookup"><span data-stu-id="0d0d4-120">Header</span></span>       | <span data-ttu-id="0d0d4-121">值</span><span class="sxs-lookup"><span data-stu-id="0d0d4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d0d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d0d4-122">Authorization</span></span>  | <span data-ttu-id="0d0d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d0d4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d0d4-125">Content-Type</span></span>  | <span data-ttu-id="0d0d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d0d4-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d0d4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d0d4-127">Request body</span></span>
<span data-ttu-id="0d0d4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d0d4-129">响应</span><span class="sxs-lookup"><span data-stu-id="0d0d4-129">Response</span></span>

<span data-ttu-id="0d0d4-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d0d4-131">示例</span><span class="sxs-lookup"><span data-stu-id="0d0d4-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0d0d4-132">请求</span><span class="sxs-lookup"><span data-stu-id="0d0d4-132">Request</span></span>

<span data-ttu-id="0d0d4-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="0d0d4-134">响应</span><span class="sxs-lookup"><span data-stu-id="0d0d4-134">Response</span></span>

<span data-ttu-id="0d0d4-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-135">The following is an example of the response.</span></span> 

><span data-ttu-id="0d0d4-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d0d4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d0d4-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0d0d4-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d0d4-139">语言</span><span class="sxs-lookup"><span data-stu-id="0d0d4-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d0d4-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d0d4-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-get-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
