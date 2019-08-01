---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d47fde49a76f00658e39d9a3ae6629cd9bcf56b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030070"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="4a0f7-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a0f7-103">attachment resource type</span></span>

<span data-ttu-id="4a0f7-104">可以附件形式向[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="4a0f7-105">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="4a0f7-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="4a0f7-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="4a0f7-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="4a0f7-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="4a0f7-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="4a0f7-108">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="4a0f7-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="4a0f7-109">方法</span><span class="sxs-lookup"><span data-stu-id="4a0f7-109">Methods</span></span>

<span data-ttu-id="4a0f7-110">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="4a0f7-111">方法</span><span class="sxs-lookup"><span data-stu-id="4a0f7-111">Method</span></span>       | <span data-ttu-id="4a0f7-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a0f7-112">Return Type</span></span>  |<span data-ttu-id="4a0f7-113">说明</span><span class="sxs-lookup"><span data-stu-id="4a0f7-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a0f7-114">获取附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="4a0f7-115">attachment</span><span class="sxs-lookup"><span data-stu-id="4a0f7-115">attachment</span></span>](attachment.md) |<span data-ttu-id="4a0f7-116">读取附加到事件、邮件或帖子的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-116">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="4a0f7-117">Add attachment to an event</span><span class="sxs-lookup"><span data-stu-id="4a0f7-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="4a0f7-118">附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-118">attachment</span></span>](attachment.md) |<span data-ttu-id="4a0f7-119">将文件、项目或链接附件添加到事件中。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="4a0f7-120">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="4a0f7-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="4a0f7-121">附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-121">attachment</span></span>](attachment.md) |<span data-ttu-id="4a0f7-122">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="4a0f7-123">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="4a0f7-123">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="4a0f7-124">附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-124">attachment</span></span>](attachment.md) |<span data-ttu-id="4a0f7-125">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-125">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="4a0f7-126">列出事件的附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-126">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="4a0f7-127">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a0f7-127">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4a0f7-128">获取事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-128">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="4a0f7-129">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-129">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="4a0f7-130">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a0f7-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4a0f7-131">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-131">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="4a0f7-132">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="4a0f7-132">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="4a0f7-133">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a0f7-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="4a0f7-134">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-134">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="4a0f7-135">删除</span><span class="sxs-lookup"><span data-stu-id="4a0f7-135">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4a0f7-136">无</span><span class="sxs-lookup"><span data-stu-id="4a0f7-136">None</span></span> |<span data-ttu-id="4a0f7-137">删除事件、邮件或帖子的附件。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-137">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a0f7-138">属性</span><span class="sxs-lookup"><span data-stu-id="4a0f7-138">Properties</span></span>

<span data-ttu-id="4a0f7-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="4a0f7-141">属性</span><span class="sxs-lookup"><span data-stu-id="4a0f7-141">Property</span></span>     | <span data-ttu-id="4a0f7-142">类型</span><span class="sxs-lookup"><span data-stu-id="4a0f7-142">Type</span></span>   |<span data-ttu-id="4a0f7-143">说明</span><span class="sxs-lookup"><span data-stu-id="4a0f7-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a0f7-144">contentType</span><span class="sxs-lookup"><span data-stu-id="4a0f7-144">contentType</span></span>|<span data-ttu-id="4a0f7-145">String</span><span class="sxs-lookup"><span data-stu-id="4a0f7-145">String</span></span>|<span data-ttu-id="4a0f7-146">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-146">The MIME type.</span></span>|
|<span data-ttu-id="4a0f7-147">id</span><span class="sxs-lookup"><span data-stu-id="4a0f7-147">id</span></span>|<span data-ttu-id="4a0f7-148">String</span><span class="sxs-lookup"><span data-stu-id="4a0f7-148">String</span></span>| <span data-ttu-id="4a0f7-149">只读。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-149">Read-only.</span></span>|
|<span data-ttu-id="4a0f7-150">isInline</span><span class="sxs-lookup"><span data-stu-id="4a0f7-150">isInline</span></span>|<span data-ttu-id="4a0f7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a0f7-151">Boolean</span></span>|<span data-ttu-id="4a0f7-152">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-152">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="4a0f7-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a0f7-153">lastModifiedDateTime</span></span>|<span data-ttu-id="4a0f7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a0f7-154">DateTimeOffset</span></span>|<span data-ttu-id="4a0f7-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4a0f7-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4a0f7-157">名称</span><span class="sxs-lookup"><span data-stu-id="4a0f7-157">name</span></span>|<span data-ttu-id="4a0f7-158">String</span><span class="sxs-lookup"><span data-stu-id="4a0f7-158">String</span></span>|<span data-ttu-id="4a0f7-159">附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-159">The attachment's file name.</span></span>|
|<span data-ttu-id="4a0f7-160">size</span><span class="sxs-lookup"><span data-stu-id="4a0f7-160">size</span></span>|<span data-ttu-id="4a0f7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4a0f7-161">Int32</span></span>|<span data-ttu-id="4a0f7-162">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-162">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a0f7-163">关系</span><span class="sxs-lookup"><span data-stu-id="4a0f7-163">Relationships</span></span>
<span data-ttu-id="4a0f7-164">无</span><span class="sxs-lookup"><span data-stu-id="4a0f7-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a0f7-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a0f7-165">JSON representation</span></span>

<span data-ttu-id="4a0f7-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a0f7-166">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
