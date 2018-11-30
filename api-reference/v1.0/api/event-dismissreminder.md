---
title: 'event: dismissReminder'
description: 消除提醒用户日历中触发事件。
ms.openlocfilehash: d3ac1d09eb52991d9fcdc6c2f499d1415ac11141
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010863"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="8c41a-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="8c41a-103">event: dismissReminder</span></span>

<span data-ttu-id="8c41a-104">消除提醒用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)被触发。</span><span class="sxs-lookup"><span data-stu-id="8c41a-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c41a-105">权限</span><span class="sxs-lookup"><span data-stu-id="8c41a-105">Permissions</span></span>
<span data-ttu-id="8c41a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c41a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c41a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c41a-108">Permission type</span></span>      | <span data-ttu-id="8c41a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c41a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c41a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c41a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c41a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c41a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c41a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c41a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c41a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c41a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8c41a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c41a-114">Application</span></span> | <span data-ttu-id="8c41a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c41a-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c41a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c41a-116">HTTP request</span></span>

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

<br/>

## <a name="request-headers"></a><span data-ttu-id="8c41a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c41a-117">Request headers</span></span>
| <span data-ttu-id="8c41a-118">名称</span><span class="sxs-lookup"><span data-stu-id="8c41a-118">Name</span></span>       | <span data-ttu-id="8c41a-119">类型</span><span class="sxs-lookup"><span data-stu-id="8c41a-119">Type</span></span> | <span data-ttu-id="8c41a-120">说明</span><span class="sxs-lookup"><span data-stu-id="8c41a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c41a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c41a-121">Authorization</span></span>  | <span data-ttu-id="8c41a-122">string</span><span class="sxs-lookup"><span data-stu-id="8c41a-122">string</span></span>  | <span data-ttu-id="8c41a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c41a-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="8c41a-125">响应</span><span class="sxs-lookup"><span data-stu-id="8c41a-125">Response</span></span>

<span data-ttu-id="8c41a-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8c41a-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c41a-128">示例</span><span class="sxs-lookup"><span data-stu-id="8c41a-128">Example</span></span>

<span data-ttu-id="8c41a-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8c41a-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8c41a-130">请求</span><span class="sxs-lookup"><span data-stu-id="8c41a-130">Request</span></span>
<span data-ttu-id="8c41a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c41a-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="8c41a-132">响应</span><span class="sxs-lookup"><span data-stu-id="8c41a-132">Response</span></span>
<span data-ttu-id="8c41a-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8c41a-133">Here is an example of the response.</span></span>

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
