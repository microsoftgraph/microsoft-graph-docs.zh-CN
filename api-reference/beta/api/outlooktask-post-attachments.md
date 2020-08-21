---
title: 创建附件
description: 使用此 API 将附件添加到 outlookTask。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3dc0ab4e62844bf565cdff834e57ba9843d30873
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849672"
---
# <a name="create-attachment"></a><span data-ttu-id="f0ed7-103">创建附件</span><span class="sxs-lookup"><span data-stu-id="f0ed7-103">Create attachment</span></span>

<span data-ttu-id="f0ed7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0ed7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="f0ed7-105">使用此 API 将附件 [添加到](../resources/attachment.md) [outlookTask](../resources/outlooktask.md)。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="f0ed7-106">附件可以是[fileAttachment](../resources/fileattachment.md) (或 Outlook 项)  ([类型的文件) 。](../resources/itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="f0ed7-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0ed7-107">权限</span><span class="sxs-lookup"><span data-stu-id="f0ed7-107">Permissions</span></span>

<span data-ttu-id="f0ed7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0ed7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0ed7-110">Permission type</span></span>      | <span data-ttu-id="f0ed7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0ed7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0ed7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0ed7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0ed7-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0ed7-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f0ed7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0ed7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ed7-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0ed7-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f0ed7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0ed7-116">Application</span></span> | <span data-ttu-id="f0ed7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0ed7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0ed7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="f0ed7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0ed7-119">Request headers</span></span>

| <span data-ttu-id="f0ed7-120">名称</span><span class="sxs-lookup"><span data-stu-id="f0ed7-120">Name</span></span>       | <span data-ttu-id="f0ed7-121">说明</span><span class="sxs-lookup"><span data-stu-id="f0ed7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0ed7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ed7-122">Authorization</span></span>  | <span data-ttu-id="f0ed7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0ed7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0ed7-125">Content-Type</span></span> | <span data-ttu-id="f0ed7-126">一个表示实体正文中数据类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="f0ed7-127">必需。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0ed7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0ed7-128">Request body</span></span>

<span data-ttu-id="f0ed7-129">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f0ed7-130">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed7-130">Response</span></span>

<span data-ttu-id="f0ed7-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0ed7-132">示例</span><span class="sxs-lookup"><span data-stu-id="f0ed7-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="f0ed7-133">示例 1：添加文件附件</span><span class="sxs-lookup"><span data-stu-id="f0ed7-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="f0ed7-134">请求</span><span class="sxs-lookup"><span data-stu-id="f0ed7-134">Request</span></span>

<span data-ttu-id="f0ed7-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0ed7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0ed7-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f0ed7-137">C#</span><span class="sxs-lookup"><span data-stu-id="f0ed7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0ed7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0ed7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0ed7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0ed7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f0ed7-140">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed7-140">Response</span></span>

<span data-ttu-id="f0ed7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="f0ed7-144">示例 2：添加项目附件</span><span class="sxs-lookup"><span data-stu-id="f0ed7-144">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="f0ed7-145">请求</span><span class="sxs-lookup"><span data-stu-id="f0ed7-145">Request</span></span>

<span data-ttu-id="f0ed7-146">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-146">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "ignored",
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


#### <a name="response"></a><span data-ttu-id="f0ed7-147">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed7-147">Response</span></span>

<span data-ttu-id="f0ed7-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0ed7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
