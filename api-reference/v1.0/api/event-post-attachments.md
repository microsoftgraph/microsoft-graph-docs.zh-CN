---
title: Add attachment
description: 使用此 API 将 附件 添加到事件。 自此处起
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3022351924e779facb6b9bda3bda04d0cae66ecc
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461743"
---
# <a name="add-attachment"></a><span data-ttu-id="5f576-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="5f576-104">Add attachment</span></span>

<span data-ttu-id="5f576-p102">使用此 API 将 [附件](../resources/attachment.md) 添加到事件。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="5f576-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f576-107">权限</span><span class="sxs-lookup"><span data-stu-id="5f576-107">Permissions</span></span>
<span data-ttu-id="5f576-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f576-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f576-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f576-110">Permission type</span></span>      | <span data-ttu-id="5f576-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f576-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f576-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f576-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5f576-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f576-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f576-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f576-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f576-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f576-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f576-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f576-116">Application</span></span> | <span data-ttu-id="5f576-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f576-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f576-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f576-118">HTTP request</span></span>
<span data-ttu-id="5f576-119">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="5f576-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="5f576-120">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="5f576-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="5f576-121">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="5f576-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="5f576-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f576-122">Request headers</span></span>
| <span data-ttu-id="5f576-123">名称</span><span class="sxs-lookup"><span data-stu-id="5f576-123">Name</span></span>       | <span data-ttu-id="5f576-124">类型</span><span class="sxs-lookup"><span data-stu-id="5f576-124">Type</span></span> | <span data-ttu-id="5f576-125">说明</span><span class="sxs-lookup"><span data-stu-id="5f576-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f576-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f576-126">Authorization</span></span>  | <span data-ttu-id="5f576-127">string</span><span class="sxs-lookup"><span data-stu-id="5f576-127">string</span></span>  | <span data-ttu-id="5f576-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f576-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f576-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f576-130">Content-Type</span></span> | <span data-ttu-id="5f576-131">string</span><span class="sxs-lookup"><span data-stu-id="5f576-131">string</span></span>  | <span data-ttu-id="5f576-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="5f576-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f576-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f576-134">Request body</span></span>
<span data-ttu-id="5f576-135">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f576-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f576-136">响应</span><span class="sxs-lookup"><span data-stu-id="5f576-136">Response</span></span>

<span data-ttu-id="5f576-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f576-137">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="5f576-138">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="5f576-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5f576-139">请求</span><span class="sxs-lookup"><span data-stu-id="5f576-139">Request</span></span>
<span data-ttu-id="5f576-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f576-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5f576-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5f576-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f576-142">C#</span><span class="sxs-lookup"><span data-stu-id="5f576-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f576-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f576-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f576-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="5f576-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5f576-145">Java</span><span class="sxs-lookup"><span data-stu-id="5f576-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5f576-146">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f576-146">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="5f576-147">响应</span><span class="sxs-lookup"><span data-stu-id="5f576-147">Response</span></span>
<span data-ttu-id="5f576-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5f576-148">Here is an example of the response.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="5f576-149">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="5f576-149">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5f576-150">请求</span><span class="sxs-lookup"><span data-stu-id="5f576-150">Request</span></span>

<span data-ttu-id="5f576-151">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="5f576-151">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


##### <a name="response"></a><span data-ttu-id="5f576-152">响应</span><span class="sxs-lookup"><span data-stu-id="5f576-152">Response</span></span>
<span data-ttu-id="5f576-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5f576-153">Here is an example of the response.</span></span>
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
