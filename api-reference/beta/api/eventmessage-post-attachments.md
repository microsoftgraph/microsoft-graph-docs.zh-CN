---
title: Add attachment
description: 使用此 API 新建附件。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 713a1f8e4abdf23d9278d5616ba1aca326d9286c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042357"
---
# <a name="add-attachment"></a><span data-ttu-id="26b70-103">添加附件</span><span class="sxs-lookup"><span data-stu-id="26b70-103">Add attachment</span></span>

<span data-ttu-id="26b70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b70-105">使用此 API 新建附件。</span><span class="sxs-lookup"><span data-stu-id="26b70-105">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="26b70-106">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="26b70-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="26b70-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="26b70-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="26b70-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="26b70-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="26b70-109">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="26b70-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="26b70-110">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="26b70-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="26b70-111">权限</span><span class="sxs-lookup"><span data-stu-id="26b70-111">Permissions</span></span>
<span data-ttu-id="26b70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26b70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b70-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="26b70-114">Permission type</span></span>      | <span data-ttu-id="26b70-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26b70-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26b70-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26b70-116">Delegated (work or school account)</span></span> | <span data-ttu-id="26b70-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b70-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="26b70-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26b70-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b70-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b70-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="26b70-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="26b70-120">Application</span></span> | <span data-ttu-id="26b70-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b70-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26b70-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26b70-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="26b70-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="26b70-123">Request headers</span></span>
| <span data-ttu-id="26b70-124">名称</span><span class="sxs-lookup"><span data-stu-id="26b70-124">Name</span></span>       | <span data-ttu-id="26b70-125">类型</span><span class="sxs-lookup"><span data-stu-id="26b70-125">Type</span></span> | <span data-ttu-id="26b70-126">说明</span><span class="sxs-lookup"><span data-stu-id="26b70-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26b70-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b70-127">Authorization</span></span>  | <span data-ttu-id="26b70-128">string</span><span class="sxs-lookup"><span data-stu-id="26b70-128">string</span></span>  | <span data-ttu-id="26b70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26b70-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26b70-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26b70-131">Content-Type</span></span> | <span data-ttu-id="26b70-132">string</span><span class="sxs-lookup"><span data-stu-id="26b70-132">string</span></span>  | <span data-ttu-id="26b70-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="26b70-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26b70-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="26b70-135">Request body</span></span>
<span data-ttu-id="26b70-136">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26b70-136">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26b70-137">响应</span><span class="sxs-lookup"><span data-stu-id="26b70-137">Response</span></span>

<span data-ttu-id="26b70-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="26b70-138">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="26b70-139">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="26b70-139">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="26b70-140">请求</span><span class="sxs-lookup"><span data-stu-id="26b70-140">Request</span></span>
<span data-ttu-id="26b70-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26b70-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26b70-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b70-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```
# <a name="c"></a>[<span data-ttu-id="26b70-143">C#</span><span class="sxs-lookup"><span data-stu-id="26b70-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b70-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b70-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b70-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b70-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26b70-146">Java</span><span class="sxs-lookup"><span data-stu-id="26b70-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26b70-147">响应</span><span class="sxs-lookup"><span data-stu-id="26b70-147">Response</span></span>
<span data-ttu-id="26b70-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26b70-148">Here is an example of the response.</span></span> <span data-ttu-id="26b70-149">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="26b70-149">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="26b70-150">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="26b70-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="26b70-151">请求</span><span class="sxs-lookup"><span data-stu-id="26b70-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="26b70-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b70-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": {
    "@odata.type": "microsoft.graph.message"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="26b70-153">C#</span><span class="sxs-lookup"><span data-stu-id="26b70-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b70-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b70-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b70-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b70-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26b70-156">Java</span><span class="sxs-lookup"><span data-stu-id="26b70-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26b70-157">响应</span><span class="sxs-lookup"><span data-stu-id="26b70-157">Response</span></span>
<span data-ttu-id="26b70-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26b70-158">Here is an example of the response.</span></span> <span data-ttu-id="26b70-159">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="26b70-159">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
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
  ]
}
-->


