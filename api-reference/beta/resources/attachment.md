---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 3faea96a9ef9c19c2d5471c1cc6f58ed84b9a2ef
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721626"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="99bc8-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="99bc8-103">attachment resource type</span></span>

<span data-ttu-id="99bc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99bc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="99bc8-105">您可以将相关内容以附件的形式添加到用户[事件](../resources/event.md)、[邮件](../resources/message.md)[、Outlook](../resources/outlooktask.md)任务或组[](../resources/post.md)帖子中。</span><span class="sxs-lookup"><span data-stu-id="99bc8-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="99bc8-106">组日历中的事件不支持附件。</span><span class="sxs-lookup"><span data-stu-id="99bc8-106">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="99bc8-107">Outlook 任务不支持引用附件。</span><span class="sxs-lookup"><span data-stu-id="99bc8-107">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="99bc8-108">**附件** 是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="99bc8-108">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="99bc8-109">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="99bc8-109">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="99bc8-110">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="99bc8-110">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="99bc8-111">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="99bc8-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="99bc8-112">**注意**：可以添加到的文件或项目附件的大小限制为 4 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="99bc8-112">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="99bc8-113">但是，如果要将介于 3MB 和 150MB 之间的文件附加到邮件，可以创建上载会话并反复[](../api/attachment-createuploadsession.md)上载文件范围以附加它。</span><span class="sxs-lookup"><span data-stu-id="99bc8-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="99bc8-114">有关 [示例，请参阅将大文件附加到 Outlook](/graph/outlook-large-attachments) 邮件。</span><span class="sxs-lookup"><span data-stu-id="99bc8-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="99bc8-115">方法</span><span class="sxs-lookup"><span data-stu-id="99bc8-115">Methods</span></span>

<span data-ttu-id="99bc8-116">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="99bc8-116">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="99bc8-117">方法</span><span class="sxs-lookup"><span data-stu-id="99bc8-117">Method</span></span>       | <span data-ttu-id="99bc8-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="99bc8-118">Return Type</span></span>  |<span data-ttu-id="99bc8-119">说明</span><span class="sxs-lookup"><span data-stu-id="99bc8-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99bc8-120">获取附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-120">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="99bc8-121">attachment</span><span class="sxs-lookup"><span data-stu-id="99bc8-121">attachment</span></span>](attachment.md) |<span data-ttu-id="99bc8-122">读取附加到用户事件、邮件、Outlook 任务或帖子的附件的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="99bc8-122">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="99bc8-123">将附件添加到用户事件中</span><span class="sxs-lookup"><span data-stu-id="99bc8-123">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="99bc8-124">附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-124">attachment</span></span>](attachment.md) |<span data-ttu-id="99bc8-125">将文件、项目或链接附件添加到用户日历中的事件中。</span><span class="sxs-lookup"><span data-stu-id="99bc8-125">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="99bc8-126">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="99bc8-126">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="99bc8-127">附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-127">attachment</span></span>](attachment.md) |<span data-ttu-id="99bc8-128">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="99bc8-128">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="99bc8-129">此操作将可添加到的附件大小限制在 4 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="99bc8-129">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="99bc8-130">创建会话以附加大文件</span><span class="sxs-lookup"><span data-stu-id="99bc8-130">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="99bc8-131">uploadSession</span><span class="sxs-lookup"><span data-stu-id="99bc8-131">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="99bc8-132">创建允许应用迭代上载文件范围的上载会话，以便将文件附加到指定 **消息**。</span><span class="sxs-lookup"><span data-stu-id="99bc8-132">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="99bc8-133">文件大小必须介于 3MB 和 150MB 之间。</span><span class="sxs-lookup"><span data-stu-id="99bc8-133">The file size must be between 3MB and 150MB.</span></span>|
|<span data-ttu-id="99bc8-134">[将附件添加到 Outlook 任务 (](../api/outlooktask-post-attachments.md) 已弃) </span><span class="sxs-lookup"><span data-stu-id="99bc8-134">[Add attachment to an Outlook task](../api/outlooktask-post-attachments.md) (deprecated)</span></span> | [<span data-ttu-id="99bc8-135">attachment</span><span class="sxs-lookup"><span data-stu-id="99bc8-135">attachment</span></span>](attachment.md) |<span data-ttu-id="99bc8-136">将文件或项目附件添加到 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="99bc8-136">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="99bc8-137">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="99bc8-137">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="99bc8-138">附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-138">attachment</span></span>](attachment.md) |<span data-ttu-id="99bc8-139">将文件、项目或链接附件添加到组帖子。</span><span class="sxs-lookup"><span data-stu-id="99bc8-139">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="99bc8-140">列出用户事件的附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-140">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="99bc8-141">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="99bc8-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="99bc8-142">获取用户日历中事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="99bc8-142">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="99bc8-143">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-143">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="99bc8-144">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99bc8-144">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="99bc8-145">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="99bc8-145">Get a list of attachments for a message.</span></span> |
|<span data-ttu-id="99bc8-146">[列出已弃 (](../api/outlooktask-list-attachments.md) Outlook 任务) </span><span class="sxs-lookup"><span data-stu-id="99bc8-146">[List attachments of an Outlook task](../api/outlooktask-list-attachments.md) (deprecated)</span></span> | <span data-ttu-id="99bc8-147">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="99bc8-147">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="99bc8-148">获取 Outlook 任务的附件列表。</span><span class="sxs-lookup"><span data-stu-id="99bc8-148">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="99bc8-149">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="99bc8-149">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="99bc8-150">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99bc8-150">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="99bc8-151">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="99bc8-151">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="99bc8-152">删除</span><span class="sxs-lookup"><span data-stu-id="99bc8-152">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="99bc8-153">无</span><span class="sxs-lookup"><span data-stu-id="99bc8-153">None</span></span> |<span data-ttu-id="99bc8-154">删除事件、邮件、Outlook 任务或帖子上的附件。</span><span class="sxs-lookup"><span data-stu-id="99bc8-154">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="99bc8-155">属性</span><span class="sxs-lookup"><span data-stu-id="99bc8-155">Properties</span></span>

<span data-ttu-id="99bc8-p104">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="99bc8-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="99bc8-158">属性</span><span class="sxs-lookup"><span data-stu-id="99bc8-158">Property</span></span>     | <span data-ttu-id="99bc8-159">类型</span><span class="sxs-lookup"><span data-stu-id="99bc8-159">Type</span></span>   |<span data-ttu-id="99bc8-160">说明</span><span class="sxs-lookup"><span data-stu-id="99bc8-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99bc8-161">contentType</span><span class="sxs-lookup"><span data-stu-id="99bc8-161">contentType</span></span>|<span data-ttu-id="99bc8-162">String</span><span class="sxs-lookup"><span data-stu-id="99bc8-162">String</span></span>|<span data-ttu-id="99bc8-163">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="99bc8-163">The MIME type.</span></span>|
|<span data-ttu-id="99bc8-164">id</span><span class="sxs-lookup"><span data-stu-id="99bc8-164">id</span></span>|<span data-ttu-id="99bc8-165">String</span><span class="sxs-lookup"><span data-stu-id="99bc8-165">String</span></span>| <span data-ttu-id="99bc8-166">只读。</span><span class="sxs-lookup"><span data-stu-id="99bc8-166">Read-only.</span></span>|
|<span data-ttu-id="99bc8-167">isInline</span><span class="sxs-lookup"><span data-stu-id="99bc8-167">isInline</span></span>|<span data-ttu-id="99bc8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="99bc8-168">Boolean</span></span>|<span data-ttu-id="99bc8-169">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="99bc8-169">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="99bc8-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99bc8-170">lastModifiedDateTime</span></span>|<span data-ttu-id="99bc8-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99bc8-171">DateTimeOffset</span></span>|<span data-ttu-id="99bc8-172">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="99bc8-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99bc8-173">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="99bc8-173">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="99bc8-174">name</span><span class="sxs-lookup"><span data-stu-id="99bc8-174">name</span></span>|<span data-ttu-id="99bc8-175">String</span><span class="sxs-lookup"><span data-stu-id="99bc8-175">String</span></span>|<span data-ttu-id="99bc8-176">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="99bc8-176">The display name of the attachment.</span></span> <span data-ttu-id="99bc8-177">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="99bc8-177">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="99bc8-178">size</span><span class="sxs-lookup"><span data-stu-id="99bc8-178">size</span></span>|<span data-ttu-id="99bc8-179">Int32</span><span class="sxs-lookup"><span data-stu-id="99bc8-179">Int32</span></span>|<span data-ttu-id="99bc8-180">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="99bc8-180">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99bc8-181">关系</span><span class="sxs-lookup"><span data-stu-id="99bc8-181">Relationships</span></span>
<span data-ttu-id="99bc8-182">无</span><span class="sxs-lookup"><span data-stu-id="99bc8-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99bc8-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99bc8-183">JSON representation</span></span>

<span data-ttu-id="99bc8-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99bc8-184">Here is a JSON representation of the resource</span></span>

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


