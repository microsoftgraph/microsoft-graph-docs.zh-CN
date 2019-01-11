---
title: 'event: dismissReminder'
description: 消除提醒用户日历中触发事件。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 570a9b34031afe6d53b6e577127180ebdbe7a163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864937"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="d70b5-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="d70b5-103">event: dismissReminder</span></span>

> <span data-ttu-id="d70b5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d70b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d70b5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d70b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d70b5-106">消除提醒用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)被触发。</span><span class="sxs-lookup"><span data-stu-id="d70b5-106">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d70b5-107">权限</span><span class="sxs-lookup"><span data-stu-id="d70b5-107">Permissions</span></span>
<span data-ttu-id="d70b5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d70b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d70b5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d70b5-110">Permission type</span></span>      | <span data-ttu-id="d70b5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d70b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d70b5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d70b5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d70b5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d70b5-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d70b5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d70b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d70b5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d70b5-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d70b5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d70b5-116">Application</span></span> | <span data-ttu-id="d70b5-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d70b5-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d70b5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d70b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

## <a name="request-headers"></a><span data-ttu-id="d70b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d70b5-119">Request headers</span></span>

| <span data-ttu-id="d70b5-120">名称</span><span class="sxs-lookup"><span data-stu-id="d70b5-120">Name</span></span>       | <span data-ttu-id="d70b5-121">类型</span><span class="sxs-lookup"><span data-stu-id="d70b5-121">Type</span></span> | <span data-ttu-id="d70b5-122">说明</span><span class="sxs-lookup"><span data-stu-id="d70b5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d70b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d70b5-123">Authorization</span></span>  | <span data-ttu-id="d70b5-124">string</span><span class="sxs-lookup"><span data-stu-id="d70b5-124">string</span></span>  | <span data-ttu-id="d70b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d70b5-p103">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="d70b5-127">响应</span><span class="sxs-lookup"><span data-stu-id="d70b5-127">Response</span></span>

<span data-ttu-id="d70b5-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d70b5-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70b5-130">示例</span><span class="sxs-lookup"><span data-stu-id="d70b5-130">Example</span></span>

<span data-ttu-id="d70b5-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d70b5-131">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d70b5-132">请求</span><span class="sxs-lookup"><span data-stu-id="d70b5-132">Request</span></span>
<span data-ttu-id="d70b5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d70b5-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="d70b5-134">响应</span><span class="sxs-lookup"><span data-stu-id="d70b5-134">Response</span></span>
<span data-ttu-id="d70b5-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d70b5-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
