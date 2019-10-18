---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c7bf5eef63921f1cc3fab985f4832177767fe1fc
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036072"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="c2aec-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2aec-103">attachment resource type</span></span>

<span data-ttu-id="c2aec-104">可以附件形式向用户[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="c2aec-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="c2aec-105">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="c2aec-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="c2aec-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="c2aec-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="c2aec-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="c2aec-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="c2aec-108">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="c2aec-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="c2aec-109">组日历中的事件不支持附件。</span><span class="sxs-lookup"><span data-stu-id="c2aec-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="c2aec-110">方法</span><span class="sxs-lookup"><span data-stu-id="c2aec-110">Methods</span></span>

<span data-ttu-id="c2aec-111">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="c2aec-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="c2aec-112">方法</span><span class="sxs-lookup"><span data-stu-id="c2aec-112">Method</span></span>       | <span data-ttu-id="c2aec-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2aec-113">Return Type</span></span>  |<span data-ttu-id="c2aec-114">说明</span><span class="sxs-lookup"><span data-stu-id="c2aec-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2aec-115">获取附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="c2aec-116">attachment</span><span class="sxs-lookup"><span data-stu-id="c2aec-116">attachment</span></span>](attachment.md) |<span data-ttu-id="c2aec-117">读取附加到事件、邮件或帖子的附件的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="c2aec-117">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="c2aec-118">将附件添加到用户事件中</span><span class="sxs-lookup"><span data-stu-id="c2aec-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="c2aec-119">附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-119">attachment</span></span>](attachment.md) |<span data-ttu-id="c2aec-120">将文件、项目或链接附件添加到用户日历中的事件中。</span><span class="sxs-lookup"><span data-stu-id="c2aec-120">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="c2aec-121">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="c2aec-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="c2aec-122">附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-122">attachment</span></span>](attachment.md) |<span data-ttu-id="c2aec-123">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="c2aec-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="c2aec-124">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="c2aec-124">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="c2aec-125">附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-125">attachment</span></span>](attachment.md) |<span data-ttu-id="c2aec-126">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="c2aec-126">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="c2aec-127">列出用户事件的附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-127">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="c2aec-128">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2aec-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="c2aec-129">获取用户日历中事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="c2aec-129">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="c2aec-130">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-130">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="c2aec-131">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2aec-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="c2aec-132">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="c2aec-132">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="c2aec-133">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="c2aec-133">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="c2aec-134">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2aec-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="c2aec-135">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="c2aec-135">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="c2aec-136">删除</span><span class="sxs-lookup"><span data-stu-id="c2aec-136">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c2aec-137">无</span><span class="sxs-lookup"><span data-stu-id="c2aec-137">None</span></span> |<span data-ttu-id="c2aec-138">删除事件、邮件或帖子的附件。</span><span class="sxs-lookup"><span data-stu-id="c2aec-138">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2aec-139">属性</span><span class="sxs-lookup"><span data-stu-id="c2aec-139">Properties</span></span>

<span data-ttu-id="c2aec-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="c2aec-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="c2aec-142">属性</span><span class="sxs-lookup"><span data-stu-id="c2aec-142">Property</span></span>     | <span data-ttu-id="c2aec-143">类型</span><span class="sxs-lookup"><span data-stu-id="c2aec-143">Type</span></span>   |<span data-ttu-id="c2aec-144">说明</span><span class="sxs-lookup"><span data-stu-id="c2aec-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2aec-145">contentType</span><span class="sxs-lookup"><span data-stu-id="c2aec-145">contentType</span></span>|<span data-ttu-id="c2aec-146">String</span><span class="sxs-lookup"><span data-stu-id="c2aec-146">String</span></span>|<span data-ttu-id="c2aec-147">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="c2aec-147">The MIME type.</span></span>|
|<span data-ttu-id="c2aec-148">id</span><span class="sxs-lookup"><span data-stu-id="c2aec-148">id</span></span>|<span data-ttu-id="c2aec-149">String</span><span class="sxs-lookup"><span data-stu-id="c2aec-149">String</span></span>| <span data-ttu-id="c2aec-150">只读。</span><span class="sxs-lookup"><span data-stu-id="c2aec-150">Read-only.</span></span>|
|<span data-ttu-id="c2aec-151">isInline</span><span class="sxs-lookup"><span data-stu-id="c2aec-151">isInline</span></span>|<span data-ttu-id="c2aec-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2aec-152">Boolean</span></span>|<span data-ttu-id="c2aec-153">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="c2aec-153">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="c2aec-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2aec-154">lastModifiedDateTime</span></span>|<span data-ttu-id="c2aec-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2aec-155">DateTimeOffset</span></span>|<span data-ttu-id="c2aec-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c2aec-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c2aec-158">名称</span><span class="sxs-lookup"><span data-stu-id="c2aec-158">name</span></span>|<span data-ttu-id="c2aec-159">String</span><span class="sxs-lookup"><span data-stu-id="c2aec-159">String</span></span>|<span data-ttu-id="c2aec-160">附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="c2aec-160">The attachment's file name.</span></span>|
|<span data-ttu-id="c2aec-161">size</span><span class="sxs-lookup"><span data-stu-id="c2aec-161">size</span></span>|<span data-ttu-id="c2aec-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c2aec-162">Int32</span></span>|<span data-ttu-id="c2aec-163">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="c2aec-163">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2aec-164">关系</span><span class="sxs-lookup"><span data-stu-id="c2aec-164">Relationships</span></span>
<span data-ttu-id="c2aec-165">无</span><span class="sxs-lookup"><span data-stu-id="c2aec-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2aec-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2aec-166">JSON representation</span></span>

<span data-ttu-id="c2aec-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2aec-167">Here is a JSON representation of the resource</span></span>

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
