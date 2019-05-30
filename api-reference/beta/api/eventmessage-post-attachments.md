---
title: Add attachment
description: 使用此 API 新建附件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0540769e0cda600eecdf14016adc4de3a27f7400
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536272"
---
# <a name="add-attachment"></a><span data-ttu-id="7cde1-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="7cde1-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cde1-104">使用此 API 新建附件。</span><span class="sxs-lookup"><span data-stu-id="7cde1-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="7cde1-105">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="7cde1-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="7cde1-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="7cde1-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="7cde1-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="7cde1-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="7cde1-108">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="7cde1-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="7cde1-109">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="7cde1-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7cde1-110">权限</span><span class="sxs-lookup"><span data-stu-id="7cde1-110">Permissions</span></span>
<span data-ttu-id="7cde1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cde1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cde1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cde1-113">Permission type</span></span>      | <span data-ttu-id="7cde1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cde1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cde1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cde1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7cde1-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7cde1-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7cde1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cde1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cde1-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7cde1-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7cde1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cde1-119">Application</span></span> | <span data-ttu-id="7cde1-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7cde1-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cde1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cde1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="7cde1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cde1-122">Request headers</span></span>
| <span data-ttu-id="7cde1-123">名称</span><span class="sxs-lookup"><span data-stu-id="7cde1-123">Name</span></span>       | <span data-ttu-id="7cde1-124">类型</span><span class="sxs-lookup"><span data-stu-id="7cde1-124">Type</span></span> | <span data-ttu-id="7cde1-125">说明</span><span class="sxs-lookup"><span data-stu-id="7cde1-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7cde1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cde1-126">Authorization</span></span>  | <span data-ttu-id="7cde1-127">string</span><span class="sxs-lookup"><span data-stu-id="7cde1-127">string</span></span>  | <span data-ttu-id="7cde1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7cde1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7cde1-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7cde1-130">Content-Type</span></span> | <span data-ttu-id="7cde1-131">string</span><span class="sxs-lookup"><span data-stu-id="7cde1-131">string</span></span>  | <span data-ttu-id="7cde1-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="7cde1-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cde1-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cde1-134">Request body</span></span>
<span data-ttu-id="7cde1-135">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cde1-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7cde1-136">响应</span><span class="sxs-lookup"><span data-stu-id="7cde1-136">Response</span></span>

<span data-ttu-id="7cde1-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7cde1-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="7cde1-138">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="7cde1-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="7cde1-139">请求</span><span class="sxs-lookup"><span data-stu-id="7cde1-139">Request</span></span>
<span data-ttu-id="7cde1-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7cde1-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7cde1-141">响应</span><span class="sxs-lookup"><span data-stu-id="7cde1-141">Response</span></span>
<span data-ttu-id="7cde1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7cde1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7cde1-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7cde1-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7cde1-146">C#</span><span class="sxs-lookup"><span data-stu-id="7cde1-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7cde1-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="7cde1-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="example-item-attachment"></a><span data-ttu-id="7cde1-148">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="7cde1-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="7cde1-149">请求</span><span class="sxs-lookup"><span data-stu-id="7cde1-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="7cde1-150">响应</span><span class="sxs-lookup"><span data-stu-id="7cde1-150">Response</span></span>
<span data-ttu-id="7cde1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7cde1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7cde1-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7cde1-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7cde1-155">C#</span><span class="sxs-lookup"><span data-stu-id="7cde1-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7cde1-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="7cde1-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
