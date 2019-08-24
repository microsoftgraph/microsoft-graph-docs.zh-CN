---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: da7e66d1edbda224fe547b7e7afc8fd88dc5e5aa
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622633"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="2fbe3-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fbe3-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fbe3-104">可以使用附件的形式向用户[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或组[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="2fbe3-105">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="2fbe3-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="2fbe3-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="2fbe3-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="2fbe3-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="2fbe3-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="2fbe3-108">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="2fbe3-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="2fbe3-109">组日历中的事件不支持附件。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="2fbe3-110">方法</span><span class="sxs-lookup"><span data-stu-id="2fbe3-110">Methods</span></span>

<span data-ttu-id="2fbe3-111">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="2fbe3-112">方法</span><span class="sxs-lookup"><span data-stu-id="2fbe3-112">Method</span></span>       | <span data-ttu-id="2fbe3-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="2fbe3-113">Return Type</span></span>  |<span data-ttu-id="2fbe3-114">说明</span><span class="sxs-lookup"><span data-stu-id="2fbe3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2fbe3-115">获取附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="2fbe3-116">attachment</span><span class="sxs-lookup"><span data-stu-id="2fbe3-116">attachment</span></span>](attachment.md) |<span data-ttu-id="2fbe3-117">读取附加到用户事件、邮件、Outlook 任务或帖子的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-117">Read the properties and relationships of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="2fbe3-118">向用户事件添加附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="2fbe3-119">attachment</span><span class="sxs-lookup"><span data-stu-id="2fbe3-119">attachment</span></span>](attachment.md) |<span data-ttu-id="2fbe3-120">将文件、项目或链接附件添加到用户日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-120">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="2fbe3-121">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="2fbe3-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="2fbe3-122">附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-122">attachment</span></span>](attachment.md) |<span data-ttu-id="2fbe3-123">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="2fbe3-124">将附件添加到 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="2fbe3-124">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="2fbe3-125">attachment</span><span class="sxs-lookup"><span data-stu-id="2fbe3-125">attachment</span></span>](attachment.md) |<span data-ttu-id="2fbe3-126">将文件、项目或链接附件添加到 Outlook 任务中。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-126">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="2fbe3-127">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="2fbe3-127">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="2fbe3-128">附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-128">attachment</span></span>](attachment.md) |<span data-ttu-id="2fbe3-129">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-129">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="2fbe3-130">列出用户事件的附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-130">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="2fbe3-131">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fbe3-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fbe3-132">获取用户日历中的事件附件的列表。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-132">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="2fbe3-133">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-133">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="2fbe3-134">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fbe3-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fbe3-135">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-135">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="2fbe3-136">列出 Outlook 任务的附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-136">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="2fbe3-137">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fbe3-137">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fbe3-138">获取 Outlook 任务的附件列表。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-138">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="2fbe3-139">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="2fbe3-139">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="2fbe3-140">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fbe3-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fbe3-141">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-141">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="2fbe3-142">删除</span><span class="sxs-lookup"><span data-stu-id="2fbe3-142">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="2fbe3-143">无</span><span class="sxs-lookup"><span data-stu-id="2fbe3-143">None</span></span> |<span data-ttu-id="2fbe3-144">删除事件、邮件、Outlook 任务或帖子上的附件。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-144">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="2fbe3-145">属性</span><span class="sxs-lookup"><span data-stu-id="2fbe3-145">Properties</span></span>

<span data-ttu-id="2fbe3-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="2fbe3-148">属性</span><span class="sxs-lookup"><span data-stu-id="2fbe3-148">Property</span></span>     | <span data-ttu-id="2fbe3-149">类型</span><span class="sxs-lookup"><span data-stu-id="2fbe3-149">Type</span></span>   |<span data-ttu-id="2fbe3-150">说明</span><span class="sxs-lookup"><span data-stu-id="2fbe3-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fbe3-151">contentType</span><span class="sxs-lookup"><span data-stu-id="2fbe3-151">contentType</span></span>|<span data-ttu-id="2fbe3-152">String</span><span class="sxs-lookup"><span data-stu-id="2fbe3-152">String</span></span>|<span data-ttu-id="2fbe3-153">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-153">The MIME type.</span></span>|
|<span data-ttu-id="2fbe3-154">id</span><span class="sxs-lookup"><span data-stu-id="2fbe3-154">id</span></span>|<span data-ttu-id="2fbe3-155">String</span><span class="sxs-lookup"><span data-stu-id="2fbe3-155">String</span></span>| <span data-ttu-id="2fbe3-156">只读。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-156">Read-only.</span></span>|
|<span data-ttu-id="2fbe3-157">isInline</span><span class="sxs-lookup"><span data-stu-id="2fbe3-157">isInline</span></span>|<span data-ttu-id="2fbe3-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fbe3-158">Boolean</span></span>|<span data-ttu-id="2fbe3-159">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-159">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="2fbe3-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fbe3-160">lastModifiedDateTime</span></span>|<span data-ttu-id="2fbe3-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fbe3-161">DateTimeOffset</span></span>|<span data-ttu-id="2fbe3-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2fbe3-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2fbe3-164">名称</span><span class="sxs-lookup"><span data-stu-id="2fbe3-164">name</span></span>|<span data-ttu-id="2fbe3-165">字符串</span><span class="sxs-lookup"><span data-stu-id="2fbe3-165">String</span></span>|<span data-ttu-id="2fbe3-166">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-166">The display name of the attachment.</span></span> <span data-ttu-id="2fbe3-167">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-167">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="2fbe3-168">size</span><span class="sxs-lookup"><span data-stu-id="2fbe3-168">size</span></span>|<span data-ttu-id="2fbe3-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2fbe3-169">Int32</span></span>|<span data-ttu-id="2fbe3-170">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-170">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fbe3-171">关系</span><span class="sxs-lookup"><span data-stu-id="2fbe3-171">Relationships</span></span>
<span data-ttu-id="2fbe3-172">无</span><span class="sxs-lookup"><span data-stu-id="2fbe3-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fbe3-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fbe3-173">JSON representation</span></span>

<span data-ttu-id="2fbe3-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fbe3-174">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
