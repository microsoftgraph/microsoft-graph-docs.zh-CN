---
title: 'event: dismissReminder'
description: 消除对用户日历中的事件触发的提醒。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ce95feee0373105151bcc71b8a70907eddf1c656
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015053"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="0814c-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="0814c-103">event: dismissReminder</span></span>

<span data-ttu-id="0814c-104">消除对用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)触发的提醒。</span><span class="sxs-lookup"><span data-stu-id="0814c-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0814c-105">权限</span><span class="sxs-lookup"><span data-stu-id="0814c-105">Permissions</span></span>
<span data-ttu-id="0814c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0814c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0814c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0814c-108">Permission type</span></span>      | <span data-ttu-id="0814c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0814c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0814c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0814c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0814c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0814c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0814c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0814c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0814c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0814c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0814c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0814c-114">Application</span></span> | <span data-ttu-id="0814c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0814c-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0814c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0814c-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="0814c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0814c-117">Request headers</span></span>
| <span data-ttu-id="0814c-118">名称</span><span class="sxs-lookup"><span data-stu-id="0814c-118">Name</span></span>       | <span data-ttu-id="0814c-119">类型</span><span class="sxs-lookup"><span data-stu-id="0814c-119">Type</span></span> | <span data-ttu-id="0814c-120">说明</span><span class="sxs-lookup"><span data-stu-id="0814c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0814c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0814c-121">Authorization</span></span>  | <span data-ttu-id="0814c-122">string</span><span class="sxs-lookup"><span data-stu-id="0814c-122">string</span></span>  | <span data-ttu-id="0814c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0814c-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="0814c-125">响应</span><span class="sxs-lookup"><span data-stu-id="0814c-125">Response</span></span>

<span data-ttu-id="0814c-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0814c-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0814c-128">示例</span><span class="sxs-lookup"><span data-stu-id="0814c-128">Example</span></span>

<span data-ttu-id="0814c-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0814c-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0814c-130">请求</span><span class="sxs-lookup"><span data-stu-id="0814c-130">Request</span></span>
<span data-ttu-id="0814c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0814c-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0814c-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0814c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0814c-133">C#</span><span class="sxs-lookup"><span data-stu-id="0814c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0814c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0814c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0814c-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="0814c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0814c-136">Java</span><span class="sxs-lookup"><span data-stu-id="0814c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-dismissreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

### <a name="response"></a><span data-ttu-id="0814c-137">响应</span><span class="sxs-lookup"><span data-stu-id="0814c-137">Response</span></span>
<span data-ttu-id="0814c-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0814c-138">Here is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
