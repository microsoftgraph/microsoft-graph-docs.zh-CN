---
title: 替换班次
description: 替换现有班次。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: efe7180b352ae29bc64f663fa9122d670378dff5
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "42453327"
---
# <a name="replace-shift"></a><span data-ttu-id="170ff-103">替换班次</span><span class="sxs-lookup"><span data-stu-id="170ff-103">Replace shift</span></span>

<span data-ttu-id="170ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="170ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="170ff-105">替换现有[班次](../resources/shift.md)。</span><span class="sxs-lookup"><span data-stu-id="170ff-105">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="170ff-106">如果指定的[班次](../resources/shift.md)不存在，则此方法返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="170ff-106">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="170ff-107">权限</span><span class="sxs-lookup"><span data-stu-id="170ff-107">Permissions</span></span>

<span data-ttu-id="170ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="170ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="170ff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="170ff-110">Permission type</span></span>      | <span data-ttu-id="170ff-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="170ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170ff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="170ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="170ff-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170ff-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="170ff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="170ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="170ff-115">Not supported.</span></span>    |
|<span data-ttu-id="170ff-116">Application</span><span class="sxs-lookup"><span data-stu-id="170ff-116">Application</span></span> | <span data-ttu-id="170ff-117">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="170ff-117">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="170ff-118">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="170ff-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="170ff-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="170ff-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="170ff-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="170ff-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="170ff-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="170ff-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="170ff-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="170ff-122">Request headers</span></span>

| <span data-ttu-id="170ff-123">标头</span><span class="sxs-lookup"><span data-stu-id="170ff-123">Header</span></span>       | <span data-ttu-id="170ff-124">值</span><span class="sxs-lookup"><span data-stu-id="170ff-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="170ff-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="170ff-125">Authorization</span></span>  | <span data-ttu-id="170ff-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="170ff-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="170ff-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="170ff-128">Content-Type</span></span>  | <span data-ttu-id="170ff-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="170ff-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="170ff-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="170ff-131">Request body</span></span>

<span data-ttu-id="170ff-132">在请求正文中，提供[shift](../resources/shift.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="170ff-132">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="170ff-133">响应</span><span class="sxs-lookup"><span data-stu-id="170ff-133">Response</span></span>

<span data-ttu-id="170ff-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[shift](../resources/shift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="170ff-134">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="170ff-135">示例</span><span class="sxs-lookup"><span data-stu-id="170ff-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="170ff-136">请求</span><span class="sxs-lookup"><span data-stu-id="170ff-136">Request</span></span>

<span data-ttu-id="170ff-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="170ff-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="170ff-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="170ff-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

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
# <a name="c"></a>[<span data-ttu-id="170ff-139">C#</span><span class="sxs-lookup"><span data-stu-id="170ff-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="170ff-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170ff-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170ff-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170ff-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="170ff-142">响应</span><span class="sxs-lookup"><span data-stu-id="170ff-142">Response</span></span>

<span data-ttu-id="170ff-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="170ff-143">The following is an example of the response.</span></span> 

><span data-ttu-id="170ff-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="170ff-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
