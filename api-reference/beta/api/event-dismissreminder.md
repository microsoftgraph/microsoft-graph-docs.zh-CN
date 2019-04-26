---
title: 'event: dismissReminder'
description: 消除对用户日历中的事件触发的提醒。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dd10d8a94e2661f2006ccb10c4a823c4afc3fdb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324388"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="c4dc8-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="c4dc8-103">event: dismissReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4dc8-104">消除对用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)触发的提醒。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4dc8-105">权限</span><span class="sxs-lookup"><span data-stu-id="c4dc8-105">Permissions</span></span>
<span data-ttu-id="c4dc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4dc8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4dc8-108">Permission type</span></span>      | <span data-ttu-id="c4dc8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4dc8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4dc8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4dc8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4dc8-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4dc8-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c4dc8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4dc8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4dc8-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4dc8-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c4dc8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4dc8-114">Application</span></span> | <span data-ttu-id="c4dc8-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4dc8-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4dc8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4dc8-116">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c4dc8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4dc8-117">Request headers</span></span>

| <span data-ttu-id="c4dc8-118">名称</span><span class="sxs-lookup"><span data-stu-id="c4dc8-118">Name</span></span>       | <span data-ttu-id="c4dc8-119">类型</span><span class="sxs-lookup"><span data-stu-id="c4dc8-119">Type</span></span> | <span data-ttu-id="c4dc8-120">说明</span><span class="sxs-lookup"><span data-stu-id="c4dc8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4dc8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4dc8-121">Authorization</span></span>  | <span data-ttu-id="c4dc8-122">string</span><span class="sxs-lookup"><span data-stu-id="c4dc8-122">string</span></span>  | <span data-ttu-id="c4dc8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="c4dc8-125">响应</span><span class="sxs-lookup"><span data-stu-id="c4dc8-125">Response</span></span>

<span data-ttu-id="c4dc8-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4dc8-128">示例</span><span class="sxs-lookup"><span data-stu-id="c4dc8-128">Example</span></span>

<span data-ttu-id="c4dc8-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c4dc8-130">请求</span><span class="sxs-lookup"><span data-stu-id="c4dc8-130">Request</span></span>
<span data-ttu-id="c4dc8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="c4dc8-132">响应</span><span class="sxs-lookup"><span data-stu-id="c4dc8-132">Response</span></span>
<span data-ttu-id="c4dc8-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4dc8-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
