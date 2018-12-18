---
title: 删除日历
description: 删除默认日历以外的日历。
author: angelgolfer-ms
ms.openlocfilehash: d8e2a7aaaff9f4489d5ef1cbcae97bcdbceb8f17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348788"
---
# <a name="delete-calendar"></a><span data-ttu-id="c0ada-103">删除日历</span><span class="sxs-lookup"><span data-stu-id="c0ada-103">Delete calendar</span></span>

> <span data-ttu-id="c0ada-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c0ada-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0ada-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c0ada-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0ada-106">删除默认日历以外的日历。</span><span class="sxs-lookup"><span data-stu-id="c0ada-106">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0ada-107">权限</span><span class="sxs-lookup"><span data-stu-id="c0ada-107">Permissions</span></span>
<span data-ttu-id="c0ada-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0ada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ada-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0ada-110">Permission type</span></span>      | <span data-ttu-id="c0ada-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0ada-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0ada-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0ada-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0ada-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0ada-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c0ada-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0ada-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0ada-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0ada-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c0ada-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0ada-116">Application</span></span> | <span data-ttu-id="c0ada-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0ada-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0ada-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0ada-118">HTTP request</span></span>
<span data-ttu-id="c0ada-119"><!-- { "blockType": "ignored" } -->默认[calendarGroup](../resources/calendargroup.md)中的默认日历之外的用户的[日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="c0ada-119"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="c0ada-120">指定 [calendarGroup](../resources/calendargroup.md) 中的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="c0ada-120">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c0ada-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0ada-121">Request headers</span></span>
| <span data-ttu-id="c0ada-122">Name</span><span class="sxs-lookup"><span data-stu-id="c0ada-122">Name</span></span>           |  <span data-ttu-id="c0ada-123">类型</span><span class="sxs-lookup"><span data-stu-id="c0ada-123">Type</span></span>    | <span data-ttu-id="c0ada-124">说明</span><span class="sxs-lookup"><span data-stu-id="c0ada-124">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="c0ada-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0ada-125">Authorization</span></span>  |  <span data-ttu-id="c0ada-126">string</span><span class="sxs-lookup"><span data-stu-id="c0ada-126">string</span></span>  | <span data-ttu-id="c0ada-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0ada-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0ada-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0ada-129">Request body</span></span>
<span data-ttu-id="c0ada-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0ada-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0ada-131">响应</span><span class="sxs-lookup"><span data-stu-id="c0ada-131">Response</span></span>

<span data-ttu-id="c0ada-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c0ada-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0ada-134">示例</span><span class="sxs-lookup"><span data-stu-id="c0ada-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0ada-135">请求</span><span class="sxs-lookup"><span data-stu-id="c0ada-135">Request</span></span>
<span data-ttu-id="c0ada-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0ada-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="c0ada-137">响应</span><span class="sxs-lookup"><span data-stu-id="c0ada-137">Response</span></span>
<span data-ttu-id="c0ada-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0ada-138">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
