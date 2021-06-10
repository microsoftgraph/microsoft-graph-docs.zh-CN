---
title: 删除 timeCard
description: 删除计划中的 timeCard 实例。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc76b48ac1bac83435446d50e93a93ef256a49be
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869728"
---
# <a name="delete-timecard"></a><span data-ttu-id="73ef8-103">删除 timeCard</span><span class="sxs-lookup"><span data-stu-id="73ef8-103">Delete timeCard</span></span>

<span data-ttu-id="73ef8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73ef8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73ef8-105">删除 [计划 中的 timeCard](../resources/timeCard.md) [实例](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="73ef8-105">Delete a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73ef8-106">权限</span><span class="sxs-lookup"><span data-stu-id="73ef8-106">Permissions</span></span>

<span data-ttu-id="73ef8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73ef8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73ef8-109">Permission type</span></span>      | <span data-ttu-id="73ef8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73ef8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73ef8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73ef8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73ef8-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ef8-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="73ef8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73ef8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73ef8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73ef8-114">Not supported.</span></span>    |
|<span data-ttu-id="73ef8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73ef8-115">Application</span></span> | <span data-ttu-id="73ef8-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="73ef8-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="73ef8-117">\***重要提示：** 使用应用程序权限时，必须在请求 `MS-APP-ACTS-AS` 中包括 标头。</span><span class="sxs-lookup"><span data-stu-id="73ef8-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="73ef8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73ef8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="73ef8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73ef8-119">Request headers</span></span>

| <span data-ttu-id="73ef8-120">标头</span><span class="sxs-lookup"><span data-stu-id="73ef8-120">Header</span></span>       | <span data-ttu-id="73ef8-121">值</span><span class="sxs-lookup"><span data-stu-id="73ef8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73ef8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73ef8-122">Authorization</span></span>  | <span data-ttu-id="73ef8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73ef8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73ef8-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="73ef8-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="73ef8-126">应用代表其操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="73ef8-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="73ef8-127">使用应用程序权限范围时是必需的。</span><span class="sxs-lookup"><span data-stu-id="73ef8-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73ef8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="73ef8-128">Request body</span></span>
<span data-ttu-id="73ef8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73ef8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73ef8-130">响应</span><span class="sxs-lookup"><span data-stu-id="73ef8-130">Response</span></span>

<span data-ttu-id="73ef8-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="73ef8-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="73ef8-132">示例</span><span class="sxs-lookup"><span data-stu-id="73ef8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="73ef8-133">请求</span><span class="sxs-lookup"><span data-stu-id="73ef8-133">Request</span></span>
<span data-ttu-id="73ef8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73ef8-134">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="73ef8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="73ef8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```
# <a name="c"></a>[<span data-ttu-id="73ef8-136">C#</span><span class="sxs-lookup"><span data-stu-id="73ef8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73ef8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73ef8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73ef8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73ef8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73ef8-139">Java</span><span class="sxs-lookup"><span data-stu-id="73ef8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73ef8-140">响应</span><span class="sxs-lookup"><span data-stu-id="73ef8-140">Response</span></span>

<span data-ttu-id="73ef8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73ef8-141">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
