---
title: 替换 timeOffReason
description: 替换现有的 timeOffReason。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6e28a22e7a49d35d7ae0f06affb0652ad37ce538
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452279"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="850f7-103">替换 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="850f7-103">Replace timeOffReason</span></span>

<span data-ttu-id="850f7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="850f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="850f7-105">替换现有的[timeOffReason](../resources/timeoffreason.md)。</span><span class="sxs-lookup"><span data-stu-id="850f7-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="850f7-106">如果指定的[timeOffReason](../resources/timeoffreason.md)不存在，则此方法`404 Not found`返回。</span><span class="sxs-lookup"><span data-stu-id="850f7-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="850f7-107">权限</span><span class="sxs-lookup"><span data-stu-id="850f7-107">Permissions</span></span>

<span data-ttu-id="850f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="850f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="850f7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="850f7-110">Permission type</span></span>      | <span data-ttu-id="850f7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="850f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="850f7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="850f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="850f7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="850f7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="850f7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="850f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="850f7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="850f7-115">Not supported.</span></span>    |
|<span data-ttu-id="850f7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="850f7-116">Application</span></span> | <span data-ttu-id="850f7-117">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="850f7-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="850f7-118">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="850f7-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="850f7-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="850f7-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="850f7-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="850f7-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="850f7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="850f7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="850f7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="850f7-122">Request headers</span></span>

| <span data-ttu-id="850f7-123">标头</span><span class="sxs-lookup"><span data-stu-id="850f7-123">Header</span></span>       | <span data-ttu-id="850f7-124">值</span><span class="sxs-lookup"><span data-stu-id="850f7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="850f7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="850f7-125">Authorization</span></span>  | <span data-ttu-id="850f7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="850f7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="850f7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="850f7-128">Content-Type</span></span>  | <span data-ttu-id="850f7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="850f7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="850f7-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="850f7-131">Request body</span></span>

<span data-ttu-id="850f7-132">在请求正文中，提供[timeOffReason](../resources/timeoffreason.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="850f7-132">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="850f7-133">响应</span><span class="sxs-lookup"><span data-stu-id="850f7-133">Response</span></span>

<span data-ttu-id="850f7-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和[timeOffReason](../resources/timeoffreason.md)对象。</span><span class="sxs-lookup"><span data-stu-id="850f7-134">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="850f7-135">示例</span><span class="sxs-lookup"><span data-stu-id="850f7-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="850f7-136">请求</span><span class="sxs-lookup"><span data-stu-id="850f7-136">Request</span></span>

<span data-ttu-id="850f7-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="850f7-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="850f7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="850f7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="850f7-139">C#</span><span class="sxs-lookup"><span data-stu-id="850f7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="850f7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="850f7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="850f7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="850f7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="850f7-142">响应</span><span class="sxs-lookup"><span data-stu-id="850f7-142">Response</span></span>

<span data-ttu-id="850f7-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="850f7-143">The following is an example of the response.</span></span> 

><span data-ttu-id="850f7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="850f7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "displayName": "Alex Wilbur"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
