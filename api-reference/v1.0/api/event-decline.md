---
title: 'event: decline'
description: 拒绝邀请用户日历中指定的事件。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: c96e04bfc3547d1ff4323fbba3e4d2cde527095e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806200"
---
# <a name="event-decline"></a><span data-ttu-id="cf5cf-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="cf5cf-103">event: decline</span></span>

<span data-ttu-id="cf5cf-104">拒绝邀请用户[日历](../resources/calendar.md)中指定的[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf5cf-105">权限</span><span class="sxs-lookup"><span data-stu-id="cf5cf-105">Permissions</span></span>

<span data-ttu-id="cf5cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5cf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf5cf-108">Permission type</span></span>      | <span data-ttu-id="cf5cf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf5cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf5cf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf5cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf5cf-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf5cf-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cf5cf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf5cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf5cf-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf5cf-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cf5cf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf5cf-114">Application</span></span> | <span data-ttu-id="cf5cf-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf5cf-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf5cf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf5cf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="cf5cf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf5cf-117">Request headers</span></span>

| <span data-ttu-id="cf5cf-118">名称</span><span class="sxs-lookup"><span data-stu-id="cf5cf-118">Name</span></span>       | <span data-ttu-id="cf5cf-119">类型</span><span class="sxs-lookup"><span data-stu-id="cf5cf-119">Type</span></span> | <span data-ttu-id="cf5cf-120">说明</span><span class="sxs-lookup"><span data-stu-id="cf5cf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf5cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf5cf-121">Authorization</span></span>  | <span data-ttu-id="cf5cf-122">string</span><span class="sxs-lookup"><span data-stu-id="cf5cf-122">string</span></span>  | <span data-ttu-id="cf5cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf5cf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf5cf-125">Content-Type</span></span> | <span data-ttu-id="cf5cf-126">string</span><span class="sxs-lookup"><span data-stu-id="cf5cf-126">string</span></span>  | <span data-ttu-id="cf5cf-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf5cf-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf5cf-129">Request body</span></span>

<span data-ttu-id="cf5cf-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf5cf-131">参数</span><span class="sxs-lookup"><span data-stu-id="cf5cf-131">Parameter</span></span>    | <span data-ttu-id="cf5cf-132">类型</span><span class="sxs-lookup"><span data-stu-id="cf5cf-132">Type</span></span>   |<span data-ttu-id="cf5cf-133">说明</span><span class="sxs-lookup"><span data-stu-id="cf5cf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf5cf-134">注释</span><span class="sxs-lookup"><span data-stu-id="cf5cf-134">comment</span></span>|<span data-ttu-id="cf5cf-135">String</span><span class="sxs-lookup"><span data-stu-id="cf5cf-135">String</span></span>|<span data-ttu-id="cf5cf-p104">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="cf5cf-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="cf5cf-138">sendResponse</span></span>|<span data-ttu-id="cf5cf-139">布尔</span><span class="sxs-lookup"><span data-stu-id="cf5cf-139">Boolean</span></span>|<span data-ttu-id="cf5cf-p105">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="cf5cf-143">响应</span><span class="sxs-lookup"><span data-stu-id="cf5cf-143">Response</span></span>

<span data-ttu-id="cf5cf-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf5cf-146">示例</span><span class="sxs-lookup"><span data-stu-id="cf5cf-146">Example</span></span>

<span data-ttu-id="cf5cf-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cf5cf-148">请求</span><span class="sxs-lookup"><span data-stu-id="cf5cf-148">Request</span></span>

<span data-ttu-id="cf5cf-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

<br/>

### <a name="response"></a><span data-ttu-id="cf5cf-150">响应</span><span class="sxs-lookup"><span data-stu-id="cf5cf-150">Response</span></span>

<span data-ttu-id="cf5cf-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cf5cf-151">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
