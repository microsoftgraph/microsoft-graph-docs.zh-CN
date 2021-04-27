---
title: 创建班次
description: 创建新的班次。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e74b00a6ec3563d5ee47b13fb4d082d6a0e9bfaf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052731"
---
# <a name="create-shift"></a><span data-ttu-id="32f5c-103">创建班次</span><span class="sxs-lookup"><span data-stu-id="32f5c-103">Create shift</span></span>

<span data-ttu-id="32f5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32f5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32f5c-105">在计划 [中](../resources/shift.md) 创建新的班次 [实例](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="32f5c-105">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="32f5c-106">权限</span><span class="sxs-lookup"><span data-stu-id="32f5c-106">Permissions</span></span>

<span data-ttu-id="32f5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32f5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f5c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="32f5c-109">Permission type</span></span>      | <span data-ttu-id="32f5c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32f5c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32f5c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32f5c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32f5c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32f5c-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="32f5c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32f5c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32f5c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="32f5c-114">Not supported.</span></span>    |
|<span data-ttu-id="32f5c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="32f5c-115">Application</span></span> | <span data-ttu-id="32f5c-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="32f5c-116">Schedule.ReadWrite.All\*</span></span> |

## <a name="http-request"></a><span data-ttu-id="32f5c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32f5c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="32f5c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="32f5c-118">Request headers</span></span>

| <span data-ttu-id="32f5c-119">标头</span><span class="sxs-lookup"><span data-stu-id="32f5c-119">Header</span></span>       | <span data-ttu-id="32f5c-120">值</span><span class="sxs-lookup"><span data-stu-id="32f5c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32f5c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32f5c-121">Authorization</span></span>  | <span data-ttu-id="32f5c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32f5c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="32f5c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32f5c-124">Content-Type</span></span>  | <span data-ttu-id="32f5c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="32f5c-p103">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="32f5c-127">响应</span><span class="sxs-lookup"><span data-stu-id="32f5c-127">Response</span></span>

<span data-ttu-id="32f5c-128">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [shift](../resources/shift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32f5c-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f5c-129">示例</span><span class="sxs-lookup"><span data-stu-id="32f5c-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32f5c-130">请求</span><span class="sxs-lookup"><span data-stu-id="32f5c-130">Request</span></span>

<span data-ttu-id="32f5c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="32f5c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32f5c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="32f5c-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="32f5c-133">C#</span><span class="sxs-lookup"><span data-stu-id="32f5c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32f5c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32f5c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32f5c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32f5c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32f5c-136">Java</span><span class="sxs-lookup"><span data-stu-id="32f5c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-shifts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32f5c-137">响应</span><span class="sxs-lookup"><span data-stu-id="32f5c-137">Response</span></span>

<span data-ttu-id="32f5c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="32f5c-138">The following is an example of the response.</span></span> 

><span data-ttu-id="32f5c-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="32f5c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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


