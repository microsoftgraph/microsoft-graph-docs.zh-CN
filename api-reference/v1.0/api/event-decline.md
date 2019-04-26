---
title: 'event: decline'
description: 拒绝用户日历中的指定事件邀请。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 920a97db9a6716d2111a8179c86d5556042a6edd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550091"
---
# <a name="event-decline"></a><span data-ttu-id="789ee-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="789ee-103">event: decline</span></span>

<span data-ttu-id="789ee-104">拒绝对用户[日历](../resources/calendar.md)中指定[事件](../resources/event.md)的邀请。</span><span class="sxs-lookup"><span data-stu-id="789ee-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="789ee-105">权限</span><span class="sxs-lookup"><span data-stu-id="789ee-105">Permissions</span></span>

<span data-ttu-id="789ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="789ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789ee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="789ee-108">Permission type</span></span>      | <span data-ttu-id="789ee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="789ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="789ee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="789ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="789ee-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="789ee-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="789ee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="789ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="789ee-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="789ee-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="789ee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="789ee-114">Application</span></span> | <span data-ttu-id="789ee-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="789ee-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="789ee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="789ee-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="789ee-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="789ee-117">Request headers</span></span>

| <span data-ttu-id="789ee-118">名称</span><span class="sxs-lookup"><span data-stu-id="789ee-118">Name</span></span>       | <span data-ttu-id="789ee-119">类型</span><span class="sxs-lookup"><span data-stu-id="789ee-119">Type</span></span> | <span data-ttu-id="789ee-120">说明</span><span class="sxs-lookup"><span data-stu-id="789ee-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="789ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="789ee-121">Authorization</span></span>  | <span data-ttu-id="789ee-122">string</span><span class="sxs-lookup"><span data-stu-id="789ee-122">string</span></span>  | <span data-ttu-id="789ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="789ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="789ee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="789ee-125">Content-Type</span></span> | <span data-ttu-id="789ee-126">string</span><span class="sxs-lookup"><span data-stu-id="789ee-126">string</span></span>  | <span data-ttu-id="789ee-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="789ee-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="789ee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="789ee-129">Request body</span></span>

<span data-ttu-id="789ee-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="789ee-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="789ee-131">参数</span><span class="sxs-lookup"><span data-stu-id="789ee-131">Parameter</span></span>    | <span data-ttu-id="789ee-132">类型</span><span class="sxs-lookup"><span data-stu-id="789ee-132">Type</span></span>   |<span data-ttu-id="789ee-133">说明</span><span class="sxs-lookup"><span data-stu-id="789ee-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="789ee-134">注释</span><span class="sxs-lookup"><span data-stu-id="789ee-134">comment</span></span>|<span data-ttu-id="789ee-135">String</span><span class="sxs-lookup"><span data-stu-id="789ee-135">String</span></span>|<span data-ttu-id="789ee-p104">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="789ee-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="789ee-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="789ee-138">sendResponse</span></span>|<span data-ttu-id="789ee-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="789ee-139">Boolean</span></span>|<span data-ttu-id="789ee-p105">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="789ee-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="789ee-143">响应</span><span class="sxs-lookup"><span data-stu-id="789ee-143">Response</span></span>

<span data-ttu-id="789ee-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="789ee-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="789ee-146">示例</span><span class="sxs-lookup"><span data-stu-id="789ee-146">Example</span></span>

<span data-ttu-id="789ee-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="789ee-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="789ee-148">请求</span><span class="sxs-lookup"><span data-stu-id="789ee-148">Request</span></span>

<span data-ttu-id="789ee-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="789ee-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="789ee-150">响应</span><span class="sxs-lookup"><span data-stu-id="789ee-150">Response</span></span>

<span data-ttu-id="789ee-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="789ee-151">Here is an example of the response.</span></span>

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
