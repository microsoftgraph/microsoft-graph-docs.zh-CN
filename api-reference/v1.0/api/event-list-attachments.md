---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e324d67cd6e7c57d3a936a0ec6d6e9ace3ec5df0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039585"
---
# <a name="list-attachments"></a><span data-ttu-id="97500-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="97500-103">List attachments</span></span>

<span data-ttu-id="97500-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97500-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97500-105">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="97500-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="97500-106">权限</span><span class="sxs-lookup"><span data-stu-id="97500-106">Permissions</span></span>
<span data-ttu-id="97500-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97500-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97500-109">Permission type</span></span>      | <span data-ttu-id="97500-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97500-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97500-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97500-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97500-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97500-112">Calendars.Read</span></span>    |
|<span data-ttu-id="97500-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97500-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97500-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97500-114">Calendars.Read</span></span>    |
|<span data-ttu-id="97500-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97500-115">Application</span></span> | <span data-ttu-id="97500-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97500-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="97500-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97500-117">HTTP request</span></span>
<span data-ttu-id="97500-118">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="97500-118">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="97500-119">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="97500-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="97500-120">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="97500-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97500-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97500-121">Optional query parameters</span></span>
<span data-ttu-id="97500-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97500-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97500-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="97500-123">Request headers</span></span>
| <span data-ttu-id="97500-124">名称</span><span class="sxs-lookup"><span data-stu-id="97500-124">Name</span></span>       | <span data-ttu-id="97500-125">类型</span><span class="sxs-lookup"><span data-stu-id="97500-125">Type</span></span> | <span data-ttu-id="97500-126">说明</span><span class="sxs-lookup"><span data-stu-id="97500-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97500-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="97500-127">Authorization</span></span>  | <span data-ttu-id="97500-128">string</span><span class="sxs-lookup"><span data-stu-id="97500-128">string</span></span>  | <span data-ttu-id="97500-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97500-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97500-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="97500-131">Request body</span></span>
<span data-ttu-id="97500-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97500-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97500-133">响应</span><span class="sxs-lookup"><span data-stu-id="97500-133">Response</span></span>

<span data-ttu-id="97500-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="97500-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97500-135">示例</span><span class="sxs-lookup"><span data-stu-id="97500-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97500-136">请求</span><span class="sxs-lookup"><span data-stu-id="97500-136">Request</span></span>
<span data-ttu-id="97500-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97500-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97500-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="97500-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="97500-139">C#</span><span class="sxs-lookup"><span data-stu-id="97500-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97500-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97500-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97500-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97500-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97500-142">Java</span><span class="sxs-lookup"><span data-stu-id="97500-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97500-143">响应</span><span class="sxs-lookup"><span data-stu-id="97500-143">Response</span></span>
<span data-ttu-id="97500-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97500-144">Here is an example of the response.</span></span> <span data-ttu-id="97500-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="97500-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
