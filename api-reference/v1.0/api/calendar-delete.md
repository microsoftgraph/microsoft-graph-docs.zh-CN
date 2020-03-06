---
title: 删除日历
description: 删除默认日历以外的日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f39115551e5bd8890e95075245946f48c8a8bc23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518824"
---
# <a name="delete-calendar"></a><span data-ttu-id="b3778-103">删除日历</span><span class="sxs-lookup"><span data-stu-id="b3778-103">Delete calendar</span></span>

<span data-ttu-id="b3778-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3778-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3778-105">删除默认日历以外的日历。</span><span class="sxs-lookup"><span data-stu-id="b3778-105">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3778-106">权限</span><span class="sxs-lookup"><span data-stu-id="b3778-106">Permissions</span></span>
<span data-ttu-id="b3778-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3778-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3778-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3778-109">Permission type</span></span>      | <span data-ttu-id="b3778-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3778-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3778-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3778-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3778-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3778-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b3778-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3778-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3778-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3778-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b3778-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3778-115">Application</span></span> | <span data-ttu-id="b3778-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3778-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3778-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3778-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b3778-118">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="b3778-118">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="b3778-119">指定 [calendarGroup](../resources/calendargroup.md) 中的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="b3778-119">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b3778-120">请求头</span><span class="sxs-lookup"><span data-stu-id="b3778-120">Request headers</span></span>
| <span data-ttu-id="b3778-121">名称</span><span class="sxs-lookup"><span data-stu-id="b3778-121">Name</span></span>           |  <span data-ttu-id="b3778-122">类型</span><span class="sxs-lookup"><span data-stu-id="b3778-122">Type</span></span>    | <span data-ttu-id="b3778-123">说明</span><span class="sxs-lookup"><span data-stu-id="b3778-123">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="b3778-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3778-124">Authorization</span></span>  |  <span data-ttu-id="b3778-125">string</span><span class="sxs-lookup"><span data-stu-id="b3778-125">string</span></span>  | <span data-ttu-id="b3778-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3778-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3778-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3778-128">Request body</span></span>
<span data-ttu-id="b3778-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3778-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3778-130">响应</span><span class="sxs-lookup"><span data-stu-id="b3778-130">Response</span></span>

<span data-ttu-id="b3778-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b3778-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3778-133">示例</span><span class="sxs-lookup"><span data-stu-id="b3778-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3778-134">请求</span><span class="sxs-lookup"><span data-stu-id="b3778-134">Request</span></span>
<span data-ttu-id="b3778-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3778-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3778-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3778-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="b3778-137">C#</span><span class="sxs-lookup"><span data-stu-id="b3778-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3778-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3778-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3778-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3778-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3778-140">Java</span><span class="sxs-lookup"><span data-stu-id="b3778-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3778-141">响应</span><span class="sxs-lookup"><span data-stu-id="b3778-141">Response</span></span>
<span data-ttu-id="b3778-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b3778-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
