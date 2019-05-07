---
title: 创建 timeOff
description: 创建新的 timeOff。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 04fb8821ea5592b1cb5521b711be67bbe5ce995a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638933"
---
# <a name="create-timeoff"></a><span data-ttu-id="773b0-103">创建 timeOff</span><span class="sxs-lookup"><span data-stu-id="773b0-103">Create timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="773b0-104">在[计划](../resources/schedule.md)中创建新的[timeOff](../resources/timeoff.md)实例。</span><span class="sxs-lookup"><span data-stu-id="773b0-104">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="773b0-105">权限</span><span class="sxs-lookup"><span data-stu-id="773b0-105">Permissions</span></span>

<span data-ttu-id="773b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="773b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="773b0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="773b0-108">Permission type</span></span>      | <span data-ttu-id="773b0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="773b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="773b0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="773b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="773b0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="773b0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="773b0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="773b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="773b0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="773b0-113">Not supported.</span></span>    |
|<span data-ttu-id="773b0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="773b0-114">Application</span></span> | <span data-ttu-id="773b0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="773b0-115">Not supported.</span></span> |

> <span data-ttu-id="773b0-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="773b0-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="773b0-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="773b0-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="773b0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="773b0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="773b0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="773b0-119">Request headers</span></span>

| <span data-ttu-id="773b0-120">标头</span><span class="sxs-lookup"><span data-stu-id="773b0-120">Header</span></span>       | <span data-ttu-id="773b0-121">值</span><span class="sxs-lookup"><span data-stu-id="773b0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="773b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="773b0-122">Authorization</span></span>  | <span data-ttu-id="773b0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="773b0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="773b0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="773b0-125">Content-Type</span></span>  | <span data-ttu-id="773b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="773b0-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="773b0-127">响应</span><span class="sxs-lookup"><span data-stu-id="773b0-127">Response</span></span>

<span data-ttu-id="773b0-128">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象。</span><span class="sxs-lookup"><span data-stu-id="773b0-128">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="773b0-129">示例</span><span class="sxs-lookup"><span data-stu-id="773b0-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="773b0-130">请求</span><span class="sxs-lookup"><span data-stu-id="773b0-130">Request</span></span>

<span data-ttu-id="773b0-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="773b0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff
Content-type: application/json

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
#### <a name="response"></a><span data-ttu-id="773b0-132">响应</span><span class="sxs-lookup"><span data-stu-id="773b0-132">Response</span></span>

<span data-ttu-id="773b0-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="773b0-133">The following is an example of the response.</span></span> 

><span data-ttu-id="773b0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="773b0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type":"microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 201 Created
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="773b0-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="773b0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="773b0-137">语言</span><span class="sxs-lookup"><span data-stu-id="773b0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="773b0-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="773b0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-timesoff.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-post-timesoff.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
