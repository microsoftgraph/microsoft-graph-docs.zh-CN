---
title: 'event: tentativelyAccept'
description: 暂时接受用户日历中的指定事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2788977c465a44ac06f89ba84004fb2bcb1da4a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461592"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="3aca6-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="3aca6-103">event: tentativelyAccept</span></span>

<span data-ttu-id="3aca6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aca6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aca6-105">暂时接受用户[日历](../resources/calendar.md)中的指定[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="3aca6-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3aca6-106">权限</span><span class="sxs-lookup"><span data-stu-id="3aca6-106">Permissions</span></span>
<span data-ttu-id="3aca6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3aca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aca6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3aca6-109">Permission type</span></span>      | <span data-ttu-id="3aca6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3aca6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aca6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3aca6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3aca6-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aca6-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3aca6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3aca6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aca6-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aca6-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3aca6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3aca6-115">Application</span></span> | <span data-ttu-id="3aca6-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aca6-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aca6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3aca6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="3aca6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3aca6-118">Request headers</span></span>
| <span data-ttu-id="3aca6-119">名称</span><span class="sxs-lookup"><span data-stu-id="3aca6-119">Name</span></span>       | <span data-ttu-id="3aca6-120">类型</span><span class="sxs-lookup"><span data-stu-id="3aca6-120">Type</span></span> | <span data-ttu-id="3aca6-121">说明</span><span class="sxs-lookup"><span data-stu-id="3aca6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3aca6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aca6-122">Authorization</span></span>  | <span data-ttu-id="3aca6-123">string</span><span class="sxs-lookup"><span data-stu-id="3aca6-123">string</span></span>  | <span data-ttu-id="3aca6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3aca6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aca6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3aca6-126">Content-Type</span></span> | <span data-ttu-id="3aca6-127">string</span><span class="sxs-lookup"><span data-stu-id="3aca6-127">string</span></span>  | <span data-ttu-id="3aca6-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="3aca6-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aca6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3aca6-130">Request body</span></span>
<span data-ttu-id="3aca6-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3aca6-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3aca6-132">参数</span><span class="sxs-lookup"><span data-stu-id="3aca6-132">Parameter</span></span>    | <span data-ttu-id="3aca6-133">类型</span><span class="sxs-lookup"><span data-stu-id="3aca6-133">Type</span></span>   |<span data-ttu-id="3aca6-134">说明</span><span class="sxs-lookup"><span data-stu-id="3aca6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aca6-135">注释</span><span class="sxs-lookup"><span data-stu-id="3aca6-135">comment</span></span>|<span data-ttu-id="3aca6-136">String</span><span class="sxs-lookup"><span data-stu-id="3aca6-136">String</span></span>|<span data-ttu-id="3aca6-p104">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="3aca6-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="3aca6-139">sendResponse</span><span class="sxs-lookup"><span data-stu-id="3aca6-139">sendResponse</span></span>|<span data-ttu-id="3aca6-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3aca6-140">Boolean</span></span>|<span data-ttu-id="3aca6-p105">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="3aca6-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="3aca6-144">响应</span><span class="sxs-lookup"><span data-stu-id="3aca6-144">Response</span></span>

<span data-ttu-id="3aca6-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3aca6-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aca6-147">示例</span><span class="sxs-lookup"><span data-stu-id="3aca6-147">Example</span></span>
<span data-ttu-id="3aca6-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3aca6-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3aca6-149">请求</span><span class="sxs-lookup"><span data-stu-id="3aca6-149">Request</span></span>
<span data-ttu-id="3aca6-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3aca6-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3aca6-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aca6-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="3aca6-152">C#</span><span class="sxs-lookup"><span data-stu-id="3aca6-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aca6-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aca6-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aca6-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aca6-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aca6-155">Java</span><span class="sxs-lookup"><span data-stu-id="3aca6-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3aca6-156">响应</span><span class="sxs-lookup"><span data-stu-id="3aca6-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="3aca6-157">响应</span><span class="sxs-lookup"><span data-stu-id="3aca6-157">Response</span></span>
<span data-ttu-id="3aca6-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3aca6-158">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
