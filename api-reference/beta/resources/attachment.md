---
title: attachment 资源类型
description: 您可以向事件中添加相关内容,
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535555"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="e3bf5-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3bf5-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3bf5-104">您可以将相关内容添加到[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或以附件形式[发布](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="e3bf5-105">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="e3bf5-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="e3bf5-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="e3bf5-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="e3bf5-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="e3bf5-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="e3bf5-108">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="e3bf5-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="e3bf5-109">方法</span><span class="sxs-lookup"><span data-stu-id="e3bf5-109">Methods</span></span>

<span data-ttu-id="e3bf5-110">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="e3bf5-111">方法</span><span class="sxs-lookup"><span data-stu-id="e3bf5-111">Method</span></span>       | <span data-ttu-id="e3bf5-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3bf5-112">Return Type</span></span>  |<span data-ttu-id="e3bf5-113">说明</span><span class="sxs-lookup"><span data-stu-id="e3bf5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3bf5-114">获取附件</span><span class="sxs-lookup"><span data-stu-id="e3bf5-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e3bf5-115">attachment</span><span class="sxs-lookup"><span data-stu-id="e3bf5-115">attachment</span></span>](attachment.md) |<span data-ttu-id="e3bf5-116">读取附加到事件、邮件、Outlook 任务或帖子的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-116">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="e3bf5-117">Add attachment to an event</span><span class="sxs-lookup"><span data-stu-id="e3bf5-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="e3bf5-118">attachment</span><span class="sxs-lookup"><span data-stu-id="e3bf5-118">attachment</span></span>](attachment.md) |<span data-ttu-id="e3bf5-119">将文件、项目或链接附件添加到事件中。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="e3bf5-120">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="e3bf5-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="e3bf5-121">attachment</span><span class="sxs-lookup"><span data-stu-id="e3bf5-121">attachment</span></span>](attachment.md) |<span data-ttu-id="e3bf5-122">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="e3bf5-123">将附件添加到 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="e3bf5-123">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="e3bf5-124">attachment</span><span class="sxs-lookup"><span data-stu-id="e3bf5-124">attachment</span></span>](attachment.md) |<span data-ttu-id="e3bf5-125">将文件、项目或链接附件添加到 Outlook 任务中。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-125">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="e3bf5-126">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="e3bf5-126">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="e3bf5-127">附件</span><span class="sxs-lookup"><span data-stu-id="e3bf5-127">attachment</span></span>](attachment.md) |<span data-ttu-id="e3bf5-128">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-128">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="e3bf5-129">列出事件的附件</span><span class="sxs-lookup"><span data-stu-id="e3bf5-129">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="e3bf5-130">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3bf5-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e3bf5-131">获取事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-131">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="e3bf5-132">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="e3bf5-132">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="e3bf5-133">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3bf5-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e3bf5-134">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-134">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="e3bf5-135">列出 Outlook 任务的附件</span><span class="sxs-lookup"><span data-stu-id="e3bf5-135">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="e3bf5-136">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3bf5-136">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e3bf5-137">获取 Outlook 任务的附件列表。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-137">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="e3bf5-138">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="e3bf5-138">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="e3bf5-139">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3bf5-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e3bf5-140">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-140">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="e3bf5-141">删除</span><span class="sxs-lookup"><span data-stu-id="e3bf5-141">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e3bf5-142">无</span><span class="sxs-lookup"><span data-stu-id="e3bf5-142">None</span></span> |<span data-ttu-id="e3bf5-143">删除事件、邮件、Outlook 任务或帖子上的附件。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-143">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3bf5-144">属性</span><span class="sxs-lookup"><span data-stu-id="e3bf5-144">Properties</span></span>

<span data-ttu-id="e3bf5-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="e3bf5-147">属性</span><span class="sxs-lookup"><span data-stu-id="e3bf5-147">Property</span></span>     | <span data-ttu-id="e3bf5-148">类型</span><span class="sxs-lookup"><span data-stu-id="e3bf5-148">Type</span></span>   |<span data-ttu-id="e3bf5-149">说明</span><span class="sxs-lookup"><span data-stu-id="e3bf5-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3bf5-150">contentType</span><span class="sxs-lookup"><span data-stu-id="e3bf5-150">contentType</span></span>|<span data-ttu-id="e3bf5-151">String</span><span class="sxs-lookup"><span data-stu-id="e3bf5-151">String</span></span>|<span data-ttu-id="e3bf5-152">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-152">The MIME type.</span></span>|
|<span data-ttu-id="e3bf5-153">id</span><span class="sxs-lookup"><span data-stu-id="e3bf5-153">id</span></span>|<span data-ttu-id="e3bf5-154">String</span><span class="sxs-lookup"><span data-stu-id="e3bf5-154">String</span></span>| <span data-ttu-id="e3bf5-155">只读。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-155">Read-only.</span></span>|
|<span data-ttu-id="e3bf5-156">isInline</span><span class="sxs-lookup"><span data-stu-id="e3bf5-156">isInline</span></span>|<span data-ttu-id="e3bf5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3bf5-157">Boolean</span></span>|<span data-ttu-id="e3bf5-158">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-158">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="e3bf5-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3bf5-159">lastModifiedDateTime</span></span>|<span data-ttu-id="e3bf5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3bf5-160">DateTimeOffset</span></span>|<span data-ttu-id="e3bf5-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e3bf5-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e3bf5-163">name</span><span class="sxs-lookup"><span data-stu-id="e3bf5-163">name</span></span>|<span data-ttu-id="e3bf5-164">String</span><span class="sxs-lookup"><span data-stu-id="e3bf5-164">String</span></span>|<span data-ttu-id="e3bf5-165">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-165">The display name of the attachment.</span></span> <span data-ttu-id="e3bf5-166">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-166">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e3bf5-167">size</span><span class="sxs-lookup"><span data-stu-id="e3bf5-167">size</span></span>|<span data-ttu-id="e3bf5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e3bf5-168">Int32</span></span>|<span data-ttu-id="e3bf5-169">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-169">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3bf5-170">关系</span><span class="sxs-lookup"><span data-stu-id="e3bf5-170">Relationships</span></span>
<span data-ttu-id="e3bf5-171">无</span><span class="sxs-lookup"><span data-stu-id="e3bf5-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3bf5-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3bf5-172">JSON representation</span></span>

<span data-ttu-id="e3bf5-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3bf5-173">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
