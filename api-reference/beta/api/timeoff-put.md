---
title: 替换 timeOff
description: 替换现有的 timeOff。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9288ed6db5111b99f4cf0f7488d81626678f90dc
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895289"
---
# <a name="replace-timeoff"></a><span data-ttu-id="12533-103">替换 timeOff</span><span class="sxs-lookup"><span data-stu-id="12533-103">Replace timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12533-104">替换现有的[timeOff](../resources/timeoff.md)。</span><span class="sxs-lookup"><span data-stu-id="12533-104">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="12533-105">如果指定的[timeOff](../resources/timeoff.md)不存在，则此方法`404 Not found`返回。</span><span class="sxs-lookup"><span data-stu-id="12533-105">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="12533-106">权限</span><span class="sxs-lookup"><span data-stu-id="12533-106">Permissions</span></span>

<span data-ttu-id="12533-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12533-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12533-109">Permission type</span></span>      | <span data-ttu-id="12533-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12533-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12533-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12533-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12533-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12533-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="12533-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12533-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12533-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12533-114">Not supported.</span></span>    |
|<span data-ttu-id="12533-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12533-115">Application</span></span> | <span data-ttu-id="12533-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12533-116">Not supported.</span></span> |

> <span data-ttu-id="12533-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="12533-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="12533-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="12533-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="12533-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12533-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="12533-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12533-120">Request headers</span></span>

| <span data-ttu-id="12533-121">标头</span><span class="sxs-lookup"><span data-stu-id="12533-121">Header</span></span>       | <span data-ttu-id="12533-122">值</span><span class="sxs-lookup"><span data-stu-id="12533-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12533-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12533-123">Authorization</span></span>  | <span data-ttu-id="12533-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12533-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12533-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12533-126">Content-Type</span></span>  | <span data-ttu-id="12533-127">application/json</span><span class="sxs-lookup"><span data-stu-id="12533-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12533-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="12533-128">Request body</span></span>

<span data-ttu-id="12533-129">在请求正文中，提供[timeOff](../resources/timeoff.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12533-129">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12533-130">响应</span><span class="sxs-lookup"><span data-stu-id="12533-130">Response</span></span>

<span data-ttu-id="12533-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12533-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12533-132">示例</span><span class="sxs-lookup"><span data-stu-id="12533-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="12533-133">请求</span><span class="sxs-lookup"><span data-stu-id="12533-133">Request</span></span>

<span data-ttu-id="12533-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="12533-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="12533-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="12533-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="12533-136">C#</span><span class="sxs-lookup"><span data-stu-id="12533-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12533-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12533-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="12533-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12533-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="12533-139">响应</span><span class="sxs-lookup"><span data-stu-id="12533-139">Response</span></span>

<span data-ttu-id="12533-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="12533-140">The following is an example of the response.</span></span> 

><span data-ttu-id="12533-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="12533-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.type":"microsoft.graph.identitySet",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
