---
title: 删除日历
description: 删除默认日历以外的日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2e9195ef561ffeb8174d31eac51a9b75a6b7eb72
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865164"
---
# <a name="delete-calendar"></a><span data-ttu-id="4a670-103">删除日历</span><span class="sxs-lookup"><span data-stu-id="4a670-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a670-104">删除默认日历以外的日历。</span><span class="sxs-lookup"><span data-stu-id="4a670-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a670-105">权限</span><span class="sxs-lookup"><span data-stu-id="4a670-105">Permissions</span></span>
<span data-ttu-id="4a670-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a670-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a670-108">Permission type</span></span>      | <span data-ttu-id="4a670-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a670-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a670-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a670-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a670-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a670-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4a670-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a670-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a670-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a670-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4a670-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a670-114">Application</span></span> | <span data-ttu-id="4a670-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a670-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a670-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a670-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4a670-117">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="4a670-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="4a670-118">指定 [calendarGroup](../resources/calendargroup.md) 中的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="4a670-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a670-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a670-119">Request headers</span></span>
| <span data-ttu-id="4a670-120">名称</span><span class="sxs-lookup"><span data-stu-id="4a670-120">Name</span></span>           |  <span data-ttu-id="4a670-121">类型</span><span class="sxs-lookup"><span data-stu-id="4a670-121">Type</span></span>    | <span data-ttu-id="4a670-122">说明</span><span class="sxs-lookup"><span data-stu-id="4a670-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="4a670-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a670-123">Authorization</span></span>  |  <span data-ttu-id="4a670-124">string</span><span class="sxs-lookup"><span data-stu-id="4a670-124">string</span></span>  | <span data-ttu-id="4a670-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a670-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a670-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a670-127">Request body</span></span>
<span data-ttu-id="4a670-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a670-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a670-129">响应</span><span class="sxs-lookup"><span data-stu-id="4a670-129">Response</span></span>

<span data-ttu-id="4a670-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4a670-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a670-132">示例</span><span class="sxs-lookup"><span data-stu-id="4a670-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a670-133">请求</span><span class="sxs-lookup"><span data-stu-id="4a670-133">Request</span></span>
<span data-ttu-id="4a670-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a670-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4a670-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4a670-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a670-136">C#</span><span class="sxs-lookup"><span data-stu-id="4a670-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a670-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a670-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a670-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="4a670-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a670-139">Java</span><span class="sxs-lookup"><span data-stu-id="4a670-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a670-140">响应</span><span class="sxs-lookup"><span data-stu-id="4a670-140">Response</span></span>
<span data-ttu-id="4a670-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a670-141">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
