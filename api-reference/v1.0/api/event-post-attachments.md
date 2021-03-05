---
title: Add attachment
description: 使用此 API 将 附件 添加到事件。 自此处起
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 14d62182f4d21618dae5d8009c4376404fff66eb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473815"
---
# <a name="add-attachment"></a><span data-ttu-id="888b3-104">添加附件</span><span class="sxs-lookup"><span data-stu-id="888b3-104">Add attachment</span></span>

<span data-ttu-id="888b3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="888b3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="888b3-106">使用此 API 将附件 [添加到](../resources/attachment.md) 现有 [事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="888b3-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="888b3-107">此操作将可添加到的附件大小限制在 3 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="888b3-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="888b3-108">如果组织者向会议事件添加附件，组织者随后可以更新事件以发送附件[](event-update.md)并更新每个与会者的事件。</span><span class="sxs-lookup"><span data-stu-id="888b3-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="888b3-109">权限</span><span class="sxs-lookup"><span data-stu-id="888b3-109">Permissions</span></span>
<span data-ttu-id="888b3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="888b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="888b3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="888b3-112">Permission type</span></span>      | <span data-ttu-id="888b3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="888b3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="888b3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="888b3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="888b3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="888b3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="888b3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="888b3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="888b3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="888b3-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="888b3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="888b3-118">Application</span></span> | <span data-ttu-id="888b3-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="888b3-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="888b3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="888b3-120">HTTP request</span></span>
<span data-ttu-id="888b3-121">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="888b3-121">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="888b3-122">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="888b3-122">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="888b3-123">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="888b3-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="888b3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="888b3-124">Request headers</span></span>
| <span data-ttu-id="888b3-125">名称</span><span class="sxs-lookup"><span data-stu-id="888b3-125">Name</span></span>       | <span data-ttu-id="888b3-126">类型</span><span class="sxs-lookup"><span data-stu-id="888b3-126">Type</span></span> | <span data-ttu-id="888b3-127">说明</span><span class="sxs-lookup"><span data-stu-id="888b3-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="888b3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="888b3-128">Authorization</span></span>  | <span data-ttu-id="888b3-129">string</span><span class="sxs-lookup"><span data-stu-id="888b3-129">string</span></span>  | <span data-ttu-id="888b3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="888b3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="888b3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="888b3-132">Content-Type</span></span> | <span data-ttu-id="888b3-133">string</span><span class="sxs-lookup"><span data-stu-id="888b3-133">string</span></span>  | <span data-ttu-id="888b3-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="888b3-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="888b3-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="888b3-136">Request body</span></span>
<span data-ttu-id="888b3-137">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="888b3-137">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="888b3-138">响应</span><span class="sxs-lookup"><span data-stu-id="888b3-138">Response</span></span>

<span data-ttu-id="888b3-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="888b3-139">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="888b3-140">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="888b3-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="888b3-141">请求</span><span class="sxs-lookup"><span data-stu-id="888b3-141">Request</span></span>
<span data-ttu-id="888b3-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="888b3-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="888b3-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="888b3-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event_v1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```
# <a name="c"></a>[<span data-ttu-id="888b3-144">C#</span><span class="sxs-lookup"><span data-stu-id="888b3-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="888b3-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="888b3-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="888b3-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="888b3-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="888b3-147">Java</span><span class="sxs-lookup"><span data-stu-id="888b3-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="888b3-148">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="888b3-148">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="888b3-149">响应</span><span class="sxs-lookup"><span data-stu-id="888b3-149">Response</span></span>
<span data-ttu-id="888b3-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="888b3-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_event_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="888b3-151">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="888b3-151">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="888b3-152">请求</span><span class="sxs-lookup"><span data-stu-id="888b3-152">Request</span></span>

<span data-ttu-id="888b3-153">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="888b3-153">Here is an example which attaches an event with another event as an item attachment.</span></span>


# <a name="http"></a>[<span data-ttu-id="888b3-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="888b3-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 600

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
        "@odata.type": "microsoft.graph.event",
        "subject": "Discuss gifts for children",
        "body": {
            "contentType": "HTML",
            "content": "Let's look for funding!"
         },
         "start": {
             "dateTime": "2016-12-02T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2016-12-02T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="888b3-155">C#</span><span class="sxs-lookup"><span data-stu-id="888b3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="888b3-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="888b3-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="888b3-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="888b3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="888b3-158">Java</span><span class="sxs-lookup"><span data-stu-id="888b3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="888b3-159">响应</span><span class="sxs-lookup"><span data-stu-id="888b3-159">Response</span></span>
<span data-ttu-id="888b3-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="888b3-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

