---
title: 创建班次
description: 创建新班次。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed3e1e5d908d3683afeebe19a37b640cae567593
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867979"
---
# <a name="create-shift"></a><span data-ttu-id="7b8ab-103">创建班次</span><span class="sxs-lookup"><span data-stu-id="7b8ab-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b8ab-104">按[计划](../resources/schedule.md)创建新的[班次](../resources/shift.md)实例。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b8ab-105">权限</span><span class="sxs-lookup"><span data-stu-id="7b8ab-105">Permissions</span></span>

<span data-ttu-id="7b8ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b8ab-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b8ab-108">Permission type</span></span>      | <span data-ttu-id="7b8ab-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b8ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b8ab-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b8ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b8ab-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b8ab-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b8ab-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b8ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b8ab-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-113">Not supported.</span></span>    |
|<span data-ttu-id="7b8ab-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b8ab-114">Application</span></span> | <span data-ttu-id="7b8ab-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="7b8ab-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="7b8ab-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="7b8ab-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7b8ab-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7b8ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b8ab-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="7b8ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b8ab-120">Request headers</span></span>

| <span data-ttu-id="7b8ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b8ab-121">Header</span></span>       | <span data-ttu-id="7b8ab-122">值</span><span class="sxs-lookup"><span data-stu-id="7b8ab-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b8ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b8ab-123">Authorization</span></span>  | <span data-ttu-id="7b8ab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7b8ab-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b8ab-126">Content-Type</span></span>  | <span data-ttu-id="7b8ab-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7b8ab-p104">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7b8ab-129">响应</span><span class="sxs-lookup"><span data-stu-id="7b8ab-129">Response</span></span>

<span data-ttu-id="7b8ab-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和[shift](../resources/shift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-130">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b8ab-131">示例</span><span class="sxs-lookup"><span data-stu-id="7b8ab-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7b8ab-132">请求</span><span class="sxs-lookup"><span data-stu-id="7b8ab-132">Request</span></span>

<span data-ttu-id="7b8ab-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7b8ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b8ab-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts
Content-type: application/json

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b8ab-135">C#</span><span class="sxs-lookup"><span data-stu-id="7b8ab-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b8ab-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b8ab-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b8ab-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b8ab-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b8ab-138">响应</span><span class="sxs-lookup"><span data-stu-id="7b8ab-138">Response</span></span>

<span data-ttu-id="7b8ab-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-139">The following is an example of the response.</span></span> 

><span data-ttu-id="7b8ab-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b8ab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
