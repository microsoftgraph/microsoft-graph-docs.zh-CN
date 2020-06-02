---
title: 删除 timeOff
description: 从计划中删除 timeOff 实例。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 41f41df6b773d18aecb132bb3311447bbeb72bd3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "42452314"
---
# <a name="delete-timeoff"></a><span data-ttu-id="b96a9-103">删除 timeOff</span><span class="sxs-lookup"><span data-stu-id="b96a9-103">Delete timeOff</span></span>

<span data-ttu-id="b96a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b96a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b96a9-105">从[计划](../resources/schedule.md)中删除[timeOff](../resources/timeoff.md)实例。</span><span class="sxs-lookup"><span data-stu-id="b96a9-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b96a9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b96a9-106">Permissions</span></span>

<span data-ttu-id="b96a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b96a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b96a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b96a9-109">Permission type</span></span>      | <span data-ttu-id="b96a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b96a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b96a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b96a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b96a9-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b96a9-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b96a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b96a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b96a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b96a9-114">Not supported.</span></span>    |
|<span data-ttu-id="b96a9-115">Application</span><span class="sxs-lookup"><span data-stu-id="b96a9-115">Application</span></span> | <span data-ttu-id="b96a9-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="b96a9-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="b96a9-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="b96a9-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b96a9-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b96a9-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b96a9-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="b96a9-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b96a9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b96a9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="b96a9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b96a9-121">Request headers</span></span>

| <span data-ttu-id="b96a9-122">标头</span><span class="sxs-lookup"><span data-stu-id="b96a9-122">Header</span></span>       | <span data-ttu-id="b96a9-123">值</span><span class="sxs-lookup"><span data-stu-id="b96a9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b96a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b96a9-124">Authorization</span></span>  | <span data-ttu-id="b96a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b96a9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b96a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b96a9-127">Request body</span></span>
<span data-ttu-id="b96a9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b96a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b96a9-129">响应</span><span class="sxs-lookup"><span data-stu-id="b96a9-129">Response</span></span>

<span data-ttu-id="b96a9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b96a9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b96a9-132">示例</span><span class="sxs-lookup"><span data-stu-id="b96a9-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b96a9-133">请求</span><span class="sxs-lookup"><span data-stu-id="b96a9-133">Request</span></span>

<span data-ttu-id="b96a9-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b96a9-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b96a9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b96a9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="b96a9-136">C#</span><span class="sxs-lookup"><span data-stu-id="b96a9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b96a9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b96a9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b96a9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b96a9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b96a9-139">响应</span><span class="sxs-lookup"><span data-stu-id="b96a9-139">Response</span></span>

<span data-ttu-id="b96a9-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b96a9-140">The following is an example of the response.</span></span> 

><span data-ttu-id="b96a9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b96a9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
