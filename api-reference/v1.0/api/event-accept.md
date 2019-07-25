---
title: 'event: accept'
description: 接受用户日历中的指定事件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2f8f33ff835a99d3a72c55bbcc95ea53db1fd51b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887480"
---
# <a name="event-accept"></a><span data-ttu-id="882cd-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="882cd-103">event: accept</span></span>

<span data-ttu-id="882cd-104">接受用户[日历](../resources/calendar.md)中的指定[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="882cd-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="882cd-105">权限</span><span class="sxs-lookup"><span data-stu-id="882cd-105">Permissions</span></span>
<span data-ttu-id="882cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="882cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="882cd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="882cd-108">Permission type</span></span>      | <span data-ttu-id="882cd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="882cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="882cd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="882cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="882cd-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="882cd-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="882cd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="882cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="882cd-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="882cd-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="882cd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="882cd-114">Application</span></span> | <span data-ttu-id="882cd-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="882cd-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="882cd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="882cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="882cd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="882cd-117">Request headers</span></span>
| <span data-ttu-id="882cd-118">名称</span><span class="sxs-lookup"><span data-stu-id="882cd-118">Name</span></span>       | <span data-ttu-id="882cd-119">类型</span><span class="sxs-lookup"><span data-stu-id="882cd-119">Type</span></span> | <span data-ttu-id="882cd-120">说明</span><span class="sxs-lookup"><span data-stu-id="882cd-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="882cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="882cd-121">Authorization</span></span>  | <span data-ttu-id="882cd-122">string</span><span class="sxs-lookup"><span data-stu-id="882cd-122">string</span></span>  | <span data-ttu-id="882cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="882cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="882cd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="882cd-125">Content-Type</span></span> | <span data-ttu-id="882cd-126">string</span><span class="sxs-lookup"><span data-stu-id="882cd-126">string</span></span>  | <span data-ttu-id="882cd-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="882cd-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="882cd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="882cd-129">Request body</span></span>
<span data-ttu-id="882cd-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="882cd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="882cd-131">参数</span><span class="sxs-lookup"><span data-stu-id="882cd-131">Parameter</span></span>    | <span data-ttu-id="882cd-132">类型</span><span class="sxs-lookup"><span data-stu-id="882cd-132">Type</span></span>   |<span data-ttu-id="882cd-133">说明</span><span class="sxs-lookup"><span data-stu-id="882cd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="882cd-134">注释</span><span class="sxs-lookup"><span data-stu-id="882cd-134">comment</span></span>|<span data-ttu-id="882cd-135">String</span><span class="sxs-lookup"><span data-stu-id="882cd-135">String</span></span>|<span data-ttu-id="882cd-p104">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="882cd-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="882cd-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="882cd-138">sendResponse</span></span>|<span data-ttu-id="882cd-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="882cd-139">Boolean</span></span>|<span data-ttu-id="882cd-p105">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="882cd-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="882cd-143">响应</span><span class="sxs-lookup"><span data-stu-id="882cd-143">Response</span></span>

<span data-ttu-id="882cd-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="882cd-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="882cd-146">示例</span><span class="sxs-lookup"><span data-stu-id="882cd-146">Example</span></span>
<span data-ttu-id="882cd-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="882cd-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="882cd-148">请求</span><span class="sxs-lookup"><span data-stu-id="882cd-148">Request</span></span>
<span data-ttu-id="882cd-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="882cd-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="882cd-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="882cd-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="882cd-151">C#</span><span class="sxs-lookup"><span data-stu-id="882cd-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-accept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="882cd-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="882cd-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-accept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="882cd-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="882cd-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-accept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="882cd-154">Java</span><span class="sxs-lookup"><span data-stu-id="882cd-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-accept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="882cd-155">响应</span><span class="sxs-lookup"><span data-stu-id="882cd-155">Response</span></span>
<span data-ttu-id="882cd-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="882cd-156">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
