---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: a6810ff870124a793bee40ec9df66ae7cb5eabc8
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621657"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="ca068-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca068-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca068-104">可以使用附件的形式向用户[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或组[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="ca068-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="ca068-105">组日历中的事件不支持附件。</span><span class="sxs-lookup"><span data-stu-id="ca068-105">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="ca068-106">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="ca068-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="ca068-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="ca068-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="ca068-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="ca068-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="ca068-109">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="ca068-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="ca068-110">**注意**：由于在每个 REST 请求的总大小中目前有4mb 的限制，这通常会限制可添加到 4 mb 以下的文件或项目附件的大小。</span><span class="sxs-lookup"><span data-stu-id="ca068-110">**Note**: Since there is currently a limit of 4MB on the total size of each REST request, in general, this limits the size of the file or item attachment you can add to under 4MB.</span></span> 
>
> <span data-ttu-id="ca068-111">但是，如果您要附加到邮件的文件介于3MB 和150MB 之间，则可以[创建上载会话](../api/attachment-createuploadsession.md)并以迭代方式上载要附加的文件的范围。</span><span class="sxs-lookup"><span data-stu-id="ca068-111">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="ca068-112">有关示例，请参阅[将大型文件附加到 Outlook 邮件](/graph/outlook-large-attachments)。</span><span class="sxs-lookup"><span data-stu-id="ca068-112">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="ca068-113">方法</span><span class="sxs-lookup"><span data-stu-id="ca068-113">Methods</span></span>

<span data-ttu-id="ca068-114">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="ca068-114">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="ca068-115">方法</span><span class="sxs-lookup"><span data-stu-id="ca068-115">Method</span></span>       | <span data-ttu-id="ca068-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca068-116">Return Type</span></span>  |<span data-ttu-id="ca068-117">说明</span><span class="sxs-lookup"><span data-stu-id="ca068-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca068-118">获取附件</span><span class="sxs-lookup"><span data-stu-id="ca068-118">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ca068-119">attachment</span><span class="sxs-lookup"><span data-stu-id="ca068-119">attachment</span></span>](attachment.md) |<span data-ttu-id="ca068-120">读取附加到用户事件、邮件、Outlook 任务或帖子的附件的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="ca068-120">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="ca068-121">将附件添加到用户事件中</span><span class="sxs-lookup"><span data-stu-id="ca068-121">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="ca068-122">附件</span><span class="sxs-lookup"><span data-stu-id="ca068-122">attachment</span></span>](attachment.md) |<span data-ttu-id="ca068-123">将文件、项目或链接附件添加到用户日历中的事件中。</span><span class="sxs-lookup"><span data-stu-id="ca068-123">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="ca068-124">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="ca068-124">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="ca068-125">attachment</span><span class="sxs-lookup"><span data-stu-id="ca068-125">attachment</span></span>](attachment.md) |<span data-ttu-id="ca068-126">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="ca068-126">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="ca068-127">如果附加文件，文件大小必须小于4MB。</span><span class="sxs-lookup"><span data-stu-id="ca068-127">If attaching a file, the file size must be less than 4MB.</span></span>|
|[<span data-ttu-id="ca068-128">创建会话以附加大型文件</span><span class="sxs-lookup"><span data-stu-id="ca068-128">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="ca068-129">uploadSession</span><span class="sxs-lookup"><span data-stu-id="ca068-129">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="ca068-130">创建一个允许应用程序以迭代方式上载文件范围的上载会话，以便将文件附加到指定的**邮件**。</span><span class="sxs-lookup"><span data-stu-id="ca068-130">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="ca068-131">文件大小必须介于3MB 和150MB 之间。</span><span class="sxs-lookup"><span data-stu-id="ca068-131">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="ca068-132">将附件添加到 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="ca068-132">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="ca068-133">attachment</span><span class="sxs-lookup"><span data-stu-id="ca068-133">attachment</span></span>](attachment.md) |<span data-ttu-id="ca068-134">将文件、项目或链接附件添加到 Outlook 任务中。</span><span class="sxs-lookup"><span data-stu-id="ca068-134">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="ca068-135">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="ca068-135">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="ca068-136">附件</span><span class="sxs-lookup"><span data-stu-id="ca068-136">attachment</span></span>](attachment.md) |<span data-ttu-id="ca068-137">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="ca068-137">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="ca068-138">列出用户事件的附件</span><span class="sxs-lookup"><span data-stu-id="ca068-138">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="ca068-139">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca068-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ca068-140">获取用户日历中事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="ca068-140">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="ca068-141">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="ca068-141">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="ca068-142">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca068-142">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ca068-143">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="ca068-143">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="ca068-144">列出 Outlook 任务的附件</span><span class="sxs-lookup"><span data-stu-id="ca068-144">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="ca068-145">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca068-145">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ca068-146">获取 Outlook 任务的附件列表。</span><span class="sxs-lookup"><span data-stu-id="ca068-146">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="ca068-147">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="ca068-147">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="ca068-148">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca068-148">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ca068-149">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="ca068-149">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="ca068-150">删除</span><span class="sxs-lookup"><span data-stu-id="ca068-150">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ca068-151">无</span><span class="sxs-lookup"><span data-stu-id="ca068-151">None</span></span> |<span data-ttu-id="ca068-152">删除事件、邮件、Outlook 任务或帖子上的附件。</span><span class="sxs-lookup"><span data-stu-id="ca068-152">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca068-153">属性</span><span class="sxs-lookup"><span data-stu-id="ca068-153">Properties</span></span>

<span data-ttu-id="ca068-p104">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="ca068-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="ca068-156">属性</span><span class="sxs-lookup"><span data-stu-id="ca068-156">Property</span></span>     | <span data-ttu-id="ca068-157">类型</span><span class="sxs-lookup"><span data-stu-id="ca068-157">Type</span></span>   |<span data-ttu-id="ca068-158">说明</span><span class="sxs-lookup"><span data-stu-id="ca068-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca068-159">contentType</span><span class="sxs-lookup"><span data-stu-id="ca068-159">contentType</span></span>|<span data-ttu-id="ca068-160">String</span><span class="sxs-lookup"><span data-stu-id="ca068-160">String</span></span>|<span data-ttu-id="ca068-161">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="ca068-161">The MIME type.</span></span>|
|<span data-ttu-id="ca068-162">id</span><span class="sxs-lookup"><span data-stu-id="ca068-162">id</span></span>|<span data-ttu-id="ca068-163">字符串</span><span class="sxs-lookup"><span data-stu-id="ca068-163">String</span></span>| <span data-ttu-id="ca068-164">只读。</span><span class="sxs-lookup"><span data-stu-id="ca068-164">Read-only.</span></span>|
|<span data-ttu-id="ca068-165">isInline</span><span class="sxs-lookup"><span data-stu-id="ca068-165">isInline</span></span>|<span data-ttu-id="ca068-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca068-166">Boolean</span></span>|<span data-ttu-id="ca068-167">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="ca068-167">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="ca068-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca068-168">lastModifiedDateTime</span></span>|<span data-ttu-id="ca068-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca068-169">DateTimeOffset</span></span>|<span data-ttu-id="ca068-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ca068-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ca068-172">名称</span><span class="sxs-lookup"><span data-stu-id="ca068-172">name</span></span>|<span data-ttu-id="ca068-173">字符串</span><span class="sxs-lookup"><span data-stu-id="ca068-173">String</span></span>|<span data-ttu-id="ca068-174">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ca068-174">The display name of the attachment.</span></span> <span data-ttu-id="ca068-175">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="ca068-175">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="ca068-176">大小</span><span class="sxs-lookup"><span data-stu-id="ca068-176">size</span></span>|<span data-ttu-id="ca068-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ca068-177">Int32</span></span>|<span data-ttu-id="ca068-178">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="ca068-178">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca068-179">关系</span><span class="sxs-lookup"><span data-stu-id="ca068-179">Relationships</span></span>
<span data-ttu-id="ca068-180">无</span><span class="sxs-lookup"><span data-stu-id="ca068-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca068-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca068-181">JSON representation</span></span>

<span data-ttu-id="ca068-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca068-182">Here is a JSON representation of the resource</span></span>

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
