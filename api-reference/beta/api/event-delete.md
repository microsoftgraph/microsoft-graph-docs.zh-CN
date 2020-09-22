---
title: 删除事件
description: 删除事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b2813a6206f011dd484d52a14257fd957879f30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980980"
---
# <a name="delete-event"></a><span data-ttu-id="2e654-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="2e654-103">Delete event</span></span>

<span data-ttu-id="2e654-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e654-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e654-105">从包含的日历中删除指定[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="2e654-105">Removes the specified [event](../resources/event.md) from the containing calendar.</span></span> 

<span data-ttu-id="2e654-106">如果事件是会议，则在组织者的日历上删除事件会向与会者发送取消邮件。</span><span class="sxs-lookup"><span data-stu-id="2e654-106">If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e654-107">权限</span><span class="sxs-lookup"><span data-stu-id="2e654-107">Permissions</span></span>
<span data-ttu-id="2e654-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e654-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e654-110">Permission type</span></span>      | <span data-ttu-id="2e654-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e654-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e654-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e654-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2e654-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e654-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e654-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e654-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e654-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e654-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e654-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e654-116">Application</span></span> | <span data-ttu-id="2e654-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e654-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e654-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e654-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e654-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e654-119">Request headers</span></span>
| <span data-ttu-id="2e654-120">名称</span><span class="sxs-lookup"><span data-stu-id="2e654-120">Name</span></span>       | <span data-ttu-id="2e654-121">类型</span><span class="sxs-lookup"><span data-stu-id="2e654-121">Type</span></span> | <span data-ttu-id="2e654-122">说明</span><span class="sxs-lookup"><span data-stu-id="2e654-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2e654-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e654-123">Authorization</span></span>  | <span data-ttu-id="2e654-124">string</span><span class="sxs-lookup"><span data-stu-id="2e654-124">string</span></span>  | <span data-ttu-id="2e654-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e654-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e654-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e654-127">Request body</span></span>
<span data-ttu-id="2e654-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e654-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e654-129">响应</span><span class="sxs-lookup"><span data-stu-id="2e654-129">Response</span></span>

<span data-ttu-id="2e654-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2e654-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e654-132">示例</span><span class="sxs-lookup"><span data-stu-id="2e654-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e654-133">请求</span><span class="sxs-lookup"><span data-stu-id="2e654-133">Request</span></span>
<span data-ttu-id="2e654-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e654-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e654-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e654-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
# <a name="c"></a>[<span data-ttu-id="2e654-136">C#</span><span class="sxs-lookup"><span data-stu-id="2e654-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e654-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e654-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e654-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e654-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e654-139">响应</span><span class="sxs-lookup"><span data-stu-id="2e654-139">Response</span></span>
<span data-ttu-id="2e654-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2e654-140">Here is an example of the response.</span></span> 
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


