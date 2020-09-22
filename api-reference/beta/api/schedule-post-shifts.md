---
title: 创建班次
description: 创建新班次。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4561f3a36bc43f81b5ee05bded702c2ec558b1a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047006"
---
# <a name="create-shift"></a><span data-ttu-id="73e23-103">创建班次</span><span class="sxs-lookup"><span data-stu-id="73e23-103">Create shift</span></span>

<span data-ttu-id="73e23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73e23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73e23-105">按[计划](../resources/schedule.md)创建新的[班次](../resources/shift.md)实例。</span><span class="sxs-lookup"><span data-stu-id="73e23-105">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73e23-106">权限</span><span class="sxs-lookup"><span data-stu-id="73e23-106">Permissions</span></span>

<span data-ttu-id="73e23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73e23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73e23-109">Permission type</span></span>      | <span data-ttu-id="73e23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73e23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73e23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73e23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73e23-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73e23-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="73e23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73e23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73e23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73e23-114">Not supported.</span></span>    |
|<span data-ttu-id="73e23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73e23-115">Application</span></span> | <span data-ttu-id="73e23-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="73e23-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="73e23-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="73e23-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="73e23-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="73e23-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="73e23-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="73e23-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="73e23-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73e23-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="73e23-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="73e23-121">Request headers</span></span>

| <span data-ttu-id="73e23-122">标头</span><span class="sxs-lookup"><span data-stu-id="73e23-122">Header</span></span>       | <span data-ttu-id="73e23-123">值</span><span class="sxs-lookup"><span data-stu-id="73e23-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73e23-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="73e23-124">Authorization</span></span>  | <span data-ttu-id="73e23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73e23-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73e23-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73e23-127">Content-Type</span></span>  | <span data-ttu-id="73e23-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="73e23-p104">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="73e23-130">响应</span><span class="sxs-lookup"><span data-stu-id="73e23-130">Response</span></span>

<span data-ttu-id="73e23-131">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [shift](../resources/shift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73e23-131">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73e23-132">示例</span><span class="sxs-lookup"><span data-stu-id="73e23-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="73e23-133">请求</span><span class="sxs-lookup"><span data-stu-id="73e23-133">Request</span></span>

<span data-ttu-id="73e23-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73e23-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73e23-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="73e23-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="73e23-136">C#</span><span class="sxs-lookup"><span data-stu-id="73e23-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73e23-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73e23-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73e23-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73e23-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73e23-139">响应</span><span class="sxs-lookup"><span data-stu-id="73e23-139">Response</span></span>

<span data-ttu-id="73e23-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73e23-140">The following is an example of the response.</span></span> 

><span data-ttu-id="73e23-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73e23-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


