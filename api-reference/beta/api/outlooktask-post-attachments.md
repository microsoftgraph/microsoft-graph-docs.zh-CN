---
title: 创建附件
description: 使用此 API 可将附件添加到 outlookTask。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4f9386e680bb344055c62063232d5a8603fe42f
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994706"
---
# <a name="create-attachment"></a><span data-ttu-id="4dfac-103">创建附件</span><span class="sxs-lookup"><span data-stu-id="4dfac-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dfac-104">使用此 API 可将[附件](../resources/attachment.md)添加到[outlookTask](../resources/outlooktask.md)。</span><span class="sxs-lookup"><span data-stu-id="4dfac-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="4dfac-105">附件可以是文件（ [fileAttachment](../resources/fileattachment.md)类型）或 Outlook 项目（[itemAttachment](../resources/itemattachment.md)类型）。</span><span class="sxs-lookup"><span data-stu-id="4dfac-105">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="4dfac-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4dfac-106">Permissions</span></span>

<span data-ttu-id="4dfac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dfac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dfac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dfac-109">Permission type</span></span>      | <span data-ttu-id="4dfac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dfac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dfac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dfac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4dfac-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dfac-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4dfac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dfac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dfac-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dfac-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4dfac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dfac-115">Application</span></span> | <span data-ttu-id="4dfac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dfac-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dfac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dfac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="4dfac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dfac-118">Request headers</span></span>

| <span data-ttu-id="4dfac-119">名称</span><span class="sxs-lookup"><span data-stu-id="4dfac-119">Name</span></span>       | <span data-ttu-id="4dfac-120">说明</span><span class="sxs-lookup"><span data-stu-id="4dfac-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4dfac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dfac-121">Authorization</span></span>  | <span data-ttu-id="4dfac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4dfac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4dfac-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4dfac-124">Content-Type</span></span> | <span data-ttu-id="4dfac-125">一个字符串，表示实体的正文中的数据类型。</span><span class="sxs-lookup"><span data-stu-id="4dfac-125">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="4dfac-126">必需。</span><span class="sxs-lookup"><span data-stu-id="4dfac-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dfac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dfac-127">Request body</span></span>

<span data-ttu-id="4dfac-128">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dfac-128">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4dfac-129">响应</span><span class="sxs-lookup"><span data-stu-id="4dfac-129">Response</span></span>

<span data-ttu-id="4dfac-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dfac-130">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4dfac-131">示例</span><span class="sxs-lookup"><span data-stu-id="4dfac-131">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="4dfac-132">示例1：添加文件附件</span><span class="sxs-lookup"><span data-stu-id="4dfac-132">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="4dfac-133">请求</span><span class="sxs-lookup"><span data-stu-id="4dfac-133">Request</span></span>

<span data-ttu-id="4dfac-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4dfac-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_file_attachment_to_task"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

#### <a name="response"></a><span data-ttu-id="4dfac-135">响应</span><span class="sxs-lookup"><span data-stu-id="4dfac-135">Response</span></span>

<span data-ttu-id="4dfac-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dfac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "add_file_attachment_to_task",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP 201 Created

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/outlook/tasks('AAMkADAAAANXbdnAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "text/plain",
    "id": "AAMkADAAAANXbdnAAABEgAQAKQF4_X0QwVHpmAmxUgHN_Q=",
    "lastModifiedDateTime": "2020-01-07T22:13:30Z",
    "name": "menu.txt",
    "contentType": "text/plain",
    "size": 178,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="4dfac-139">示例2：添加项目附件</span><span class="sxs-lookup"><span data-stu-id="4dfac-139">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4dfac-140">请求</span><span class="sxs-lookup"><span data-stu-id="4dfac-140">Request</span></span>

<span data-ttu-id="4dfac-141">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="4dfac-141">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_item_attachment_to_task"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments
Content-type: application/json

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
             "dateTime": "2020-01-12T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2020-01-12T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```


#### <a name="response"></a><span data-ttu-id="4dfac-142">响应</span><span class="sxs-lookup"><span data-stu-id="4dfac-142">Response</span></span>

<span data-ttu-id="4dfac-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dfac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "add_item_attachment_to_task",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/outlook/tasks('AAMkADAAAANXbdnAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.itemAttachment",
    "id": "AAMkADAAAANXbdnAAABEgAQANgBvaZHiKVMskpdj1k9KEQ=",
    "lastModifiedDateTime": "2020-01-07T22:18:11Z",
    "name": "Holiday event",
    "contentType": null,
    "size": 2067,
    "isInline": false
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
