---
title: attachment 资源类型
description: 您可以将相关的内容添加到事件，
localization_priority: Normal
ms.openlocfilehash: 5648194b0f636c8757d1b20c492abc099dce377d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842789"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="d4587-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4587-103">attachment resource type</span></span>

> <span data-ttu-id="d4587-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4587-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4587-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4587-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4587-106">您可以将相关的内容添加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或附件的形式[发布](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="d4587-106">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="d4587-107">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="d4587-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="d4587-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="d4587-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="d4587-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="d4587-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="d4587-110">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="d4587-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="d4587-111">方法</span><span class="sxs-lookup"><span data-stu-id="d4587-111">Methods</span></span>

<span data-ttu-id="d4587-112">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="d4587-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="d4587-113">方法</span><span class="sxs-lookup"><span data-stu-id="d4587-113">Method</span></span>       | <span data-ttu-id="d4587-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4587-114">Return Type</span></span>  |<span data-ttu-id="d4587-115">说明</span><span class="sxs-lookup"><span data-stu-id="d4587-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4587-116">获取附件</span><span class="sxs-lookup"><span data-stu-id="d4587-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="d4587-117">attachment</span><span class="sxs-lookup"><span data-stu-id="d4587-117">attachment</span></span>](attachment.md) |<span data-ttu-id="d4587-118">读取的属性和附件，附加到事件、 邮件、 Outlook 任务或公告的关系。</span><span class="sxs-lookup"><span data-stu-id="d4587-118">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="d4587-119">Add attachment to an event</span><span class="sxs-lookup"><span data-stu-id="d4587-119">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="d4587-120">附件</span><span class="sxs-lookup"><span data-stu-id="d4587-120">attachment</span></span>](attachment.md) |<span data-ttu-id="d4587-121">将文件、项目或链接附件添加到事件中。</span><span class="sxs-lookup"><span data-stu-id="d4587-121">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="d4587-122">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="d4587-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="d4587-123">附件</span><span class="sxs-lookup"><span data-stu-id="d4587-123">attachment</span></span>](attachment.md) |<span data-ttu-id="d4587-124">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="d4587-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="d4587-125">将附件添加到 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="d4587-125">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="d4587-126">attachment</span><span class="sxs-lookup"><span data-stu-id="d4587-126">attachment</span></span>](attachment.md) |<span data-ttu-id="d4587-127">添加文件、 项或 Outlook 任务链接附件。</span><span class="sxs-lookup"><span data-stu-id="d4587-127">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="d4587-128">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="d4587-128">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="d4587-129">附件</span><span class="sxs-lookup"><span data-stu-id="d4587-129">attachment</span></span>](attachment.md) |<span data-ttu-id="d4587-130">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="d4587-130">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="d4587-131">列出事件的附件</span><span class="sxs-lookup"><span data-stu-id="d4587-131">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="d4587-132">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4587-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d4587-133">获取事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="d4587-133">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="d4587-134">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="d4587-134">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="d4587-135">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4587-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d4587-136">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="d4587-136">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="d4587-137">Outlook 任务的列出附件</span><span class="sxs-lookup"><span data-stu-id="d4587-137">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="d4587-138">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4587-138">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d4587-139">获取附件 Outlook 任务的列表。</span><span class="sxs-lookup"><span data-stu-id="d4587-139">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="d4587-140">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="d4587-140">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="d4587-141">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4587-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="d4587-142">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="d4587-142">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="d4587-143">删除</span><span class="sxs-lookup"><span data-stu-id="d4587-143">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="d4587-144">无</span><span class="sxs-lookup"><span data-stu-id="d4587-144">None</span></span> |<span data-ttu-id="d4587-145">删除事件、 邮件、 Outlook 任务或公告上的附件。</span><span class="sxs-lookup"><span data-stu-id="d4587-145">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4587-146">属性</span><span class="sxs-lookup"><span data-stu-id="d4587-146">Properties</span></span>

<span data-ttu-id="d4587-p102">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="d4587-p102">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="d4587-149">属性</span><span class="sxs-lookup"><span data-stu-id="d4587-149">Property</span></span>     | <span data-ttu-id="d4587-150">类型</span><span class="sxs-lookup"><span data-stu-id="d4587-150">Type</span></span>   |<span data-ttu-id="d4587-151">说明</span><span class="sxs-lookup"><span data-stu-id="d4587-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4587-152">contentType</span><span class="sxs-lookup"><span data-stu-id="d4587-152">contentType</span></span>|<span data-ttu-id="d4587-153">String</span><span class="sxs-lookup"><span data-stu-id="d4587-153">String</span></span>|<span data-ttu-id="d4587-154">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="d4587-154">The MIME type.</span></span>|
|<span data-ttu-id="d4587-155">id</span><span class="sxs-lookup"><span data-stu-id="d4587-155">id</span></span>|<span data-ttu-id="d4587-156">String</span><span class="sxs-lookup"><span data-stu-id="d4587-156">String</span></span>| <span data-ttu-id="d4587-157">只读。</span><span class="sxs-lookup"><span data-stu-id="d4587-157">Read-only.</span></span>|
|<span data-ttu-id="d4587-158">isInline</span><span class="sxs-lookup"><span data-stu-id="d4587-158">isInline</span></span>|<span data-ttu-id="d4587-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4587-159">Boolean</span></span>|<span data-ttu-id="d4587-160">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="d4587-160">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="d4587-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4587-161">lastModifiedDateTime</span></span>|<span data-ttu-id="d4587-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4587-162">DateTimeOffset</span></span>|<span data-ttu-id="d4587-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d4587-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d4587-165">名称</span><span class="sxs-lookup"><span data-stu-id="d4587-165">name</span></span>|<span data-ttu-id="d4587-166">String</span><span class="sxs-lookup"><span data-stu-id="d4587-166">String</span></span>|<span data-ttu-id="d4587-167">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d4587-167">The display name of the attachment.</span></span> <span data-ttu-id="d4587-168">这不需要是实际的文件名称。</span><span class="sxs-lookup"><span data-stu-id="d4587-168">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="d4587-169">size</span><span class="sxs-lookup"><span data-stu-id="d4587-169">size</span></span>|<span data-ttu-id="d4587-170">Int32</span><span class="sxs-lookup"><span data-stu-id="d4587-170">Int32</span></span>|<span data-ttu-id="d4587-171">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="d4587-171">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4587-172">Relationships</span><span class="sxs-lookup"><span data-stu-id="d4587-172">Relationships</span></span>
<span data-ttu-id="d4587-173">无</span><span class="sxs-lookup"><span data-stu-id="d4587-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4587-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4587-174">JSON representation</span></span>

<span data-ttu-id="d4587-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4587-175">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
