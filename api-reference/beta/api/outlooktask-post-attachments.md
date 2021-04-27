---
title: 创建附件
description: 使用此 API 将附件添加到 outlookTask。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fd4dbe34759372629ccb0cb76feef2c13fa096ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055468"
---
# <a name="create-attachment-deprecated"></a><span data-ttu-id="baa8f-103">创建 (的附件) </span><span class="sxs-lookup"><span data-stu-id="baa8f-103">Create attachment (deprecated)</span></span>

<span data-ttu-id="baa8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baa8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="baa8f-105">使用此 API 将附件 [添加到](../resources/attachment.md) [outlookTask](../resources/outlooktask.md)。</span><span class="sxs-lookup"><span data-stu-id="baa8f-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="baa8f-106">附件可以是[fileAttachment](../resources/fileattachment.md) (类型的文件，) Outlook [itemAttachment (itemAttachment](../resources/itemattachment.md)) 。</span><span class="sxs-lookup"><span data-stu-id="baa8f-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="baa8f-107">权限</span><span class="sxs-lookup"><span data-stu-id="baa8f-107">Permissions</span></span>

<span data-ttu-id="baa8f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baa8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baa8f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="baa8f-110">Permission type</span></span>      | <span data-ttu-id="baa8f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baa8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baa8f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baa8f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="baa8f-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baa8f-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="baa8f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baa8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baa8f-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baa8f-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="baa8f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="baa8f-116">Application</span></span> | <span data-ttu-id="baa8f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="baa8f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="baa8f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baa8f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="baa8f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="baa8f-119">Request headers</span></span>

| <span data-ttu-id="baa8f-120">名称</span><span class="sxs-lookup"><span data-stu-id="baa8f-120">Name</span></span>       | <span data-ttu-id="baa8f-121">说明</span><span class="sxs-lookup"><span data-stu-id="baa8f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="baa8f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="baa8f-122">Authorization</span></span>  | <span data-ttu-id="baa8f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="baa8f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="baa8f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="baa8f-125">Content-Type</span></span> | <span data-ttu-id="baa8f-126">表示实体正文中数据类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="baa8f-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="baa8f-127">必需。</span><span class="sxs-lookup"><span data-stu-id="baa8f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baa8f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="baa8f-128">Request body</span></span>

<span data-ttu-id="baa8f-129">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baa8f-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="baa8f-130">响应</span><span class="sxs-lookup"><span data-stu-id="baa8f-130">Response</span></span>

<span data-ttu-id="baa8f-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="baa8f-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="baa8f-132">示例</span><span class="sxs-lookup"><span data-stu-id="baa8f-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="baa8f-133">示例 1：添加文件附件</span><span class="sxs-lookup"><span data-stu-id="baa8f-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="baa8f-134">请求</span><span class="sxs-lookup"><span data-stu-id="baa8f-134">Request</span></span>

<span data-ttu-id="baa8f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="baa8f-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="baa8f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="baa8f-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="baa8f-137">C#</span><span class="sxs-lookup"><span data-stu-id="baa8f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="baa8f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="baa8f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="baa8f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="baa8f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="baa8f-140">Java</span><span class="sxs-lookup"><span data-stu-id="baa8f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-file-attachment-to-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="baa8f-141">响应</span><span class="sxs-lookup"><span data-stu-id="baa8f-141">Response</span></span>

<span data-ttu-id="baa8f-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="baa8f-142">Here is an example of the response.</span></span> <span data-ttu-id="baa8f-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="baa8f-143">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="baa8f-144">示例 2：添加项目附件</span><span class="sxs-lookup"><span data-stu-id="baa8f-144">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="baa8f-145">请求</span><span class="sxs-lookup"><span data-stu-id="baa8f-145">Request</span></span>

<span data-ttu-id="baa8f-146">下面将一个事件附加到另一个事件作为项目附件的示例。</span><span class="sxs-lookup"><span data-stu-id="baa8f-146">Here is an example which attaches an event with another event as an item attachment.</span></span>


# <a name="http"></a>[<span data-ttu-id="baa8f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="baa8f-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="baa8f-148">C#</span><span class="sxs-lookup"><span data-stu-id="baa8f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-item-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="baa8f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="baa8f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-item-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="baa8f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="baa8f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-item-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="baa8f-151">Java</span><span class="sxs-lookup"><span data-stu-id="baa8f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-item-attachment-to-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="baa8f-152">响应</span><span class="sxs-lookup"><span data-stu-id="baa8f-152">Response</span></span>

<span data-ttu-id="baa8f-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="baa8f-153">Here is an example of the response.</span></span> <span data-ttu-id="baa8f-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="baa8f-154">Note: The response object shown here might be shortened for readability.</span></span>
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


