---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b83ede390c5fa9846afefba0ef76da4216505aa0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615207"
---
# <a name="list-attachments"></a><span data-ttu-id="24399-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="24399-103">List attachments</span></span>

<span data-ttu-id="24399-104">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="24399-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="24399-105">权限</span><span class="sxs-lookup"><span data-stu-id="24399-105">Permissions</span></span>
<span data-ttu-id="24399-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24399-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="24399-108">Permission type</span></span>      | <span data-ttu-id="24399-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24399-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24399-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24399-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24399-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24399-111">Calendars.Read</span></span>    |
|<span data-ttu-id="24399-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24399-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24399-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24399-113">Calendars.Read</span></span>    |
|<span data-ttu-id="24399-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="24399-114">Application</span></span> | <span data-ttu-id="24399-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24399-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="24399-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24399-116">HTTP request</span></span>
<span data-ttu-id="24399-117">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="24399-117">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="24399-118">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="24399-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="24399-119">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="24399-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24399-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="24399-120">Optional query parameters</span></span>
<span data-ttu-id="24399-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="24399-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="24399-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="24399-122">Request headers</span></span>
| <span data-ttu-id="24399-123">名称</span><span class="sxs-lookup"><span data-stu-id="24399-123">Name</span></span>       | <span data-ttu-id="24399-124">类型</span><span class="sxs-lookup"><span data-stu-id="24399-124">Type</span></span> | <span data-ttu-id="24399-125">说明</span><span class="sxs-lookup"><span data-stu-id="24399-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="24399-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="24399-126">Authorization</span></span>  | <span data-ttu-id="24399-127">string</span><span class="sxs-lookup"><span data-stu-id="24399-127">string</span></span>  | <span data-ttu-id="24399-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24399-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24399-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="24399-130">Request body</span></span>
<span data-ttu-id="24399-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24399-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24399-132">响应</span><span class="sxs-lookup"><span data-stu-id="24399-132">Response</span></span>

<span data-ttu-id="24399-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="24399-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24399-134">示例</span><span class="sxs-lookup"><span data-stu-id="24399-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24399-135">请求</span><span class="sxs-lookup"><span data-stu-id="24399-135">Request</span></span>
<span data-ttu-id="24399-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24399-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="24399-137">响应</span><span class="sxs-lookup"><span data-stu-id="24399-137">Response</span></span>
<span data-ttu-id="24399-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24399-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
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
      "contentBytes": "base64-contentBytes-value",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="24399-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="24399-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24399-142">语言</span><span class="sxs-lookup"><span data-stu-id="24399-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24399-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="24399-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
