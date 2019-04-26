---
title: Add attachment
description: 使用此 API 将 附件 添加到事件。 由于存在
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 583959b227afccaf52b5951aa4270523bccd1dc1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324336"
---
# <a name="add-attachment"></a><span data-ttu-id="57479-104">Add attachment</span><span class="sxs-lookup"><span data-stu-id="57479-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57479-p102">使用此 API 将 [附件](../resources/attachment.md) 添加到事件。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="57479-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="57479-107">权限</span><span class="sxs-lookup"><span data-stu-id="57479-107">Permissions</span></span>

<span data-ttu-id="57479-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57479-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57479-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57479-110">Permission type</span></span>      | <span data-ttu-id="57479-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57479-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57479-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57479-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57479-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57479-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="57479-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57479-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57479-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57479-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="57479-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57479-116">Application</span></span> | <span data-ttu-id="57479-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57479-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="57479-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57479-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="57479-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="57479-119">Request headers</span></span>

| <span data-ttu-id="57479-120">名称</span><span class="sxs-lookup"><span data-stu-id="57479-120">Name</span></span>       | <span data-ttu-id="57479-121">类型</span><span class="sxs-lookup"><span data-stu-id="57479-121">Type</span></span> | <span data-ttu-id="57479-122">说明</span><span class="sxs-lookup"><span data-stu-id="57479-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57479-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57479-123">Authorization</span></span>  | <span data-ttu-id="57479-124">string</span><span class="sxs-lookup"><span data-stu-id="57479-124">string</span></span>  | <span data-ttu-id="57479-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57479-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57479-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57479-127">Content-Type</span></span> | <span data-ttu-id="57479-128">string</span><span class="sxs-lookup"><span data-stu-id="57479-128">string</span></span>  | <span data-ttu-id="57479-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="57479-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57479-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="57479-131">Request body</span></span>

<span data-ttu-id="57479-132">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57479-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57479-133">响应</span><span class="sxs-lookup"><span data-stu-id="57479-133">Response</span></span>

<span data-ttu-id="57479-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57479-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="57479-135">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="57479-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="57479-136">请求</span><span class="sxs-lookup"><span data-stu-id="57479-136">Request</span></span>

<span data-ttu-id="57479-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57479-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
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

<span data-ttu-id="57479-138">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57479-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="57479-139">响应</span><span class="sxs-lookup"><span data-stu-id="57479-139">Response</span></span>

<span data-ttu-id="57479-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57479-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
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

## <a name="example-item-attachment"></a><span data-ttu-id="57479-143">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="57479-143">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="57479-144">请求</span><span class="sxs-lookup"><span data-stu-id="57479-144">Request</span></span>

<span data-ttu-id="57479-145">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="57479-145">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

### <a name="response"></a><span data-ttu-id="57479-146">响应</span><span class="sxs-lookup"><span data-stu-id="57479-146">Response</span></span>

<span data-ttu-id="57479-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57479-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
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

## <a name="example-reference-attachment"></a><span data-ttu-id="57479-150">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="57479-150">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="57479-151">请求</span><span class="sxs-lookup"><span data-stu-id="57479-151">Request</span></span>

<span data-ttu-id="57479-152">下面的示例展示了向现有事件添加引用附件的请求。</span><span class="sxs-lookup"><span data-stu-id="57479-152">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="57479-153">附件指向 OneDrive 上的文件夹。</span><span class="sxs-lookup"><span data-stu-id="57479-153">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
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

### <a name="response"></a><span data-ttu-id="57479-154">响应</span><span class="sxs-lookup"><span data-stu-id="57479-154">Response</span></span>

<span data-ttu-id="57479-155">下面的示例展示了完整的响应。</span><span class="sxs-lookup"><span data-stu-id="57479-155">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
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
  "tocPath": "",
  "suppressions": [
    "Error: create_file_attachment_from_event/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='"
  ]
}
-->
