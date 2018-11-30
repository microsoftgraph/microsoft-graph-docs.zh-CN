---
title: 'event: decline'
description: 拒绝邀请用户日历中指定的事件。
ms.openlocfilehash: 7012644f28dd6e1172ba8f71b58d6905fe62c1d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043254"
---
# <a name="event-decline"></a><span data-ttu-id="f2c33-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="f2c33-103">event: decline</span></span>

> <span data-ttu-id="f2c33-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f2c33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2c33-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2c33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2c33-106">拒绝邀请用户[日历](../resources/calendar.md)中指定的[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="f2c33-106">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c33-107">权限</span><span class="sxs-lookup"><span data-stu-id="f2c33-107">Permissions</span></span>
<span data-ttu-id="f2c33-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2c33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c33-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2c33-110">Permission type</span></span>      | <span data-ttu-id="f2c33-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2c33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c33-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2c33-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c33-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f2c33-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2c33-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c33-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f2c33-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2c33-116">Application</span></span> | <span data-ttu-id="f2c33-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c33-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2c33-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2c33-118">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="f2c33-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2c33-119">Request headers</span></span>

| <span data-ttu-id="f2c33-120">名称</span><span class="sxs-lookup"><span data-stu-id="f2c33-120">Name</span></span>       | <span data-ttu-id="f2c33-121">类型</span><span class="sxs-lookup"><span data-stu-id="f2c33-121">Type</span></span> | <span data-ttu-id="f2c33-122">说明</span><span class="sxs-lookup"><span data-stu-id="f2c33-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2c33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2c33-123">Authorization</span></span>  | <span data-ttu-id="f2c33-124">string</span><span class="sxs-lookup"><span data-stu-id="f2c33-124">string</span></span>  | <span data-ttu-id="f2c33-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2c33-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2c33-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2c33-127">Content-Type</span></span> | <span data-ttu-id="f2c33-128">string</span><span class="sxs-lookup"><span data-stu-id="f2c33-128">string</span></span>  | <span data-ttu-id="f2c33-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f2c33-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2c33-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2c33-131">Request body</span></span>

<span data-ttu-id="f2c33-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f2c33-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f2c33-133">参数</span><span class="sxs-lookup"><span data-stu-id="f2c33-133">Parameter</span></span>    | <span data-ttu-id="f2c33-134">类型</span><span class="sxs-lookup"><span data-stu-id="f2c33-134">Type</span></span>   |<span data-ttu-id="f2c33-135">说明</span><span class="sxs-lookup"><span data-stu-id="f2c33-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2c33-136">注释</span><span class="sxs-lookup"><span data-stu-id="f2c33-136">comment</span></span>|<span data-ttu-id="f2c33-137">String</span><span class="sxs-lookup"><span data-stu-id="f2c33-137">String</span></span>|<span data-ttu-id="f2c33-p105">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="f2c33-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="f2c33-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="f2c33-140">sendResponse</span></span>|<span data-ttu-id="f2c33-141">布尔</span><span class="sxs-lookup"><span data-stu-id="f2c33-141">Boolean</span></span>|<span data-ttu-id="f2c33-p106">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="f2c33-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="f2c33-145">响应</span><span class="sxs-lookup"><span data-stu-id="f2c33-145">Response</span></span>

<span data-ttu-id="f2c33-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f2c33-p107">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2c33-148">示例</span><span class="sxs-lookup"><span data-stu-id="f2c33-148">Example</span></span>

<span data-ttu-id="f2c33-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f2c33-149">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f2c33-150">请求</span><span class="sxs-lookup"><span data-stu-id="f2c33-150">Request</span></span>

<span data-ttu-id="f2c33-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2c33-151">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

### <a name="response"></a><span data-ttu-id="f2c33-152">响应</span><span class="sxs-lookup"><span data-stu-id="f2c33-152">Response</span></span>

<span data-ttu-id="f2c33-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2c33-153">Here is an example of the response.</span></span>

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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
