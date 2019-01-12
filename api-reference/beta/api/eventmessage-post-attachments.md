---
title: Add attachment
description: 使用此 API 新建附件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d2e2de9e8e7e328f2e0cabc1df8fdf7dcd7b4856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965913"
---
# <a name="add-attachment"></a><span data-ttu-id="84dcd-103">Add attachment</span><span class="sxs-lookup"><span data-stu-id="84dcd-103">Add attachment</span></span>

> <span data-ttu-id="84dcd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84dcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84dcd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84dcd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84dcd-106">使用此 API 新建附件。</span><span class="sxs-lookup"><span data-stu-id="84dcd-106">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="84dcd-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="84dcd-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="84dcd-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="84dcd-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="84dcd-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="84dcd-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="84dcd-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="84dcd-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="84dcd-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="84dcd-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="84dcd-112">权限</span><span class="sxs-lookup"><span data-stu-id="84dcd-112">Permissions</span></span>
<span data-ttu-id="84dcd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84dcd-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="84dcd-115">Permission type</span></span>      | <span data-ttu-id="84dcd-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84dcd-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84dcd-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84dcd-117">Delegated (work or school account)</span></span> | <span data-ttu-id="84dcd-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84dcd-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="84dcd-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84dcd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84dcd-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84dcd-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="84dcd-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="84dcd-121">Application</span></span> | <span data-ttu-id="84dcd-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84dcd-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="84dcd-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84dcd-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="84dcd-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="84dcd-124">Request headers</span></span>
| <span data-ttu-id="84dcd-125">名称</span><span class="sxs-lookup"><span data-stu-id="84dcd-125">Name</span></span>       | <span data-ttu-id="84dcd-126">类型</span><span class="sxs-lookup"><span data-stu-id="84dcd-126">Type</span></span> | <span data-ttu-id="84dcd-127">说明</span><span class="sxs-lookup"><span data-stu-id="84dcd-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84dcd-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="84dcd-128">Authorization</span></span>  | <span data-ttu-id="84dcd-129">string</span><span class="sxs-lookup"><span data-stu-id="84dcd-129">string</span></span>  | <span data-ttu-id="84dcd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84dcd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84dcd-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84dcd-132">Content-Type</span></span> | <span data-ttu-id="84dcd-133">string</span><span class="sxs-lookup"><span data-stu-id="84dcd-133">string</span></span>  | <span data-ttu-id="84dcd-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="84dcd-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84dcd-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="84dcd-136">Request body</span></span>
<span data-ttu-id="84dcd-137">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84dcd-137">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="84dcd-138">响应</span><span class="sxs-lookup"><span data-stu-id="84dcd-138">Response</span></span>

<span data-ttu-id="84dcd-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84dcd-139">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="84dcd-140">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="84dcd-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="84dcd-141">请求</span><span class="sxs-lookup"><span data-stu-id="84dcd-141">Request</span></span>
<span data-ttu-id="84dcd-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84dcd-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="84dcd-143">响应</span><span class="sxs-lookup"><span data-stu-id="84dcd-143">Response</span></span>
<span data-ttu-id="84dcd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84dcd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="84dcd-147">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="84dcd-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="84dcd-148">请求</span><span class="sxs-lookup"><span data-stu-id="84dcd-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="84dcd-149">响应</span><span class="sxs-lookup"><span data-stu-id="84dcd-149">Response</span></span>
<span data-ttu-id="84dcd-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84dcd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
