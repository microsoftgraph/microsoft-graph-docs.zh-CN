---
title: Add attachment
description: 使用此 API 新建附件。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e56da5a4b6f57506800e07e3f8e2b09ed7ef6f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824078"
---
# <a name="add-attachment"></a><span data-ttu-id="32b21-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="32b21-103">Add attachment</span></span>

> <span data-ttu-id="32b21-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32b21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32b21-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32b21-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32b21-106">使用此 API 新建附件。</span><span class="sxs-lookup"><span data-stu-id="32b21-106">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="32b21-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="32b21-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="32b21-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="32b21-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="32b21-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="32b21-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="32b21-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="32b21-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="32b21-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="32b21-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="32b21-112">权限</span><span class="sxs-lookup"><span data-stu-id="32b21-112">Permissions</span></span>
<span data-ttu-id="32b21-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32b21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b21-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="32b21-115">Permission type</span></span>      | <span data-ttu-id="32b21-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32b21-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32b21-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32b21-117">Delegated (work or school account)</span></span> | <span data-ttu-id="32b21-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b21-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32b21-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32b21-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32b21-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b21-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32b21-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="32b21-121">Application</span></span> | <span data-ttu-id="32b21-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32b21-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32b21-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32b21-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="32b21-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="32b21-124">Request headers</span></span>
| <span data-ttu-id="32b21-125">名称</span><span class="sxs-lookup"><span data-stu-id="32b21-125">Name</span></span>       | <span data-ttu-id="32b21-126">类型</span><span class="sxs-lookup"><span data-stu-id="32b21-126">Type</span></span> | <span data-ttu-id="32b21-127">说明</span><span class="sxs-lookup"><span data-stu-id="32b21-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="32b21-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b21-128">Authorization</span></span>  | <span data-ttu-id="32b21-129">string</span><span class="sxs-lookup"><span data-stu-id="32b21-129">string</span></span>  | <span data-ttu-id="32b21-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32b21-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32b21-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32b21-132">Content-Type</span></span> | <span data-ttu-id="32b21-133">string</span><span class="sxs-lookup"><span data-stu-id="32b21-133">string</span></span>  | <span data-ttu-id="32b21-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="32b21-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32b21-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="32b21-136">Request body</span></span>
<span data-ttu-id="32b21-137">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32b21-137">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="32b21-138">响应</span><span class="sxs-lookup"><span data-stu-id="32b21-138">Response</span></span>

<span data-ttu-id="32b21-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32b21-139">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="32b21-140">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="32b21-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="32b21-141">请求</span><span class="sxs-lookup"><span data-stu-id="32b21-141">Request</span></span>
<span data-ttu-id="32b21-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32b21-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="32b21-143">响应</span><span class="sxs-lookup"><span data-stu-id="32b21-143">Response</span></span>
<span data-ttu-id="32b21-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32b21-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="32b21-147">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="32b21-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="32b21-148">请求</span><span class="sxs-lookup"><span data-stu-id="32b21-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="32b21-149">响应</span><span class="sxs-lookup"><span data-stu-id="32b21-149">Response</span></span>
<span data-ttu-id="32b21-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32b21-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
