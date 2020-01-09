---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 0c0f257a9bdcf6c149b4f6374e2011cebb437603
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994962"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="3ca6c-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ca6c-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ca6c-104">可以使用附件的形式向用户[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或组[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="3ca6c-105">组日历中的事件不支持附件。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-105">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="3ca6c-106">Outlook 任务不支持引用附件。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-106">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="3ca6c-107">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="3ca6c-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="3ca6c-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="3ca6c-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="3ca6c-109">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="3ca6c-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="3ca6c-110">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="3ca6c-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="3ca6c-111">**注意**：可以添加到 4 MB 以下的文件或项目附件的大小有限制。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-111">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="3ca6c-112">但是，如果您要附加到邮件的文件介于3MB 和150MB 之间，则可以[创建上载会话](../api/attachment-createuploadsession.md)并以迭代方式上载要附加的文件的范围。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-112">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="3ca6c-113">有关示例，请参阅[将大型文件附加到 Outlook 邮件](/graph/outlook-large-attachments)。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-113">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="3ca6c-114">方法</span><span class="sxs-lookup"><span data-stu-id="3ca6c-114">Methods</span></span>

<span data-ttu-id="3ca6c-115">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-115">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="3ca6c-116">方法</span><span class="sxs-lookup"><span data-stu-id="3ca6c-116">Method</span></span>       | <span data-ttu-id="3ca6c-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ca6c-117">Return Type</span></span>  |<span data-ttu-id="3ca6c-118">说明</span><span class="sxs-lookup"><span data-stu-id="3ca6c-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ca6c-119">获取附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-119">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3ca6c-120">attachment</span><span class="sxs-lookup"><span data-stu-id="3ca6c-120">attachment</span></span>](attachment.md) |<span data-ttu-id="3ca6c-121">读取附加到用户事件、邮件、Outlook 任务或帖子的附件的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-121">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="3ca6c-122">将附件添加到用户事件中</span><span class="sxs-lookup"><span data-stu-id="3ca6c-122">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="3ca6c-123">附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-123">attachment</span></span>](attachment.md) |<span data-ttu-id="3ca6c-124">将文件、项目或链接附件添加到用户日历中的事件中。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-124">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="3ca6c-125">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="3ca6c-125">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="3ca6c-126">附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-126">attachment</span></span>](attachment.md) |<span data-ttu-id="3ca6c-127">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-127">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="3ca6c-128">此操作将限制可添加到 4 MB 以下的附件的大小。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-128">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="3ca6c-129">创建会话以附加大型文件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-129">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="3ca6c-130">uploadSession</span><span class="sxs-lookup"><span data-stu-id="3ca6c-130">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="3ca6c-131">创建一个允许应用程序以迭代方式上载文件范围的上载会话，以便将文件附加到指定的**邮件**。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-131">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="3ca6c-132">文件大小必须介于3MB 和150MB 之间。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-132">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="3ca6c-133">将附件添加到 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="3ca6c-133">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="3ca6c-134">attachment</span><span class="sxs-lookup"><span data-stu-id="3ca6c-134">attachment</span></span>](attachment.md) |<span data-ttu-id="3ca6c-135">将文件或项目附件添加到 Outlook 任务中。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-135">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="3ca6c-136">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="3ca6c-136">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="3ca6c-137">附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-137">attachment</span></span>](attachment.md) |<span data-ttu-id="3ca6c-138">将文件、项目或链接附件添加到组帖子。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-138">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="3ca6c-139">列出用户事件的附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-139">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="3ca6c-140">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ca6c-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3ca6c-141">获取用户日历中事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-141">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="3ca6c-142">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-142">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="3ca6c-143">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ca6c-143">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3ca6c-144">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-144">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="3ca6c-145">列出 Outlook 任务的附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-145">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="3ca6c-146">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3ca6c-146">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3ca6c-147">获取 Outlook 任务的附件列表。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-147">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="3ca6c-148">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="3ca6c-148">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="3ca6c-149">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ca6c-149">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3ca6c-150">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-150">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="3ca6c-151">删除</span><span class="sxs-lookup"><span data-stu-id="3ca6c-151">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3ca6c-152">无</span><span class="sxs-lookup"><span data-stu-id="3ca6c-152">None</span></span> |<span data-ttu-id="3ca6c-153">删除事件、邮件、Outlook 任务或帖子上的附件。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-153">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ca6c-154">属性</span><span class="sxs-lookup"><span data-stu-id="3ca6c-154">Properties</span></span>

<span data-ttu-id="3ca6c-p104">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="3ca6c-157">属性</span><span class="sxs-lookup"><span data-stu-id="3ca6c-157">Property</span></span>     | <span data-ttu-id="3ca6c-158">类型</span><span class="sxs-lookup"><span data-stu-id="3ca6c-158">Type</span></span>   |<span data-ttu-id="3ca6c-159">说明</span><span class="sxs-lookup"><span data-stu-id="3ca6c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ca6c-160">contentType</span><span class="sxs-lookup"><span data-stu-id="3ca6c-160">contentType</span></span>|<span data-ttu-id="3ca6c-161">String</span><span class="sxs-lookup"><span data-stu-id="3ca6c-161">String</span></span>|<span data-ttu-id="3ca6c-162">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-162">The MIME type.</span></span>|
|<span data-ttu-id="3ca6c-163">id</span><span class="sxs-lookup"><span data-stu-id="3ca6c-163">id</span></span>|<span data-ttu-id="3ca6c-164">字符串</span><span class="sxs-lookup"><span data-stu-id="3ca6c-164">String</span></span>| <span data-ttu-id="3ca6c-165">只读。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-165">Read-only.</span></span>|
|<span data-ttu-id="3ca6c-166">isInline</span><span class="sxs-lookup"><span data-stu-id="3ca6c-166">isInline</span></span>|<span data-ttu-id="3ca6c-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ca6c-167">Boolean</span></span>|<span data-ttu-id="3ca6c-168">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-168">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="3ca6c-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ca6c-169">lastModifiedDateTime</span></span>|<span data-ttu-id="3ca6c-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ca6c-170">DateTimeOffset</span></span>|<span data-ttu-id="3ca6c-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3ca6c-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3ca6c-173">名称</span><span class="sxs-lookup"><span data-stu-id="3ca6c-173">name</span></span>|<span data-ttu-id="3ca6c-174">字符串</span><span class="sxs-lookup"><span data-stu-id="3ca6c-174">String</span></span>|<span data-ttu-id="3ca6c-175">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-175">The display name of the attachment.</span></span> <span data-ttu-id="3ca6c-176">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-176">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="3ca6c-177">size</span><span class="sxs-lookup"><span data-stu-id="3ca6c-177">size</span></span>|<span data-ttu-id="3ca6c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="3ca6c-178">Int32</span></span>|<span data-ttu-id="3ca6c-179">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-179">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ca6c-180">关系</span><span class="sxs-lookup"><span data-stu-id="3ca6c-180">Relationships</span></span>
<span data-ttu-id="3ca6c-181">无</span><span class="sxs-lookup"><span data-stu-id="3ca6c-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ca6c-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ca6c-182">JSON representation</span></span>

<span data-ttu-id="3ca6c-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ca6c-183">Here is a JSON representation of the resource</span></span>

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
