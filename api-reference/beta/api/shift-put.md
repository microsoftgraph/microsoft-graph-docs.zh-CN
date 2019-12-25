---
title: 替换班次
description: 替换现有班次。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 729441e7379c98270ab5df6c0ac10dbd920d308b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870916"
---
# <a name="replace-shift"></a><span data-ttu-id="990d3-103">替换班次</span><span class="sxs-lookup"><span data-stu-id="990d3-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="990d3-104">替换现有[班次](../resources/shift.md)。</span><span class="sxs-lookup"><span data-stu-id="990d3-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="990d3-105">如果指定的[班次](../resources/shift.md)不存在，则此方法`404 Not found`返回。</span><span class="sxs-lookup"><span data-stu-id="990d3-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="990d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="990d3-106">Permissions</span></span>

<span data-ttu-id="990d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="990d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="990d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="990d3-109">Permission type</span></span>      | <span data-ttu-id="990d3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="990d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="990d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="990d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="990d3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="990d3-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="990d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="990d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="990d3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="990d3-114">Not supported.</span></span>    |
|<span data-ttu-id="990d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="990d3-115">Application</span></span> | <span data-ttu-id="990d3-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="990d3-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="990d3-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="990d3-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="990d3-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="990d3-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="990d3-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="990d3-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="990d3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="990d3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="990d3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="990d3-121">Request headers</span></span>

| <span data-ttu-id="990d3-122">标头</span><span class="sxs-lookup"><span data-stu-id="990d3-122">Header</span></span>       | <span data-ttu-id="990d3-123">值</span><span class="sxs-lookup"><span data-stu-id="990d3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="990d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="990d3-124">Authorization</span></span>  | <span data-ttu-id="990d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="990d3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="990d3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="990d3-127">Content-Type</span></span>  | <span data-ttu-id="990d3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="990d3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="990d3-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="990d3-130">Request body</span></span>

<span data-ttu-id="990d3-131">在请求正文中，提供[shift](../resources/shift.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="990d3-131">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="990d3-132">响应</span><span class="sxs-lookup"><span data-stu-id="990d3-132">Response</span></span>

<span data-ttu-id="990d3-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[shift](../resources/shift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="990d3-133">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="990d3-134">示例</span><span class="sxs-lookup"><span data-stu-id="990d3-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="990d3-135">请求</span><span class="sxs-lookup"><span data-stu-id="990d3-135">Request</span></span>

<span data-ttu-id="990d3-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="990d3-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="990d3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="990d3-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="990d3-138">C#</span><span class="sxs-lookup"><span data-stu-id="990d3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="990d3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="990d3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="990d3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="990d3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="990d3-141">响应</span><span class="sxs-lookup"><span data-stu-id="990d3-141">Response</span></span>

<span data-ttu-id="990d3-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="990d3-142">The following is an example of the response.</span></span> 

><span data-ttu-id="990d3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="990d3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
