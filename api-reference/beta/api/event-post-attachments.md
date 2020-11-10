---
title: Add attachment
description: 使用此 API 将 附件 添加到事件。 自此处起
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 859060a1c0a67c5b7c30f5dca72432953247c048
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954783"
---
# <a name="add-attachment"></a><span data-ttu-id="5f1bb-104">添加附件</span><span class="sxs-lookup"><span data-stu-id="5f1bb-104">Add attachment</span></span>

<span data-ttu-id="5f1bb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f1bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f1bb-106">使用此 API 可将 [附件](../resources/attachment.md) 添加到现有 [事件](../resources/event.md)中。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="5f1bb-107">此操作将限制可添加到 3 MB 以下的附件的大小。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="5f1bb-108">如果组织者将附件添加到会议事件中，则组织者随后可以 [更新](event-update.md) 事件以发送附件并为每个与会者同时更新事件。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f1bb-109">权限</span><span class="sxs-lookup"><span data-stu-id="5f1bb-109">Permissions</span></span>

<span data-ttu-id="5f1bb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f1bb-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f1bb-112">Permission type</span></span>      | <span data-ttu-id="5f1bb-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f1bb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f1bb-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f1bb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5f1bb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f1bb-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f1bb-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f1bb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f1bb-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f1bb-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f1bb-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f1bb-118">Application</span></span> | <span data-ttu-id="5f1bb-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f1bb-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f1bb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f1bb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="5f1bb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f1bb-121">Request headers</span></span>

| <span data-ttu-id="5f1bb-122">名称</span><span class="sxs-lookup"><span data-stu-id="5f1bb-122">Name</span></span>       | <span data-ttu-id="5f1bb-123">类型</span><span class="sxs-lookup"><span data-stu-id="5f1bb-123">Type</span></span> | <span data-ttu-id="5f1bb-124">说明</span><span class="sxs-lookup"><span data-stu-id="5f1bb-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f1bb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f1bb-125">Authorization</span></span>  | <span data-ttu-id="5f1bb-126">string</span><span class="sxs-lookup"><span data-stu-id="5f1bb-126">string</span></span>  | <span data-ttu-id="5f1bb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f1bb-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f1bb-129">Content-Type</span></span> | <span data-ttu-id="5f1bb-130">string</span><span class="sxs-lookup"><span data-stu-id="5f1bb-130">string</span></span>  | <span data-ttu-id="5f1bb-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f1bb-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f1bb-133">Request body</span></span>

<span data-ttu-id="5f1bb-134">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f1bb-135">响应</span><span class="sxs-lookup"><span data-stu-id="5f1bb-135">Response</span></span>

<span data-ttu-id="5f1bb-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-136">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="5f1bb-137">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="5f1bb-137">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="5f1bb-138">请求</span><span class="sxs-lookup"><span data-stu-id="5f1bb-138">Request</span></span>

<span data-ttu-id="5f1bb-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f1bb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1bb-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5f1bb-141">C#</span><span class="sxs-lookup"><span data-stu-id="5f1bb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f1bb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f1bb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f1bb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f1bb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f1bb-144">Java</span><span class="sxs-lookup"><span data-stu-id="5f1bb-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5f1bb-145">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-145">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="5f1bb-146">响应</span><span class="sxs-lookup"><span data-stu-id="5f1bb-146">Response</span></span>

<span data-ttu-id="5f1bb-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="5f1bb-150">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="5f1bb-150">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="5f1bb-151">请求</span><span class="sxs-lookup"><span data-stu-id="5f1bb-151">Request</span></span>

<span data-ttu-id="5f1bb-152">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-152">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


### <a name="response"></a><span data-ttu-id="5f1bb-153">响应</span><span class="sxs-lookup"><span data-stu-id="5f1bb-153">Response</span></span>

<span data-ttu-id="5f1bb-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="5f1bb-157">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="5f1bb-157">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="5f1bb-158">请求</span><span class="sxs-lookup"><span data-stu-id="5f1bb-158">Request</span></span>

<span data-ttu-id="5f1bb-159">下面的示例展示了向现有事件添加引用附件的请求。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-159">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="5f1bb-160">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-160">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f1bb-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1bb-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5f1bb-162">C#</span><span class="sxs-lookup"><span data-stu-id="5f1bb-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f1bb-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f1bb-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f1bb-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f1bb-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f1bb-165">Java</span><span class="sxs-lookup"><span data-stu-id="5f1bb-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f1bb-166">响应</span><span class="sxs-lookup"><span data-stu-id="5f1bb-166">Response</span></span>

<span data-ttu-id="5f1bb-167">下面的示例展示了完整的响应。</span><span class="sxs-lookup"><span data-stu-id="5f1bb-167">Here is an example of a full response.</span></span>
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


