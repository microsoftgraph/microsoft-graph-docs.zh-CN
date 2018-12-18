---
title: 列出附件
description: 检索附加到事件的 attachment 对象列表。
author: angelgolfer-ms
ms.openlocfilehash: 051ab6fa9b2064ea62606f5d01de540600ed66c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333871"
---
# <a name="list-attachments"></a><span data-ttu-id="01abc-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="01abc-103">List attachments</span></span>

> <span data-ttu-id="01abc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01abc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01abc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01abc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01abc-106">检索附加到事件的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="01abc-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="01abc-107">权限</span><span class="sxs-lookup"><span data-stu-id="01abc-107">Permissions</span></span>
<span data-ttu-id="01abc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01abc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01abc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01abc-110">Permission type</span></span>      | <span data-ttu-id="01abc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01abc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01abc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01abc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01abc-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01abc-113">Calendars.Read</span></span>    |
|<span data-ttu-id="01abc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01abc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01abc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01abc-115">Calendars.Read</span></span>    |
|<span data-ttu-id="01abc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01abc-116">Application</span></span> | <span data-ttu-id="01abc-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01abc-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="01abc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01abc-118">HTTP request</span></span>
<span data-ttu-id="01abc-119">[事件](../resources/event.md)在用户的默认[日历](../resources/calendar.md)中的附件。</span><span class="sxs-lookup"><span data-stu-id="01abc-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="01abc-120">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="01abc-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="01abc-121">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="01abc-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01abc-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01abc-122">Optional query parameters</span></span>
<span data-ttu-id="01abc-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01abc-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="01abc-124">具体而言，您可以使用 $展开查询参数，包括所有事件附件内嵌与事件属性的其余部分。</span><span class="sxs-lookup"><span data-stu-id="01abc-124">In particular, you can use the $expand query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="01abc-125">例如：</span><span class="sxs-lookup"><span data-stu-id="01abc-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```


## <a name="request-headers"></a><span data-ttu-id="01abc-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="01abc-126">Request headers</span></span>
| <span data-ttu-id="01abc-127">Name</span><span class="sxs-lookup"><span data-stu-id="01abc-127">Name</span></span>       | <span data-ttu-id="01abc-128">类型</span><span class="sxs-lookup"><span data-stu-id="01abc-128">Type</span></span> | <span data-ttu-id="01abc-129">说明</span><span class="sxs-lookup"><span data-stu-id="01abc-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01abc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="01abc-130">Authorization</span></span>  | <span data-ttu-id="01abc-131">string</span><span class="sxs-lookup"><span data-stu-id="01abc-131">string</span></span>  | <span data-ttu-id="01abc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01abc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01abc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="01abc-134">Request body</span></span>
<span data-ttu-id="01abc-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01abc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01abc-136">响应</span><span class="sxs-lookup"><span data-stu-id="01abc-136">Response</span></span>

<span data-ttu-id="01abc-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="01abc-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01abc-138">示例</span><span class="sxs-lookup"><span data-stu-id="01abc-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01abc-139">请求</span><span class="sxs-lookup"><span data-stu-id="01abc-139">Request</span></span>
<span data-ttu-id="01abc-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01abc-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="01abc-141">响应</span><span class="sxs-lookup"><span data-stu-id="01abc-141">Response</span></span>
<span data-ttu-id="01abc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01abc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
  "tocPath": ""
}-->