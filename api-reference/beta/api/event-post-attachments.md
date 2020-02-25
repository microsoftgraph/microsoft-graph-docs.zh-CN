---
title: Add attachment
description: 使用此 API 将 附件 添加到事件。 自此处起
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5064c995e1d441d2086432501aa488bd4d4885b5
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268411"
---
# <a name="add-attachment"></a><span data-ttu-id="41a5d-104">添加附件</span><span class="sxs-lookup"><span data-stu-id="41a5d-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41a5d-105">使用此 API 可将[附件](../resources/attachment.md)添加到现有[事件](../resources/event.md)中。</span><span class="sxs-lookup"><span data-stu-id="41a5d-105">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="41a5d-106">此操作将限制可添加到 3 MB 以下的附件的大小。</span><span class="sxs-lookup"><span data-stu-id="41a5d-106">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="41a5d-107">如果组织者将附件添加到会议事件中，则组织者随后可以[更新](event-update.md)事件以发送附件并为每个与会者同时更新事件。</span><span class="sxs-lookup"><span data-stu-id="41a5d-107">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="41a5d-108">权限</span><span class="sxs-lookup"><span data-stu-id="41a5d-108">Permissions</span></span>

<span data-ttu-id="41a5d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41a5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41a5d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41a5d-111">Permission type</span></span>      | <span data-ttu-id="41a5d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41a5d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41a5d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41a5d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="41a5d-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41a5d-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="41a5d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41a5d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41a5d-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41a5d-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="41a5d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41a5d-117">Application</span></span> | <span data-ttu-id="41a5d-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41a5d-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="41a5d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41a5d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="41a5d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41a5d-120">Request headers</span></span>

| <span data-ttu-id="41a5d-121">名称</span><span class="sxs-lookup"><span data-stu-id="41a5d-121">Name</span></span>       | <span data-ttu-id="41a5d-122">类型</span><span class="sxs-lookup"><span data-stu-id="41a5d-122">Type</span></span> | <span data-ttu-id="41a5d-123">说明</span><span class="sxs-lookup"><span data-stu-id="41a5d-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41a5d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="41a5d-124">Authorization</span></span>  | <span data-ttu-id="41a5d-125">string</span><span class="sxs-lookup"><span data-stu-id="41a5d-125">string</span></span>  | <span data-ttu-id="41a5d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41a5d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41a5d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41a5d-128">Content-Type</span></span> | <span data-ttu-id="41a5d-129">string</span><span class="sxs-lookup"><span data-stu-id="41a5d-129">string</span></span>  | <span data-ttu-id="41a5d-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="41a5d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41a5d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="41a5d-132">Request body</span></span>

<span data-ttu-id="41a5d-133">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41a5d-133">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="41a5d-134">响应</span><span class="sxs-lookup"><span data-stu-id="41a5d-134">Response</span></span>

<span data-ttu-id="41a5d-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41a5d-135">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="41a5d-136">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="41a5d-136">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="41a5d-137">请求</span><span class="sxs-lookup"><span data-stu-id="41a5d-137">Request</span></span>

<span data-ttu-id="41a5d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41a5d-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41a5d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="41a5d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```
# <a name="c"></a>[<span data-ttu-id="41a5d-140">C#</span><span class="sxs-lookup"><span data-stu-id="41a5d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41a5d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41a5d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41a5d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41a5d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="41a5d-143">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41a5d-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="41a5d-144">响应</span><span class="sxs-lookup"><span data-stu-id="41a5d-144">Response</span></span>

<span data-ttu-id="41a5d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41a5d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_event_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
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

## <a name="example-item-attachment"></a><span data-ttu-id="41a5d-148">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="41a5d-148">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="41a5d-149">请求</span><span class="sxs-lookup"><span data-stu-id="41a5d-149">Request</span></span>

<span data-ttu-id="41a5d-150">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="41a5d-150">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
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


### <a name="response"></a><span data-ttu-id="41a5d-151">响应</span><span class="sxs-lookup"><span data-stu-id="41a5d-151">Response</span></span>

<span data-ttu-id="41a5d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41a5d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/beta/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="41a5d-155">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="41a5d-155">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="41a5d-156">请求</span><span class="sxs-lookup"><span data-stu-id="41a5d-156">Request</span></span>

<span data-ttu-id="41a5d-157">下面的示例展示了向现有事件添加引用附件的请求。</span><span class="sxs-lookup"><span data-stu-id="41a5d-157">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="41a5d-158">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="41a5d-158">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="41a5d-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="41a5d-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments
Content-type: application/json
Content-length: 319

{
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "name": "Personal pictures",
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    "providerType": "oneDriveConsumer",
    "permission": "Edit",
    "isFolder": "True"
}
```
# <a name="c"></a>[<span data-ttu-id="41a5d-160">C#</span><span class="sxs-lookup"><span data-stu-id="41a5d-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41a5d-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41a5d-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41a5d-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41a5d-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41a5d-163">响应</span><span class="sxs-lookup"><span data-stu-id="41a5d-163">Response</span></span>

<span data-ttu-id="41a5d-164">下面的示例展示了完整的响应。</span><span class="sxs-lookup"><span data-stu-id="41a5d-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
