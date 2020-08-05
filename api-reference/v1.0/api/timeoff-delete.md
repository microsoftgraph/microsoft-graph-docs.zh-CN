---
title: 删除 timeOff
description: 从计划中删除 timeOff 实例。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 68c26aafd2dcf5f7c4755117587267e9c03e3eaf
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/04/2020
ms.locfileid: "44218052"
---
# <a name="delete-timeoff"></a><span data-ttu-id="67d11-103">删除 timeOff</span><span class="sxs-lookup"><span data-stu-id="67d11-103">Delete timeOff</span></span>

<span data-ttu-id="67d11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67d11-105">从[计划](../resources/schedule.md)中删除[timeOff](../resources/timeoff.md)实例。</span><span class="sxs-lookup"><span data-stu-id="67d11-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67d11-106">权限</span><span class="sxs-lookup"><span data-stu-id="67d11-106">Permissions</span></span>

<span data-ttu-id="67d11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67d11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67d11-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67d11-109">Permission type</span></span>      | <span data-ttu-id="67d11-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67d11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67d11-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67d11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67d11-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="67d11-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="67d11-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67d11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67d11-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="67d11-114">Not supported.</span></span>    |
|<span data-ttu-id="67d11-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="67d11-115">Application</span></span> | <span data-ttu-id="67d11-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67d11-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="67d11-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="67d11-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="67d11-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="67d11-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="67d11-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67d11-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="67d11-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="67d11-120">Request headers</span></span>

| <span data-ttu-id="67d11-121">标头</span><span class="sxs-lookup"><span data-stu-id="67d11-121">Header</span></span>       | <span data-ttu-id="67d11-122">值</span><span class="sxs-lookup"><span data-stu-id="67d11-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67d11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67d11-123">Authorization</span></span>  | <span data-ttu-id="67d11-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67d11-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67d11-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67d11-126">Request body</span></span>
<span data-ttu-id="67d11-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67d11-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67d11-128">响应</span><span class="sxs-lookup"><span data-stu-id="67d11-128">Response</span></span>

<span data-ttu-id="67d11-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="67d11-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67d11-131">示例</span><span class="sxs-lookup"><span data-stu-id="67d11-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="67d11-132">请求</span><span class="sxs-lookup"><span data-stu-id="67d11-132">Request</span></span>

<span data-ttu-id="67d11-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67d11-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67d11-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="67d11-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="67d11-135">C#</span><span class="sxs-lookup"><span data-stu-id="67d11-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67d11-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67d11-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67d11-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67d11-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67d11-138">Java</span><span class="sxs-lookup"><span data-stu-id="67d11-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="67d11-139">响应</span><span class="sxs-lookup"><span data-stu-id="67d11-139">Response</span></span>

<span data-ttu-id="67d11-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67d11-140">The following is an example of the response.</span></span> 

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
