---
title: 'event: dismissReminder'
description: 消除对用户日历中的事件触发的提醒。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: db13f64b5df6ab3caa31775ba67757af954f4a3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43365651"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="5e37b-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="5e37b-103">event: dismissReminder</span></span>

<span data-ttu-id="5e37b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e37b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e37b-105">消除对用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)触发的提醒。</span><span class="sxs-lookup"><span data-stu-id="5e37b-105">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e37b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e37b-106">Permissions</span></span>
<span data-ttu-id="5e37b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e37b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e37b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e37b-109">Permission type</span></span>      | <span data-ttu-id="5e37b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e37b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e37b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e37b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e37b-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e37b-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5e37b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e37b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e37b-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e37b-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5e37b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e37b-115">Application</span></span> | <span data-ttu-id="5e37b-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e37b-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e37b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e37b-117">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5e37b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e37b-118">Request headers</span></span>

| <span data-ttu-id="5e37b-119">名称</span><span class="sxs-lookup"><span data-stu-id="5e37b-119">Name</span></span>       | <span data-ttu-id="5e37b-120">类型</span><span class="sxs-lookup"><span data-stu-id="5e37b-120">Type</span></span> | <span data-ttu-id="5e37b-121">说明</span><span class="sxs-lookup"><span data-stu-id="5e37b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e37b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e37b-122">Authorization</span></span>  | <span data-ttu-id="5e37b-123">string</span><span class="sxs-lookup"><span data-stu-id="5e37b-123">string</span></span>  | <span data-ttu-id="5e37b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e37b-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="5e37b-126">响应</span><span class="sxs-lookup"><span data-stu-id="5e37b-126">Response</span></span>

<span data-ttu-id="5e37b-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5e37b-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e37b-129">示例</span><span class="sxs-lookup"><span data-stu-id="5e37b-129">Example</span></span>

<span data-ttu-id="5e37b-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5e37b-130">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5e37b-131">请求</span><span class="sxs-lookup"><span data-stu-id="5e37b-131">Request</span></span>
<span data-ttu-id="5e37b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e37b-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5e37b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e37b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```
# <a name="c"></a>[<span data-ttu-id="5e37b-134">C#</span><span class="sxs-lookup"><span data-stu-id="5e37b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e37b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e37b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e37b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e37b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e37b-137">响应</span><span class="sxs-lookup"><span data-stu-id="5e37b-137">Response</span></span>
<span data-ttu-id="5e37b-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e37b-138">Here is an example of the response.</span></span>

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
  "suppressions": [
  ]
}
-->
